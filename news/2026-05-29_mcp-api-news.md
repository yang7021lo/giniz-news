## 🆕 오늘의 신간 (2026-05-29)

### MCP 서버 신간

1) Runway MCP Server
- 종류: MCP 서버 (공식 ⭐)
- 무엇이 새로운지: Runway가 MCP 서버를 신규 출시(공개)해 Claude/ChatGPT/Cursor 등 MCP 호환 에이전트에서 이미지·영상 생성 워크플로를 바로 연결.
- 핵심 기능 한 줄: 대화형 에이전트 안에서 Runway 영상/이미지 생성 모델을 ‘툴’처럼 호출.
- 가격/라이선스: Runway 기존 크레딧/요금제 기반(세부 단가는 사용 모델/설정에 따라 상이).
- 출처: KuCoin Flash 기사(인용: AiHot) https://www.kucoin.com/news/flash/runway-launches-model-context-protocol-server-for-ai-generated-media
- 참고: Runway 공식 뉴스 페이지에서는 MCP 서버 공지를 확인하지 못함. https://runwayml.com/news

### AI/LLM API 신간

1) Claude Opus 4.8 + Messages API 업데이트
- 종류: AI/LLM API (공식 ⭐)
- 무엇이 새로운지: Claude Opus를 4.8로 업데이트(5/28). 특히 Messages API에서 messages 배열 내부에 system entry를 허용해 작업 중간에 시스템 지시를 안전하게 갱신 가능.
- 핵심 기능 한 줄: 에이전트 실행 중 ‘system 지시’를 메시지 스트림에 끼워 넣어 정책/예산/환경 컨텍스트를 동적으로 바꾸면서도 프롬프트 캐시를 유지.
- 가격/라이선스: 기존 Opus 가격 동일(기사 내 표기 기준), fast mode 옵션 언급.
- 출처: Anthropic 뉴스룸 https://www.anthropic.com/news/claude-opus-4-8

2) GitHub Copilot에 Claude Opus 4.8 일반 제공
- 종류: AI/LLM API/플랫폼 업데이트 (공식 ⭐)
- 무엇이 새로운지: 5/28부터 GitHub Copilot(Pro+/Business/Enterprise)에서 Opus 4.8 사용 가능.
- 핵심 기능 한 줄: Copilot에서 더 향상된 코드 이해/생성 모델 선택지 제공.
- 가격/라이선스: Copilot 요금제 내 제공(별도 단가 공지 없음).
- 출처: GitHub Changelog https://github.blog/changelog/2026-05-28-claude-opus-4-8-is-generally-available-for-github-copilot/

### 마이너 업데이트
- OpenAI 쪽은 5/28~5/29 ‘API/개발자 플랫폼’ 기준으로 눈에 띄는 신규 릴리즈 노트 항목을 확인하지 못함(Releasebot 기준). https://releasebot.io/updates/openai

### 💡 CTO 메모 (Rails 8 B2B 영업 자동화, 옥상골프 SaaS, ERP/MES 관점)
- (Rails 8 B2B 영업 자동화) Claude Messages API의 system-in-messages는 “세일즈 에이전트가 중간에 정책/가격표/컴플라이언스 룰을 업데이트”해야 하는 시나리오에 유용. 예: 리드 스코어링 중 특정 업종은 영업 제외 룰이 추가되면, 대화 흐름을 끊지 않고 system entry로 즉시 반영.
- (옥상골프 SaaS) Runway MCP는 ‘콘텐츠 생산’(티저 영상/배너/짧은 홍보 영상)을 에이전트가 자동으로 만들고 CMS에 업로드하는 파이프라인에 바로 붙일 수 있음. 단, 공식 공지/가격표를 내부 문서에 고정하려면 Runway 1차 출처 확인이 필요.
- (ERP/MES) 엔터프라이즈 에이전트에서 중요한 건 “운영 중 정책 변경(권한, 예산, 안전)”을 안전하게 주입하는 메커니즘. Anthropic의 system-in-messages는 이런 운영 요구(런타임 거버넌스)에 더 가까운 형태.
