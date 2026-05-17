## 🆕 오늘의 신간 (2026-05-18)

오늘(최근 24~48시간) 기준, MCP 서버 ‘신규 출시’ 수준의 확실한 신간은 확인되지 않았습니다.
대신, CTO 관점에서 바로 영향이 있는 API/플랫폼 변경(최근 1주 내)을 마이너 업데이트로 정리합니다.

### MCP 서버 신간
- 오늘 확인된 주요 신간 없음

### AI/LLM API 신간
- 오늘 확인된 주요 신간 없음

### 마이너 업데이트
1) OpenAI API: DALL·E 스냅샷 및 Realtime API Beta 제거(파괴적 변경)
- 종류: API
- 무엇이 새로운지: 모델 스냅샷(dall-e-2, dall-e-3) 및 Realtime API Beta 디프리케이트/삭제(2026-05-12)
- 핵심 기능 한 줄: 이미지 생성은 gpt-image-* 계열로 마이그레이션 필요, 실시간은 정식 Realtime API로 이전 필요
- 가격/라이선스: 유료(사용량 기반, 상세는 OpenAI 정책 따름)
- 출처: https://developers.openai.com/api/docs/changelog

2) OpenAI API: Responses API 웹 검색 도구에 return_token_budget 추가
- 종류: API
- 무엇이 새로운지: web search tool에 return_token_budget 파라미터 추가(2026-05-11)
- 핵심 기능 한 줄: 리서치/평가 워크로드에서 더 긴 추론(토큰 예산) 탐색을 옵션으로 허용
- 가격/라이선스: 유료(사용량 기반)
- 출처: https://developers.openai.com/api/docs/changelog

3) Gemini API: gemini-3.1-flash-lite GA + preview 디프리케이션 일정 공지
- 종류: API
- 무엇이 새로운지: gemini-3.1-flash-lite GA(2026-05-07), preview 모델 5/25 종료 예정 공지
- 핵심 기능 한 줄: 초저비용/고속 추론 라인업 정식 릴리즈로 대량 트래픽 워크로드에 바로 적용 가능
- 가격/라이선스: 유료(사용량 기반)
- ⭐ 출처: https://ai.google.dev/gemini-api/docs/changelog

4) Gemini API: Webhooks 지원(이벤트 기반) 출시
- 종류: API
- 무엇이 새로운지: Batch API/장기 작업에 대해 폴링 대체하는 Webhooks 지원(2026-05-04)
- 핵심 기능 한 줄: 비동기 추론/배치 처리 결과를 이벤트로 받아 운영 부담을 낮춤
- 가격/라이선스: 유료(사용량 기반)
- ⭐ 출처: https://ai.google.dev/gemini-api/docs/changelog

### 💡 CTO 메모 (Rails 8 B2B 영업 자동화, 옥상골프 SaaS, ERP/MES 관점)
- (영업 자동화) OpenAI DALL·E/Realtime Beta 제거처럼 ‘API 디프리케이션’은 영업 자동화 파이프라인의 장애로 바로 이어집니다. 이미지/실시간 기능을 쓰는 경우, SDK 버전 고정 + 디프리케이션 모니터링(주 1회) + 대체 모델 핫스왑 플래그를 기본으로 두세요.
- (옥상골프 SaaS) Gemini Webhooks는 “예약/결제/센서 데이터 → AI 분석/요약” 같은 비동기 작업에 적합합니다. 폴링 제거로 비용/지연을 줄이고, 장애 시 재시도 큐(예: Sidekiq)와 결합하면 운영 난이도가 내려갑니다.
- (ERP/MES) 플래시-라이트 계열(GA)은 MES 현장 단말/키오스크 등 비용 민감 구간에 ‘모델 티어링(고급=Opus/Pro, 대량=Flash-lite)’ 전략을 가능하게 합니다. 업무 분류(검수/요약/이상탐지)별로 모델을 고정하지 말고 라우팅 규칙으로 관리하세요.
