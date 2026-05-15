## 🆕 오늘의 신간 (2026-05-16)

### MCP 서버 신간

#### AWS MCP Server (GA)
- 종류: MCP 서버 (⭐ 공식)
- 무엇이 새로운지: 프리뷰(re:Invent 2025)에서 **정식 출시(GA)**

- 핵심 기능 한 줄: 코딩 에이전트가 MCP를 통해 AWS 서비스에 **안전하고 감사 가능한 방식**으로 접근

- 가격/라이선스: 서버 자체는 **추가 비용 없음**, 사용한 AWS 리소스만 과금

- 출처: <https://aws.amazon.com/about-aws/whats-new/2026/05/aws-mcp-server/>

### AI/LLM API 신간

#### Google Gemini Interactions API (v1beta) 스키마 변경(브레이킹 체인지) 안내
- 종류: API (⭐ 공식)
- 무엇이 새로운지: `outputs` → `steps`로 응답 구조가 바뀌고, `response_format`으로 출력 포맷 설정이 통합되는 등 **브레이킹 체인지**

- 핵심 기능 한 줄: 향후 *mid-flight steering* 및 **비동기 tool call** 같은 기능 확장을 위한 API 형태 재정비

- 가격/라이선스: 기존 Gemini API 정책 따름(문서 내 가격 변경 언급 없음)
- 개발자 액션: 

  - (SDK) Python/JS SDK를 **2.0.0 이상**으로 업그레이드

  - (REST) 5/26 기본 전환 전까지 `Api-Revision: 2026-05-20` 헤더로 사전 적용 가능

  - 5/26 이후 6/8까지는 `Api-Revision: 2026-05-07`로 임시 옵트아웃 가능

- 출처: <https://ai.google.dev/gemini-api/docs/interactions-breaking-changes-may-2026>

#### OpenAI Realtime API: 음성 인텔리전스 기능 추가
- 종류: API
- 무엇이 새로운지: 대화 중 **듣기/추론/번역/전사/액션**을 한 번에 다루는 음성 기능 세트 추가

- 핵심 기능 한 줄: 콜센터/교육/콘텐츠 등에서 ‘말로 일하는’ 인터페이스를 더 쉽게 구성

- 가격/라이선스: 기사 기준 **토큰 과금( GPT-Realtime-2 )**, **분 단위 과금(Translate/Whisper)** 언급

- 출처: <https://techcrunch.com/2026/05/07/openai-launches-new-voice-intelligence-features-in-its-api/>

### 마이너 업데이트
- (참고) 이번 24~48시간 내 신규 MCP 서버/국내 공공 API 급 업데이트는 크게 확인되지 않음. 오늘은 ‘메이저 2건 + 브레이킹 변경 1건’ 위주로 정리.

### 💡 CTO 메모 (Rails 8 B2B 영업 자동화, 옥상골프 SaaS, ERP/MES 관점)
- Rails 8 B2B 영업 자동화: MCP 서버(예: AWS MCP Server) 기반으로 **"권한/IAM"을 경계로 에이전트가 클라우드 리소스를 조작**하게 만들면, 영업/CS 자동화도 "데이터 소스 연결"을 넘어 "업무 실행"(예: 리포트 생성 → S3 업로드 → 링크 공유)까지 확장 가능.
- 옥상골프 SaaS: 음성 기반 Realtime API는 **현장(스크린골프/레슨) 운영자의 핸즈프리 입력/응대**에 유리. 예약 변경/환불/쿠폰 발급 같은 워크플로를 음성으로 트리거하고, 로그는 텍스트로 저장하는 형태가 MVP에 적합.
- ERP/MES: Gemini Interactions API의 `steps` 구조는 **툴 호출/검색/코드 실행 결과를 타임라인으로 남기는 설계**에 가깝다. 향후 사내 에이전트 플랫폼 구축 시, “대화 로그 = 감사 로그”가 되도록 이벤트/스텝 모델을 선제적으로 맞춰두면 마이그레이션 비용이 줄어듦.
