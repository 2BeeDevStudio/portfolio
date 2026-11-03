<div align="center">

# 강다원 · Portfolio

**6년차 백엔드 → 풀스택 개발자 · 비웍스(BeeWorks) 대표 · 개발팀장**

서버 셋업부터 운영까지, 만든 것을 끝까지 책임지는 개발자입니다.

[Portfolio Site](https://dawon.2bee.dev) · [Baton+](https://baton.2bee.dev) · [BeeWorks](https://2bee.dev) · dawon@beeworks.co.kr

</div>

---

## 프로젝트

> 제목을 누르면 프로젝트별 상세 문서(설계 · 트러블슈팅 · 회고)로 이동합니다.

| 프로젝트 | 한 줄 소개 | 역할 · 기간 | 핵심 스택 |
| --- | --- | --- | --- |
| **[Baton+](baton-plus/README.md)**<br>퇴사·휴직 인수인계 B2B SaaS | 문서·메일·카톡을 AI로 인계서 초안으로 정리하고, **빠진 일을 찾아 떠나기 전에 질문** | 자사 서비스 · **1인 기획·개발·운영**<br>2026.07 — 운영 중 | Java 21 · Spring Boot · PostgreSQL(pgvector) · React · Claude API |
| **[로테이션 소개팅 예약·운영 자동화](imweb-automation/README.md)**<br>아임웹 쇼핑몰 자동화 | 결제 웹훅 → 구글시트 → 카카오 알림톡, 외부 매칭 앱 API 연동까지 **무인 자동화** | 외주 · **서버 셋업부터 혼자**<br>2026.04 — 운영·유지보수 중 | Python · Flask · AWS EC2 · Apps Script |
| **[커머스 통합관리 ERP](commerce-erp/README.md)**<br>농수산물 유통 ERP | 주문·출고·정산·CS·마진 통합관리, 사방넷 API 연동 | **유지보수 · 기능 개선**<br>2025.09 — 2026.04 | Node.js · Express · React · MySQL |
| 베이커리 카페 브랜드 웹사이트 | 대한민국 제과명장 베이커리 — IA 설계 → 디자인 목업 → 아임웹 구현 | 외주 · 기획·제작<br>2026.10 — 진행 중 | 아임웹 · 생성형 AI |

---

## 프로젝트별 한눈에

**🏃 [Baton+](baton-plus/README.md)** — 퇴사·휴직 때 한 번 쓰는 인수인계 서비스. 정부 지원사업(사업화과제해결지원금) 선정.
- **누락 점검**: 회의록 할 일 표를 코드로 읽어 기한 지난 항목을 찾고, 완료 여부를 담당자 본인의 발언으로 검증해 확인 요청
- **근거 기반 RAG**: 인용 구절이 원문에 있는지 코드로 재검증, 평가 세트 채점으로 큰 오류 3건 → 0.7건
- **보안·운영**: 인계 단위 데이터 격리 · 원본 암호화 · 보관 기간 자동 파기, JUnit 410건 · 배포 전 취약점 스캔

**🤖 [로테이션 소개팅 예약·운영 자동화](imweb-automation/README.md)** — 주문부터 알림톡·참가자 관리까지 서버 셋업부터 운영까지 직접 만들었습니다.
- 웹훅 처리 지연(499 타임아웃)으로 주문이 누락되던 문제를 알림톡 발송 분리로 해결 (응답 2~5초 → 0.3초)
- EC2 + Elastic IP로 알림톡 고정 IP 요건을 해결하며 서버 비용 약 87% 절감 (Lambda + NAT 대비)
- Google Sheets API 클라이언트 재사용으로 메모리 800MB → 420MB 안정화

**🛠️ [커머스 통합관리 ERP](commerce-erp/README.md)** — 운영 중인 대형 ERP(컨트롤러 50여 개)를 유지보수했습니다.
- 출고율이 현장과 안 맞던 원인을 업무 관점(D-2 기준)에서 찾아 계산 기준을 바로잡았습니다
- 필터 상태 전체선택 버그처럼 데이터가 잘못 바뀔 수 있는 부분을 먼저 막았습니다

---

## 경력

| 기간 | 회사 | 역할 · 한 일 |
| --- | --- | --- |
| 2025.09 — 현재 | **비웍스(BeeWorks)** | 대표 · 개발팀장 — Baton+ 개발·운영, 외주 개발 |
| 2025.04 — 2025.09 | ㈜미르이즈 | 핀테크서비스본부 대리 — 시금고 세입·세출 유지보수, 쿼리 튜닝, 데이터센터 서버 이관 |
| 2020.01 — 2023.11 | 파인원커뮤니케이션즈 | 서비스플랫폼사업본부 연구원 — 숙박 플랫폼 ‘꿀스테이’ 백엔드 |

---

## 기술 스택

- **Backend** — Java (Spring Boot · Spring Security), Node.js (Express), Python (Flask)
- **Database** — PostgreSQL (pgvector), MySQL / MariaDB, Oracle, Redis, Flyway
- **Frontend** — React, TypeScript, Vite
- **AI** — Claude API, RAG, Ollama 임베딩
- **Infra** — AWS (EC2), Oracle Cloud, Docker Compose, Cloudflare Tunnel, Nginx, Vercel
- **연동** — Webhook, 카카오 알림톡(알리고), Google Sheets / Apps Script, 사방넷 Open API, AWS SES
