## 🆕 오늘의 신간 (2026-05-28)

### MCP 서버 신간

- **Google Ads MCP Server (Experimental)**
  - 종류: MCP 서버
  - 무엇이 새로운지: (공식/대형사) Google Ads API를 MCP 서버 형태로 제공하는 공개 저장소가 확인됨
  - 핵심 기능: LLM/에이전트가 Google Ads 계정/고객 목록을 조회하는 도구를 호출 가능
  - 가격/라이선스: 오픈소스 (Apache-2.0)
  - ⭐: Google 계열(googleads)
  - 출처: [GitHub - googleads/google-ads-mcp](https://github.com/googleads/google-ads-mcp)

### AI/LLM API 신간

- **Claude Platform: MCP Tunnels (Research Preview)**
  - 종류: API/플랫폼 업데이트
  - 무엇이 새로운지: 사설 네트워크(프라이빗 네트워크) 내부의 MCP 서버에 연결할 수 있는 MCP tunnels가 Research Preview로 제공
  - 핵심 기능: 사내망 MCP 서버를 외부 호스트/에이전트에서 더 쉽게 연결
  - 가격/라이선스: Claude Platform 정책에 따름(유료)
  - ⭐: Anthropic
  - 출처: [Claude Platform release notes](https://platform.claude.com/docs/en/release-notes/overview)

### 마이너 업데이트

- **Gemini API (May 2026): Managed Agents Public Preview + gemini-3.5-flash GA**
  - 종류: API 업데이트
  - 무엇이 새로운지: Gemini API에서 관리형 에이전트(샌드박스 실행)가 퍼블릭 프리뷰로 공개되고, gemini-3.5-flash가 GA로 릴리즈
  - 핵심 기능: 상태ful 에이전트/코드 실행/파일 관리가 가능한 샌드박스형 에이전트 운영
  - 가격/라이선스: Google AI for Developers 정책에 따름
  - ⭐: Google
  - 출처: [Gemini API release notes](https://ai.google.dev/gemini-api/docs/changelog)

### 💡 CTO 메모 (Rails 8 B2B 영업 자동화, 옥상골프 SaaS, ERP/MES 관점)

- **Rails 8 B2B 영업 자동화**: MCP tunnels류 기능이 의미 있는 이유는, ‘에이전트가 사내 CRM/ERP/문서 시스템에 붙는 마지막 1마일’을 네트워크/보안 요구사항 때문에 막히는 경우가 많기 때문입니다. 고객사 온프렘/사내망 연동은 (1) 프록시/터널 (2) 인증/권한 모델 (3) 감사로그가 세트로 가야 B2B 도입이 됩니다.
- **옥상골프 SaaS**: 예약/결제/회원/코치 스케줄을 LLM이 직접 건드리게 하지 말고, MCP 서버(툴)로 ‘허용된 트랜잭션’만 열어두는 방식이 운영 안정성에 유리합니다(예: “회원 환불 가능 여부 조회”, “예약 가능 슬롯 추천”처럼 읽기/제약된 쓰기 분리).
- **ERP/MES**: Google Ads MCP 같은 ‘대형사 API → MCP 서버 래핑’ 패턴은 ERP/MES에서도 재현 가능합니다(예: “작업지시 조회”, “불량률 리포트 생성”). 다만 MES는 실시간/권한/감사 이슈가 크므로, MCP 서버에 role-based tool gating과 실행 결과 아카이빙(파일 spill) 설계를 같이 넣는 게 좋습니다.
