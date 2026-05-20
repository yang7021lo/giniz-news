## 🆕 오늘의 신간 (2026-05-21)

### MCP 서버 신간

- **Chrome DevTools MCP: v1.0.1**  
  - 종류: MCP 서버  
  - 무엇이 새로운지: 신규 릴리즈(태그: `chrome-devtools-mcp-v1.0.1`, 2026-05-18 공개)  
  - 핵심 기능: 에이전트/LLM이 Chrome DevTools 기능을 MCP로 호출해 브라우저 디버깅·자동화 워크플로에 연결  
  - 가격/라이선스: 오픈소스(라이선스는 저장소 기준 확인 필요)  
  - 출처: https://github.com/ChromeDevTools/chrome-devtools-mcp/releases/tag/chrome-devtools-mcp-v1.0.1

### AI/LLM API 신간

- ⭐ **OpenAI API: Secure MCP Tunnel(Enterprise)**  
  - 종류: API(플랫폼 기능 업데이트)  
  - 무엇이 새로운지: 2026-05-19 공개된 기능 업데이트  
  - 핵심 기능: ChatGPT/Codex/Responses API/AgentKit 등이 고객이 호스팅한 `tunnel-client`를 통해 사설망·온프레미스 MCP 서버에 연결(공개 인터넷 노출 없이)  
  - 가격/라이선스: Enterprise 계정 중심 GA(셀프서브 여부는 제한적)  
  - 출처: https://developers.openai.com/api/docs/changelog

- ⭐ **Anthropic Claude Platform: MCP tunnels(Research Preview) + Managed Agents 업데이트**  
  - 종류: API(플랫폼 기능 업데이트)  
  - 무엇이 새로운지: 2026-05-19 릴리즈 노트 반영  
  - 핵심 기능: (1) private network MCP 서버 연결용 MCP tunnels 프리뷰, (2) Managed Agents의 self-hosted sandbox 지원, (3) 실행 중 MCP/tool 설정 변경, (4) 대용량 tool output 파일 spill 지원  
  - 가격/라이선스: Claude Platform 기능(세부 과금은 공지 기준 확인 필요)  
  - 출처: https://platform.claude.com/docs/en/release-notes/overview

### 마이너 업데이트

- **Chrome DevTools MCP: 테스트 시나리오 업데이트(커밋)**  
  - 종류: MCP 서버(개발 업데이트)  
  - 무엇이 새로운지: 2026-05-20 커밋에서 experimentalPageIdRouting 플래그 대응 eval 시나리오 업데이트  
  - 핵심 기능: 평가/테스트 시나리오 정비로 안정성 개선  
  - 가격/라이선스: 오픈소스  
  - 출처: https://github.com/ChromeDevTools/chrome-devtools-mcp/commit/8e8e83e3f8d150689ffb58c3b977eb72016c7b3f

### 💡 CTO 메모 (Rails 8 B2B 영업 자동화, 옥상골프 SaaS, ERP/MES 관점)

- **‘MCP Tunnel’은 B2B 도입의 마지막 장애물(네트워크/보안)을 치우는 포인트**입니다. 사내망(ERP/MES, CRM, 파일서버)에 붙는 MCP 서버를 공개 인터넷에 노출하지 않고도 연결할 수 있으면, 보안팀 설득 비용이 급감합니다.
- **Rails 8 기반 영업 자동화**에서는 “리드→계약→청구”까지의 데이터 흐름을 MCP 도구로 표준화해두면, 모델/에이전트가 바뀌어도 툴 레이어는 재사용됩니다(벤더 락인 최소화).
- **옥상골프 SaaS**는 현장 운영 데이터(예약, 결제, 시설 점검, 멤버십)와 고객 커뮤니케이션(카카오/문자) 사이를 자동화할 때, MCP 서버를 ‘업무 자동화 버스’로 두고 API들을 붙이는 구조가 깔끔합니다.
