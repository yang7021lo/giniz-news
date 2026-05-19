## 🆕 오늘의 신간 (2026-05-20)

### MCP 서버 신간

오늘은 ‘새 MCP 서버 자체’의 신규 출시/등록 소식을 공식 채널(레지스트리/공식 레포)에서 24~48시간 범위로 특정하기 어려웠습니다. 대신, MCP를 실제로 쓰는 방식에 직접 영향이 있는 ‘MCP 연결/운영 기능’ 업데이트가 확인되어 아래에 포함했습니다.

### AI/LLM API 신간

- **MCP Tunnels (Research Preview)**
  - 종류: API (⭐ Anthropic Claude API)
  - 무엇이 새로운지: 신규 기능(리서치 프리뷰)
  - 핵심 기능 한 줄: 사설망(프라이빗 네트워크) 안의 MCP 서버에 Claude가 연결할 수 있도록 “MCP 터널”을 제공
  - 가격/라이선스: Claude API 요금 체계 내(세부는 문서 참조)
  - 출처: https://platform.claude.com/docs/en/release-notes/overview

- **Self-hosted Sandboxes for Claude Managed Agents**
  - 종류: API (⭐ Anthropic Claude API)
  - 무엇이 새로운지: 신규 기능
  - 핵심 기능 한 줄: Managed Agents의 툴 실행을 Anthropic 인프라 대신 고객이 직접 호스팅하는 샌드박스에서 수행 가능
  - 가격/라이선스: Claude API 요금 체계 내(세부는 문서 참조)
  - 출처: https://platform.claude.com/docs/en/release-notes/overview

- **Live session에서 MCP 서버/툴 구성 업데이트 지원 (Managed Agents)**
  - 종류: API (⭐ Anthropic Claude API)
  - 무엇이 새로운지: 기능 업데이트
  - 핵심 기능 한 줄: 진행 중인 세션에 연결된 MCP 서버/툴 구성을 런타임에 변경 가능
  - 가격/라이선스: Claude API 요금 체계 내(세부는 문서 참조)
  - 출처: https://platform.claude.com/docs/en/release-notes/overview

- **100K+ 토큰 툴 출력 자동 파일 스필(Managed Agents)**
  - 종류: API (⭐ Anthropic Claude API)
  - 무엇이 새로운지: 안정성/운영 업데이트
  - 핵심 기능 한 줄: agent_toolset/MCP 툴 출력이 100K 토큰을 넘으면 샌드박스 파일로 자동 저장하고, 모델에는 미리보기+파일 경로만 전달
  - 가격/라이선스: Claude API 요금 체계 내(세부는 문서 참조)
  - 출처: https://platform.claude.com/docs/en/release-notes/overview

### 마이너 업데이트

- **OpenAI API changelog(공식)에서 ‘2026-05-20’로 표기된 신규 항목은 확인되지 않았습니다.** (표시된 5/20 항목은 2025년으로 보임) 
  - 출처: https://developers.openai.com/api/docs/changelog

### 💡 CTO 메모 (Rails 8 B2B 영업 자동화, 옥상골프 SaaS, ERP/MES 관점)

- **MCP Tunnels = “사내망 데이터/툴을 SaaS 에이전트로 안전하게 끌어오는 길”**입니다. Rails 8 기반 B2B 영업 자동화에서 CRM/ERP가 사내망에 있거나, 고객사 VPN 내부에 있는 경우가 많습니다. 이때 ‘에이전트가 내부 MCP 서버에 연결’할 수 있으면, (1) 제안서/견적 자동화 (2) 거래처별 재고/납기 조회 (3) CS 이슈의 원인(생산/출하/설비) 역추적 같은 워크플로우가 빨라집니다.
- **Self-hosted sandbox는 규제/보안 산업 고객 설득 포인트**입니다. “모델은 외부지만 실행은 우리 망/우리 컨테이너” 구조가 가능해져, 옥상골프 SaaS에서도 결제/회원/예약/장비 로그 같은 민감 데이터 처리에 대해 설득력이 생깁니다.
- **100K+ 토큰 출력 스필은 ‘대용량 로그/리포트 자동 생성’ 운영 안정성**에 직결됩니다. ERP/MES 관점에서 하루치 생산/불량/설비 로그를 에이전트가 요약/분석할 때 출력이 커지는데, 이를 파일로 다루면 파이프라인을 더 견고하게 구성할 수 있습니다.
