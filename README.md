# Jang Sungju | Security Operations · Network · Server Security Portfolio

VLAN·ACL 접근통제, Burp Suite 웹 요청 검증, Windows Server 취약점 점검 경험을 바탕으로 **윈스테크넷 보안관제 신입** 지원을 준비하고 있습니다. 통신 흐름과 로그·설정에 근거한 원인 분석, 결과 기록과 공유를 중요하게 생각합니다.

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
| Windows Server | 주요정보통신기반시설 기술적 취약점 분석·평가 가이드에 따른 계정·권한·보안 설정 점검 실습 |
| Security | Burp Suite HTTP 요청 파라미터 변조 실습, 웹 요청의 서버 측 검증 필요성 이해 |
| 협업 | 팀 프로젝트 PM 경험, 일정·이슈 정리 및 문제 해결 과정 기록 |

## Selected Projects

### 1. Closer — Safe Dugout 웹·네트워크 보안 점검/개선

K-Digital Training 팀 프로젝트 · **PM** · 약 1개월 반

- **네트워크:** Packet Tracer 기반 본사·지사 환경에서 VLAN 분리와 ACL 허용·차단 정책 구성, 필요한 통신이 접근통제 정책에 맞는지 검증
- **문제 해결:** 본사·지사 간 필요한 통신이 ACL 차단 규칙의 영향을 받는 상황을 확인하고 허용 규칙을 검토·수정하는 실습
- **웹 보안:** Burp Suite로 HTTP 요청의 포인트 파라미터 값을 100에서 1000으로 변경하는 실습. 클라이언트 입력을 그대로 신뢰하지 않고 서버에서 유효성·권한을 검증해야 하는 이유를 학습
- **협업:** PM으로 팀별 진행 상황, 일정 및 이슈 취합

### 2. AI Dev Team — 자연어 기반 AI 개발 자동화 대시보드 (진행 중)

- **목표:** 자연어로 개발 아이디어와 기능 요청을 입력하면 대시보드가 작업을 접수하고 구현·독립 검토·테스트 단계를 연결하도록 하는 범용 개발 자동화 플랫폼
- **AI 역할 분리:** Claude Code는 실제 코드 구현과 수정, Codex는 구현 결과의 독립적인 코드 리뷰·테스트 및 개선점 확인 담당
- **본인 역할:** 요구사항과 워크플로 설계, AI 도구별 역할 및 최종 승인 기준 정의, Docker·Colima 실행환경 구성, 컨테이너 상태·서비스 연결·작업 결과·로그 검증과 피드백. AI가 작성한 코드를 본인이 직접 구현했다고 표현하지 않음
- **개발 환경:** Mac mini, Docker, Colima, PostgreSQL, Redis, SSH
- **진행 상태:** 개발 자동화 흐름을 구성·보완 중. 인프라 운영 점검 자체가 프로젝트의 주된 목적은 아님

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

- **2026 충남 IT Hackathon 대상:** team2, 팀원으로 참가 · 팀 수상 (2026.11.14). 수상 증빙: 상장 발급 대기 중

- **K-Digital Training:** (정보보안) 웹서버개발 및 웹보안 솔루션 구축 융합과정, 코리아IT아카데미 (2025.06.11–2025.12.24)
- **2026 창업발명공모전 장려상 (개인 수상):** (사)국제문화기술진흥원 (2026.06.26)
