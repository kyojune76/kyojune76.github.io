# kyojune76

한세대학교 IT학부 융합보안전공 · 2027년 2월 졸업 예정
Offensive Security / LLM · Agentic AI 기반 자율 취약점 발굴

## Skills
- Web Hacking
- Android Security
- Forensics (File Carving, Disk Imaging, 정적분석, 동적분석)
- LLM / Agentic AI 기반 보안 도구 개발
- JavaScript
- React / Node.js
- HTML / CSS
- Figma

---

## CVE / Vulnerability Research

### CVE-2026-65831 — ArcadeDB Privilege Escalation
- reader 권한만으로 JS 스크립팅에서 GraalVM 샌드박스를 우회해 호스트 파일을 읽는 권한상승 취약점 발굴
- CVSS 7.7 (High), GHSA-48qw-824m-86pr
- 제보 당일 메인테이너 패치 및 릴리스

### Portabase Master Key Overwrite
- 인증 없이 path traversal로 AES-256-GCM 마스터 키를 덮어쓰는 취약점 발굴
- CVSS 9.8 (Critical), GHSA-7697-vf3j-253j
- 제보 당일 메인테이너 패치 및 릴리스

### CVE-2025-23061 — Mongoose N-day Research
- 패치 소스코드를 직접 분석해, 패치된 버전(mongoose 8.9.5)에도 프로토타입 체인을 통한 우회 가능성이 잔존함을 발견
- 패치 적용만으로 위험이 해소되지 않음을 확인

---

## Experience

### AIBB (AI BunkerBuster)
**LLM 기반 자율 침투 테스트 시스템 개발 (팀장)**
- Docker 격리 환경에서 5개 취약점 환경 자동 공격 파이프라인 설계 및 구현
- Scanner(Nmap + Nuclei) → LLM 페이로드 생성 → HTTP 공격 → 피드백 루프 자동화
- 도구를 단계적으로 개방하는 능력 래더(L0~L3)를 고안해, 각 취약점이 어느 자율성 수준에서 풀리는지 정량 측정
- Phase별 전략(basic → encoding → advanced → creative)으로 70회 자동 시도 및 실패 학습
- 단발 RCE(shellshock, ssti, thinkphp)는 자율 해결, 다단계 익스플로잇(spring4shell)은 정확히 진단하고도 완주 실패하는 한계선을 규명
- Docker Manager, Scanner 통합, Autonomous Attack Bot 핵심 모듈 개발
- 기존 도구 30% 대비 80%+ 성공률 목표, 피드백 루프 효과 정량 측정

**기술**: Python, Docker, Nmap, Nuclei, Claude API, Git

### 차량 네트워크(CAN) 보안 — 구현 및 실데이터 분석
- CAN 버스의 브로드캐스트 및 ID 필터링 구조를 Python으로 직접 구현
- 실제 차량 공격 데이터를 분석해 DoS와 스푸핑의 탐지 난이도 차이를 규명하고 AI 기반 탐지의 필요성을 도출

### 교내 정보보호 연구실 연구실장 (2025.04 ~ 2025.11)
- 디스크 이미징, 파일 카빙, 악성코드 정적분석

---

## Featured Project

### MyShieldOn — On-device Android Security Checker
- 루팅 감지
- APK integrity 검증
- 금융앱 서명 hash값 무결성 검증
- ADB Mode 활성화 여부 확인
- 보안의식 낮은 고연령층 대상을 고려한 API 다양화 로직 사용
- 스토어 외 설치 APK 확인

Repository: https://github.com/kyojune76/MyShieldOn

---

## Awards

- 핵테온 세종 CTF 2026 — 웹 해킹 및 AI 보안 파트 전담, 250팀 중 47위
- picoCTF 2026 (Carnegie Mellon University) — 웹 및 AI 보안 파트, 전체 47위 (참가자 9,049명)

---

## Activity

- Dreamhack: https://dreamhack.io/users/83579
- Velog: https://velog.io/@kyojune1197/posts
