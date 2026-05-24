## 🆕 오늘의 신간 (2026-05-25)

### MCP 서버 신간

#### ⭐ AWS MCP Server (Agent Toolkit for AWS)
- 종류: MCP 서버
- 무엇이 새로운지: AWS가 **관리형(remote) MCP 서버**를 제공하며, **전체 AWS API 커버리지**(300+ 서비스/15,000+ API action)와 **샌드박스 Python 스크립트 실행**, **실시간 문서 검색/조회**, **CloudWatch + IAM 기반 제어**를 하나의 엔드포인트로 묶어 제공. ([AWS Agent Toolkit for AWS](https://aws.amazon.com/products/developer-tools/agent-toolkit-for-aws/))
- 핵심 기능 한 줄: “에이전트가 AWS를 안전하게 다루게 하려면 IAM/감사로그/문서검색/스크립트 실행을 한 번에 묶어야 한다”를 제품 형태로 구현.
- 가격/라이선스: Agent Toolkit for AWS는 **추가 비용 없이 제공**되며, 에이전트가 사용하는 AWS 리소스만 표준 요금으로 과금. ([AWS Agent Toolkit for AWS](https://aws.amazon.com/products/developer-tools/agent-toolkit-for-aws/))
- 참고: API 호출에는 IAM 자격증명이 필요하지만, **Agent skills와 문서 검색은 인증 없이도 가능**. ([AWS Agent Toolkit for AWS](https://aws.amazon.com/products/developer-tools/agent-toolkit-for-aws/))

#### ⭐ Azure MCP Server 1.0 (GA)
- 종류: MCP 서버
- 무엇이 새로운지: Microsoft가 **Azure MCP Server 1.0 GA**를 선언. ([Azure MCP Server (GitHub)](https://github.com/mcp/com.microsoft/azure))
- 핵심 기능 한 줄: “모든 Azure MCP 도구를 단일 서버로 제공” + **40+ Azure 서비스 컨텍스트**를 에이전트에 제공. ([Azure MCP Server (GitHub)](https://github.com/mcp/com.microsoft/azure))
- 가격/라이선스: (README 본문 기준) 명시 없음. ([Azure MCP Server (GitHub)](https://github.com/mcp/com.microsoft/azure))

#### ⭐ Amazon Devices Builder Tools (ADBT) MCP Server (Fire TV)
- 종류: MCP 서버
- 무엇이 새로운지: Amazon이 **Fire TV 개발용 ADBT for AI**를 공개했고, 구성 요소로 **ADBT MCP Server + Agent skills**를 포함. ([Amazon Appstore Developer Blog](https://developer.amazon.com/apps-and-games/blogs/2026/05/introducing-amazon-builder-tools))
- 핵심 기능 한 줄: Fire TV 개발 워크플로우(문서 검색/회수, 마이그레이션, 디버깅 등)를 에이전트가 바로 호출 가능한 툴/스킬로 제공.
- 가격/라이선스: 페이지 내 명시 없음. ([Amazon Appstore Developer Blog](https://developer.amazon.com/apps-and-games/blogs/2026/05/introducing-amazon-builder-tools))

### AI/LLM API 신간

- 오늘(최근 24~48시간) 기준으로는 “새 API 기능 출시/메이저 버전 공개” 성격의 공식 신간은 크게 확인되지 않음.

### 마이너 업데이트

- OpenAI: Status 페이지에 “**GPT-5.5 is now available to all paid users in Codex**” 공지가 표시됨(기능 배포 공지 성격). ([OpenAI Status – History](https://status.openai.com/history))

### 💡 CTO 메모 (Rails 8 B2B 영업 자동화, 옥상골프 SaaS, ERP/MES 관점)

- 관리형 MCP(예: AWS/Azure)는 ‘툴 호출’보다 **감사(CloudTrail/CloudWatch) + 권한(IAM) + 최신 문서(RAG) + 샌드박스 실행**을 패키징했다는 점이 핵심. 내부 ERP/MES 연동도 “API를 열어준다”보다 “권한/감사/실행 경계”를 먼저 제품화하면, 보안팀/감사 대응이 쉬워져 PoC→상용 전환이 빨라짐. ([AWS Agent Toolkit for AWS](https://aws.amazon.com/products/developer-tools/agent-toolkit-for-aws/))
- Rails 8 기반 B2B 영업 자동화는 (1) CRM/메일/캘린더/콜로그를 MCP로 표준화해 **에이전트가 ‘다음 행동’을 실행**하게 하고 (2) 실행은 반드시 “정책 엔진(허용/금지)” + “감사 로그”를 남기는 구조로 설계하는 게 장기적으로 유리.
- 옥상골프 SaaS는 ‘운영 자동화’(예약/정산/장비점검/고객문의) 쪽이 에이전트 ROI가 큼. ADBT처럼 **도메인 지식 + 워크플로우 스킬**을 미리 구성해두면, LLM 자체 교체(Claude/OpenAI/Google)에도 영향이 작아짐. ([Amazon Appstore Developer Blog](https://developer.amazon.com/apps-and-games/blogs/2026/05/introducing-amazon-builder-tools))
