## 🆕 오늘의 신간 (2026-05-27)

### MCP 서버 신간

- GitHub MCP Server: Secret Scanning 기능 GA
  - 종류: MCP 서버
  - 무엇이 새로운지: Secret scanning 지원이 Public Preview(2026-03)에서 GA로 전환(2026-05-05).
  - 핵심 기능 한 줄: MCP 호스트/에이전트(예: Copilot CLI, VS Code)에서 커밋/PR 전에 코드 변경분을 스캔해 시크릿(키/토큰 등) 유출을 사전 차단.
  - 가격/라이선스: GitHub Secret Protection 활성화 저장소 대상(플랜/정책에 따라 유료일 수 있음).
  - ⭐: ⭐ (GitHub 1st-party)
  - 출처: https://github.blog/changelog/2026-05-05-secret-scanning-with-github-mcp-server-is-now-generally-available/

### AI/LLM API 신간

- OpenAI API: 5월 중순 업데이트(최근 24~48시간 내 ‘신규’ 항목은 확인되지 않음)
  - 종류: API
  - 무엇이 새로운지: 2026-05-19 Secure MCP Tunnel(엔터프라이즈용), 2026-05-12 일부 모델/베타 엔드포인트 deprecate 등은 있었으나 5/26~5/27 신규 항목은 changelog에서 확인되지 않음.
  - 핵심 기능 한 줄: 사설/온프렘 MCP 서버를 퍼블릭 노출 없이 OpenAI 제품/플랫폼이 연결(터널 클라이언트 기반)하는 옵션(엔터프라이즈).
  - 가격/라이선스: 엔터프라이즈(계정 단위) 중심.
  - ⭐: ⭐
  - 출처: https://developers.openai.com/api/docs/changelog

### 마이너 업데이트

- (오늘 확인 범위 내) ‘어제~오늘’로 확정 가능한 추가 MCP 서버 릴리즈/대형 API 릴리즈 노트는 부족. 위 항목 중심으로 공유.

### 💡 CTO 메모 (Rails 8 B2B 영업 자동화, 옥상골프 SaaS, ERP/MES 관점)

- Secure MCP Tunnel 류(사설 MCP 서버를 터널로 안전 연결)는 “B2B 영업 자동화/ERP·MES”에서 특히 중요: 고객사 내부망(ERP/MES) 연동을 퍼블릭 인터넷에 노출하지 않고도 에이전트 워크플로우에 연결할 수 있는 표준 패턴이 됨.
- GitHub Secret Scanning MCP GA는 ‘개발 에이전트 도입’ 시 보안팀 설득 포인트: 커밋 이전 단계에서 키 유출을 자동 차단하는 통제 장치를 같이 제시하면, 에이전트 도입의 리스크를 ‘관리 가능한 형태’로 바꿀 수 있음.
