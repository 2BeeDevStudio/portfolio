# 포트폴리오

주문·업무 자동화부터 백엔드 아키텍처 설계, 대형 ERP 유지보수까지 — **서버 셋업부터 운영까지 직접 해온 풀스택 개발자**입니다.

📮 2beedevstudio@gmail.com · 🌐 [2bee.dev](https://2bee.dev)

---

## 프로젝트

| 프로젝트 | 한 줄 소개 | 나의 역할 | 핵심 스택 |
| --- | --- | --- | --- |
| **[아임웹 쇼핑몰 자동화](imweb-automation/README.md)** | 주문 수신 → 알림톡 → 구글시트 → 참가자 관리 완전 자동화 | 서버 셋업부터 **혼자 전부** | Python · Flask · AWS EC2 · GAS |
| **[Contix — 팀 지식·인수인계 도구](contix/README.md)** | 통화·문서를 정리하면 인수인계가 쌓이는 팀 도구 (정부지원 MVP 개발 중) | 기획 · 데이터 설계 · 백엔드 | Java 21 · Spring Boot · PostgreSQL(pgvector) |
| **[커머스 통합관리 ERP](commerce-erp/README.md)** | 주문·출고·정산·CS·마진 통합관리 시스템 | **유지보수 및 기능 개선** | Node.js · Express · React · MariaDB |

---

## 프로젝트별 한눈에

**🤖 아임웹 쇼핑몰 자동화** — 주문 수신부터 알림톡·구글시트 연동까지 서버 셋업부터 운영까지 직접 만들었습니다.
- EC2 + Elastic IP로 서버 비용을 낮췄습니다 (Lambda+NAT 방식 대비 약 87%)
- 발송이 실패해도 크론이 자동으로 재시도해 누락을 막았습니다
- Google Sheets API 객체를 매번 새로 만들던 걸 재사용하도록 바꿔 메모리를 800MB → 420MB로 안정화했습니다

**🧠 Contix** — 통화 메모·문서를 매일 정리하다 보면 인수인계가 쌓이는 팀 도구. 현재 정부지원사업 MVP를 개발 중입니다.
- 권한을 검색보다 먼저 적용해, 볼 수 없는 문서가 결과나 AI 답변에 섞이지 않게 했습니다
- AI 연동은 나중에 갈아끼울 수 있게 인터페이스로 분리했습니다 (지금은 스텁, 이후 Claude 연동)

**🛠️ 커머스 통합관리 ERP** — 운영 중인 대형 ERP를 유지보수했습니다.
- 출고율이 실제와 안 맞던 원인을 업무 관점(D-2 기준)에서 찾아 계산 기준을 바로잡았습니다
- 필터 상태 전체선택 버그처럼 데이터가 잘못 바뀔 수 있는 부분을 먼저 막았습니다

---

## 기술 스택 요약

- **Backend** — Java(Spring Boot), Node.js(Express), Python(Flask)
- **Database** — PostgreSQL(pgvector·pg_trgm), MariaDB/MySQL
- **Frontend** — React, Material-UI
- **Infra** — AWS EC2, Nginx, systemd/crontab, Docker, Vercel
- **연동** — Webhook, 알림톡(알리고), Google Sheets/Apps Script
