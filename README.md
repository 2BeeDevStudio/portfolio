<div align="center">

# 강다원 Portfolio

6년차 백엔드 개발자에서 풀스택으로 일하고 있습니다. 비웍스(BeeWorks) 대표이자 개발팀장입니다.

서버 셋업부터 운영까지, 만든 것은 끝까지 책임집니다.

[Portfolio Site](https://dawon.2bee.dev) · [Baton+](https://baton.2bee.dev) · [BeeWorks](https://2bee.dev) · dawon@beeworks.co.kr

</div>

---

## 프로젝트

> 제목을 누르면 프로젝트별 상세 문서(설계, 트러블슈팅, 회고)로 이동합니다.

| 프로젝트 | 한 줄 소개 | 역할 · 기간 | 핵심 스택 |
| --- | --- | --- | --- |
| [Baton+](baton-plus/README.md)<br>퇴사·휴직 인수인계 B2B SaaS | 문서, 메일, 카톡을 AI로 인계서 초안으로 정리하고, 빠진 일을 찾아 떠나기 전에 물어봅니다 | 자사 서비스, 1인 기획·개발·운영<br>2026.07 ~ 운영 중 | Java 21, Spring Boot, PostgreSQL, React, Claude API |
| [로테이션 소개팅 예약·운영 자동화](imweb-automation/README.md)<br>아임웹 쇼핑몰 자동화 | 결제 웹훅에서 구글 시트, 카카오 알림톡, 외부 매칭 앱 API 연동까지 사람 손 없이 돌아가게 만들었습니다 | 외주, 서버 셋업부터 혼자<br>2026.04 ~ 운영·유지보수 중 | Python, Flask, AWS EC2, Apps Script |
| [커머스 통합관리 ERP](commerce-erp/README.md)<br>농수산물 유통 ERP | 주문, 출고, 정산, CS, 마진 통합관리와 사방넷 API 연동 | 유지보수, 기능 개선<br>2025.09 ~ 2026.04 | Node.js, Express, React, MySQL |
| 베이커리 카페 브랜드 웹사이트 | 대한민국 제과명장 베이커리의 웹사이트를 IA 설계, 디자인 목업, 아임웹 구현 순서로 만들고 있습니다 | 외주, 기획·제작<br>2026.10 ~ 진행 중 | 아임웹, 생성형 AI |

---

## 프로젝트별로 조금 더

### [Baton+](baton-plus/README.md)

퇴사나 휴직 때 한 번 쓰는 인수인계 서비스입니다. 정부 지원사업(사업화과제해결지원금)에 선정됐습니다.

- 회의록의 할 일 표를 코드로 읽어 기한이 지난 항목을 찾고, 완료됐다는 말이 담당자 본인의 발언인지 확인한 뒤 인계자에게 물어봅니다.
- AI 답변의 인용 구절이 원문에 실제로 있는지 코드로 다시 확인합니다. 평가 세트를 만들어 채점하면서 큰 오류를 3건에서 0.7건으로 줄였습니다.
- 인계 단위로 데이터를 나누고, 원본 파일을 암호화해 저장하고, 보관 기간이 지나면 자동으로 지웁니다. JUnit 테스트 410건과 배포 전 취약점 점검을 거쳐 배포합니다.

### [로테이션 소개팅 예약·운영 자동화](imweb-automation/README.md)

주문 접수부터 알림톡 발송, 참가자 관리까지 서버 셋업부터 운영까지 직접 만들었습니다.

- 웹훅 처리가 늦어(499 타임아웃) 주문이 빠지던 문제를 알림톡 발송을 따로 떼어 해결했습니다. 응답이 2~5초에서 0.3초로 줄었습니다.
- 알림톡의 고정 IP 요건을 EC2와 Elastic IP로 맞춰, Lambda와 NAT를 쓰는 방식보다 서버 비용을 약 87% 줄였습니다.
- Google Sheets API 클라이언트를 재사용하도록 바꿔 메모리를 800MB에서 420MB로 안정시켰습니다.

### [커머스 통합관리 ERP](commerce-erp/README.md)

컨트롤러가 50개가 넘는, 운영 중인 큰 ERP를 유지보수했습니다.

- 출고율이 현장 체감과 맞지 않던 원인을 업무 기준(D-2)에서 찾아 계산 기준을 바로잡았습니다.
- 필터를 건 상태에서 전체 선택하면 보이지 않는 데이터까지 바뀌는 버그처럼, 데이터가 잘못 바뀔 수 있는 부분부터 먼저 막았습니다.

---

## 경력

| 기간 | 회사 | 역할 · 한 일 |
| --- | --- | --- |
| 2025.09 ~ 현재 | 비웍스(BeeWorks) | 대표, 개발팀장. Baton+ 개발·운영, 외주 개발 |
| 2025.04 ~ 2025.09 | ㈜미르이즈 | 핀테크서비스본부 대리. 시금고 세입·세출 유지보수, 쿼리 튜닝, 데이터센터 서버 이관 |
| 2020.01 ~ 2023.11 | 파인원커뮤니케이션즈 | 서비스플랫폼사업본부 연구원. 숙박 플랫폼 '꿀스테이' 백엔드 |

---

## 기술 스택

| 구분 | 기술 |
| --- | --- |
| Backend | Java (Spring Boot, Spring Security), Node.js (Express), Python (Flask) |
| Database | PostgreSQL (pgvector), MySQL, MariaDB, Oracle, Redis, Flyway |
| Frontend | React, TypeScript, Vite |
| AI | Claude API, RAG, Ollama 임베딩 |
| Infra | AWS (EC2), Oracle Cloud, Docker Compose, Cloudflare Tunnel, Nginx, Vercel |
| 연동 | Webhook, 카카오 알림톡(알리고), Google Sheets, Apps Script, 사방넷 Open API, AWS SES |
