## 🆕 오늘의 신간 (2026-05-26)

### MCP 서버 신간

(오늘 확인된 신규 MCP 서버 런칭/릴리즈 없음)

### AI/LLM API 신간

1) OpenAI: Secure MCP Tunnel (엔터프라이즈)
- 종류: API
- 무엇이 새로운지: 신규 기능(엔터프라이즈용)
- 핵심 기능 한 줄: 고객이 호스팅하는 `tunnel-client`를 통해 사내/온프레미스 MCP 서버에 외부 노출 없이 연결.
- 가격/라이선스: 엔터프라이즈 고객 대상(계정 기반 제공)
- ⭐: ⭐
- 출처: https://developers.openai.com/api/docs/changelog

2) Anthropic: Claude Developer Platform/Managed Agents – MCP Tunnels(Research Preview) + Self-hosted Sandboxes(Public Beta)
- 종류: API
- 무엇이 새로운지: 신규 기능(프리뷰/베타)
- 핵심 기능 한 줄: 사내 네트워크 내 MCP 서버에 에이전트가 접근하도록 ‘MCP 터널’을 제공하고, 툴 실행 샌드박스를 고객 인프라로 옮길 수 있게 지원.
- 가격/라이선스: (공식 가격 표기는 출처에서 확인 필요)
- ⭐: ⭐
- 출처: https://releasebot.io/updates/anthropic

### 마이너 업데이트

- Anthropic Claude Code v2.1.149~150: `/usage`에 MCP 서버별 비용 등 사용량 인사이트 강화, 엔터프라이즈 managed setting에 claude.ai 클라우드 MCP 커넥터 로드 옵션 추가.
  - 출처: https://releasebot.io/updates/anthropic

### 💡 CTO 메모 (Rails 8 B2B 영업 자동화, 옥상골프 SaaS, ERP/MES 관점)

- Rails 8 기반 B2B 영업 자동화에서 ‘사내 자산(ERP/MES/CS DB)’을 안전하게 연결하려면, 이번에 양대 진영(OpenAI/Anthropic)이 모두 ‘MCP 터널’ 계열을 밀고 있다는 점이 힌트입니다. 핵심은 “에이전트는 외부에 있어도, 툴/데이터는 사내에 둔 채 안전하게 호출” 구조로 전환하는 것.
- 옥상골프 SaaS는 현장 장비/센서/예약/결제/고객지원이 섞이므로, MCP 서버를 ‘현장 운영용 툴링 게이트웨이’로 두고(예: 예약/락커/키오스크 제어), 외부 LLM에는 터널로만 접근시키면 보안/운영이 쉬워집니다.
- ERP/MES 관점에서는 “도메인별 MCP 서버”를 잘게 쪼개고(생산실적, 재고, 납기, 품질 등), 터널 기반으로 연결하면 감사/권한/로그 설계가 수월합니다. 특히 엔터프라이즈용 터널은 네트워크/인증 표준(OAuth/OIDC) 정합성을 확보하는 방향으로 가는 중이라, 지금부터 권한모델을 표준에 맞춰 두는 게 장기적으로 유리합니다.
