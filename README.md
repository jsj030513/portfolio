# Jang Sungju | Infrastructure · Network · Security Portfolio

Linux 기반 시스템과 네트워크의 안정적 운영, 로그와 설정값에 근거한 장애 원인 분석에 관심이 있습니다. **KIS정보통신 데이터센터 시스템 관리** 등 인프라·보안 관련 신입 직무를 준비하고 있습니다.

- **Portfolio:** https://jsj030513.github.io/portfolio/
- **GitHub:** https://github.com/jsj030513

> 아래 활동은 교육과 개인 프로젝트에서의 경험입니다. 실제 기업 데이터센터 운영 경력은 없으며, AI가 구현한 코드와 제가 기획·구성·검증한 역할을 구분합니다.

## Infrastructure & Technical Skills

| 분야 | 학습 및 경험 |
| --- | --- |
| Linux / 운영 점검 | 프로세스·CPU·네트워크 연결·디스크 상태 확인 기초 (`top`, `ps`, `ss`, `df`, `du`), SSH 활용 |
| Containers | Mac mini에서 Docker·Colima 기반 개발 환경 구성 및 컨테이너 상태 점검 |
| Service / DB | PostgreSQL·Redis 실행 상태와 서비스 연동 확인, 애플리케이션 Health Check·로그 확인 |
| Network | Packet Tracer·GNS3, VLAN, ACL, Routing 및 본사·지사 간 통신 점검 |
| Security | Burp Suite HTTP 요청 파라미터 변조 실습, 웹 요청의 서버 측 검증 필요성 이해 |
| 협업 | 팀 프로젝트 PM 경험, 일정·이슈 정리 및 문제 해결 과정 기록 |

## Selected Projects

### 1. AI Dev Team — 로컬 AI 개발 자동화 환경 (진행 중)

- **목표:** 대시보드에서 개발 요청을 받아 AI 도구별 구현·검토·QA 단계를 연결하는 자동화 작업 흐름 구상 및 구성
- **환경:** Mac mini, Docker, Colima, PostgreSQL, Redis, SSH
- **운영 경험:** 컨테이너 상태, 서비스 포트, 실행 로그와 Health Check를 활용해 구성요소가 동작하고 연동되는지 점검
- **본인 역할:** 작업 흐름·역할 분담 설계, 로컬 환경 구성 및 점검, 진행 상황 검증. AI 도구가 작성한 코드를 전부 직접 구현했다고 표현하지 않음
- **직무 연관성:** 여러 서비스가 연결된 환경에서 문제 구간을 분리하고 서비스 상태를 확인하는 경험

### 2. Closer — Safe Dugout 웹·네트워크 보안 점검/개선

K-Digital Training 팀 프로젝트 · **PM** · 약 1개월 반

- **네트워크:** Packet Tracer 기반 본사·지사 환경에서 VLAN 분리와 ACL 허용·차단 정책 구성
- **문제 해결:** 본사·지사 간 필요한 통신이 ACL 차단 규칙의 영향을 받는 상황을 확인하고 허용 규칙을 검토·수정하는 실습
- **웹 보안:** Burp Suite로 HTTP 요청의 포인트 파라미터 값을 100에서 1000으로 변경하는 실습. 클라이언트 입력을 그대로 신뢰하지 않고 서버에서 유효성·권한을 검증해야 하는 이유를 학습
- **협업:** PM으로 팀별 진행 상황, 일정 및 이슈 취합

### 3. 함께걸음 — 배리어프리 정보·돌봄회원 매칭 웹 서비스

K-Digital Training 팀 프로젝트 · **부팀장** · 약 1개월 반

- 회원가입·로그인·마이페이지 등 프론트엔드와 백엔드 기능 구현에 참여
- 팀 진행 상황을 확인하고 일정이 지연된 작업의 개발 지원
- [Frontend Repository](https://github.com/jsj030513/workTogether_frontend) · [Backend Repository](https://github.com/jsj030513/workTogether_backend)

### 4. Project Eden — 웹 게임 프로젝트 (진행 중)

- 캐릭터·월드 상호작용 기능 기획과 테스트 수행
- Spring Boot, PostgreSQL, JWT, Docker Compose, React/Vite 등의 프로젝트 기술 구성 이해
- 코드 구현에 활용한 AI 도구와 본인의 기획·테스트 역할 구분
- [Backend Repository](https://github.com/jsj030513/project-eden-backend) · [Frontend Repository](https://github.com/jsj030513/project-eden-frontend)

### 5. ARB//KOREA — 거래소 가격 비교·자동화 시스템

- 거래소 가격 비교, 거래 및 운영 안전장치가 포함된 개인 프로젝트
- Docker 실행환경, 비밀정보 관리 및 운영 안전장치에 관심을 두고 점검
- [Repository](https://github.com/jsj030513/Coin)

## Troubleshooting Approach

**현상 확인 → 로그·설정 분석 → 문제 구간 분리 → 조치 검증 → 결과 기록**

- 네트워크 문제에서는 VLAN, 게이트웨이, 라우팅, ACL을 분리해 점검
- 서버·컨테이너 문제에서는 프로세스·포트·서비스 상태와 로그를 확인
- 보안 이벤트에서는 탐지 기록을 실제 침해 여부와 구분해 해석

## Education & Award

- **K-Digital Training:** (정보보안) 웹서버개발 및 웹보안 솔루션 구축 융합과정, 코리아IT아카데미 (2025.06.11–2025.12.24)
- **2026 창업발명공모전 장려상:** (사)국제문화기술진흥원 (2026.06.26)
