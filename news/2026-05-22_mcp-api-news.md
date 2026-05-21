## 🆕 오늘의 신간 (2026-05-22)

### MCP 서버 신간

- ⭐ **Chrome DevTools for agents (MCP server) stable 1.0**
  - 종류: MCP 서버
  - 무엇이 새로운지: stable 1.0 release (신규 안정판 공개)
  - 핵심 기능 한 줄: LLM/에이전트가 DevTools 디버깅 기능을 MCP로 구조화 호출
  - 가격/라이선스: 오픈소스(레포 기반 배포) / 가격 정보는 문서 내 별도 언급 없음
  - 출처: [Chrome for Developers](https://developer.chrome.com/blog/devtools-for-agents-v1?hl=en)

- **Devart MCP Servers 제품 라인(19개 + Universal MCP Server)**
  - 종류: MCP 서버(상용 제품 라인)
  - 무엇이 새로운지: 신규 MCP Servers 제품 라인 출시
  - 핵심 기능 한 줄: Universal MCP Server로 ODBC 기반 거의 모든 데이터 소스를 에이전트에 연결(온프렘 지원)
  - 가격/라이선스: 상용(가격은 글에서 구체 미기재)
  - 출처: [Devart Blog](https://www.devart.com/blog/devart-brings-ai-agents-closer-to-enterprise-data-with-new-mcp-server-product-line.html)

- **Dub MCP Server**
  - 종류: MCP 서버
  - 무엇이 새로운지: Dub MCP Server 출시
  - 핵심 기능 한 줄: Dub API를 MCP tools로 제공(파트너/신청/커미션 관리 등)
  - 가격/라이선스: all plans에서 GA(별도 가격 언급 없음)
  - 출처: [Dub Blog](https://dub.co/blog/dub-mcp-server)

### AI/LLM API 신간

- ⭐ **OpenAI API: Secure MCP Tunnel (Enterprise)**
  - 종류: API(플랫폼 기능)
  - 무엇이 새로운지: Secure MCP Tunnel 출시(Enterprise 대상, account-led GA)
  - 핵심 기능 한 줄: 고객이 호스팅하는 `tunnel-client`로 사설/온프렘 MCP 서버를 인터넷에 노출하지 않고 연결
  - 가격/라이선스: 유료(Enterprise 범주, self-serve 아님)
  - 출처: [OpenAI API Changelog](https://developers.openai.com/api/docs/changelog)

- ⭐ **OpenAI API: Realtime 2 / Translate / Whisper (Realtime 계열 신규 모델/엔드포인트 업데이트)**
  - 종류: API
  - 무엇이 새로운지: Realtime 2(음성-음성, reasoning 설정), Realtime Translate(스트리밍 번역), Realtime Whisper(스트리밍 STT) 공개
  - 핵심 기능 한 줄: 실시간 음성 에이전트용 모델 라인업 확장
  - 가격/라이선스: 유료(플랫폼 과금, 글 내 상세 요금은 미기재)
  - 출처: [OpenAI API Changelog](https://developers.openai.com/api/docs/changelog)

- ⭐ **Claude Platform: MCP tunnels(Research Preview) + Managed Agents self-hosted sandboxes(Public Beta)**
  - 종류: API/플랫폼
  - 무엇이 새로운지: MCP tunnels(Research Preview), self-hosted sandboxes(Public Beta), 세션 중 MCP 서버/툴 설정 라이브 업데이트, 대용량 tool output 파일 spill
  - 핵심 기능 한 줄: 엔터프라이즈 경계 내에서 에이전트 실행/툴 호출을 더 안전하게 운영
  - 가격/라이선스: 미기재(Preview/Beta)
  - 출처: [Claude Platform Release Notes](https://platform.claude.com/docs/en/release-notes/overview)

- ⭐ **Gemini API: Managed Agents Public Preview + Antigravity Agent + File Search 업데이트(멀티모달)**
  - 종류: API
  - 무엇이 새로운지: Managed Agents(구글 호스팅 리눅스 샌드박스) 공개 프리뷰, `antigravity-preview-05-2026` 공개 프리뷰, File Search 멀티모달 검색 지원
  - 핵심 기능 한 줄: 상태 유지형 자율 에이전트를 샌드박스에서 운영 + 문서/이미지까지 검색 기반 컨텍스트 확장
  - 가격/라이선스: 미기재(Preview)
  - 출처: [Gemini API Release notes](https://ai.google.dev/gemini-api/docs/changelog)

### 마이너 업데이트

- ⭐ **OpenAI API: Realtime API Beta deprecate/remove 및 DALL·E 2/3 스냅샷 제거**
  - 종류: API
  - 무엇이 새로운지: Realtime API Beta 종료 및 released Realtime API로 마이그레이션 안내, 구 DALL·E 스냅샷 제거
  - 핵심 기능 한 줄: 레거시 제거로 인터페이스 정리(대체 모델/가이드 제시)
  - 출처: [OpenAI API Changelog](https://developers.openai.com/api/docs/changelog)

### 💡 CTO 메모 (Rails 8 B2B 영업 자동화, 옥상골프 SaaS, ERP/MES 관점)

- Rails 8 기반 B2B 영업 자동화에선 “사설 데이터 접근”이 가장 큰 병목입니다. 오늘 신간 중 OpenAI/Claude의 MCP tunnel 흐름은, 리드/견적/계약/CS 등 내부 시스템을 **인터넷 공개 없이** 에이전트에 붙이는 아키텍처(=보안팀 설득 포인트)를 구체화합니다.
- 옥상골프 SaaS는 장비/예약/정산/멤버십이 얽혀서 운영 자동화 니즈가 큽니다. Dub처럼 도메인 API를 MCP toolset으로 제공하면 ‘운영자 콘솔 클릭’을 에이전트 액션으로 치환하기 쉬워집니다(파트너/정산/수수료처럼 규칙 기반 업무부터).
- ERP/MES는 ODBC로 “읽기”를 먼저 개방하는 게 현실적입니다. Devart Universal MCP Server는 온프렘 ODBC 자산을 빠르게 연결하는 옵션이지만, **쓰기(주문/생산지시)** 는 승인 워크플로·감사로그·권한 모델이 선행돼야 합니다(툴을 좁게 설계).
