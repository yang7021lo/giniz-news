## 🆕 오늘의 신간 (2026-05-23)

### MCP 서버 신간

1) Devart MCP Servers 제품 라인 출시
- 종류: MCP 서버
- 무엇이 새로운지: 기업 데이터/비즈니스 플랫폼 연결용 MCP 서버 제품군 신규 출시
- 핵심 기능 한 줄: DB·CRM·ERP 등 엔터프라이즈 데이터 소스를 MCP로 연결해 에이전트가 자연어로 질의/작업 가능
- 가격/라이선스: 미공개(공지 본문에 가격/라이선스 정보 없음)
- 비고: 기업용 제품 성격(온프레미스/보안 강조)
- 출처: Devart Blog https://www.devart.com/blog/devart-brings-ai-agents-closer-to-enterprise-data-with-new-mcp-server-product-line.html

2) MCP 2026-07-28 스펙 릴리즈 후보(Release Candidate) 공개
- 종류: MCP 서버/프로토콜(스펙)
- 무엇이 새로운지: 스펙 대규모 개정 RC 공개(2026 로드맵 반영)
- 핵심 기능 한 줄: Stateless 코어 + MCP Apps/Tasks 확장 + OAuth/OIDC 정렬형 인증 + 공식 deprecation 정책
- 가격/라이선스: 해당 없음(스펙 공지)
- ⭐: 공식 프로젝트 공지
- 출처: Model Context Protocol Blog https://blog.modelcontextprotocol.io

### AI/LLM API 신간

1) ⭐ Google Gemini Interactions API 스키마/이벤트/응답포맷 ‘브레이킹 체인지’ 마이그레이션 가이드
- 종류: API
- 무엇이 새로운지: `outputs` → `steps` 스키마 전환, `response_mime_type` 제거 및 `response_format`로 통합(브레이킹)
- 핵심 기능 한 줄: 상호작용을 ‘단계 타임라인(steps)’로 구조화해 mid-flight steering/비동기 툴콜 등 확장 대비
- 가격/라이선스: 기존 Gemini API 요금 체계(본문에 가격 변화 언급 없음)
- ⭐: Google 공식
- 주요 일정(가이드 기준): 5/7 옵트인, 5/26 REST 기본값 전환, 6/8 레거시 제거
- 출처: Google AI for Developers https://ai.google.dev/gemini-api/docs/interactions-breaking-changes-may-2026

### 마이너 업데이트
- (금일 24~48시간 범위 내) OpenAI/Anthropic 공식 변경 로그에서 ‘신규 출시/메이저 업데이트’로 확정 가능한 항목은 확인되지 않음(오늘 수집 결과 기준)

### 💡 CTO 메모 (Rails 8 B2B 영업 자동화, 옥상골프 SaaS, ERP/MES 관점)
- B2B 영업 자동화: Devart처럼 ‘데이터 소스별 커넥터(서버)’를 제품화하면, 초기에는 파이프라인/리포트 자동화(리드→견적→계약) 같은 반복 업무부터 빠르게 가치가 납니다. Rails 8에서는 백오피스 워크플로(승인/알림/로그)를 먼저 안정화하고, MCP 툴콜은 “조회→요약→초안 생성”처럼 안전한 읽기 중심 플로우로 시작하는 게 리스크가 낮습니다.
- 옥상골프 SaaS: 현장 운영 데이터(예약/레슨/락커/정산)를 자연어로 ‘바로 질의’하려면 DB 연결이 병목입니다. MCP 서버를 도입하면 관리자/CS가 SQL 없이도 “이번 주 취소율 상위 시간대” 같은 질문을 즉시 처리해 운영 효율이 올라갑니다.
- ERP/MES: MCP 스펙이 stateless로 가면(로드밸런싱/표준 HTTP 인프라 친화), 공장/현장망처럼 제약 환경에서도 운영이 쉬워집니다. 다만 인증/권한 모델(OAuth/OIDC 정렬)이 강화되는 흐름이라, ‘현장 단말/에이전트’ 권한 분리(조회/승인/실행) 설계가 핵심입니다.
