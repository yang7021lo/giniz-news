## 오늘의 신간 (2026-05-19)

오늘은 최근 24~48시간 내(공식 변경로그/공식 발표 기준) MCP 서버 신간 및 AI/LLM API 신간에서 ‘메이저급’ 신규 출시/업데이트를 확인하지 못했습니다.

### MCP 서버 신간
- 오늘은 주요 신간 없음

### AI/LLM API 신간
- 오늘은 주요 신간 없음

### 마이너 업데이트
• OpenAI API: 2026-05-12 기준으로 DALL·E 스냅샷(dall-e-2, dall-e-3)과 Realtime API Beta가 deprecate 및 제거됨. 대체로 gpt-image-2 / gpt-image-1 계열 사용 권고. (종류: API, 업데이트) 출처: https://developers.openai.com/api/docs/changelog
• Gemini API: 2026-05-07 기준으로 gemini-3.1-flash-lite GA 릴리즈 및 preview 모델(gemini-3.1-flash-lite-preview) deprecate 일정 공지(5/11 deprecate 시작, 5/25 종료). (종류: API, 업데이트) 출처: https://ai.google.dev/gemini-api/docs/changelog

### CTO 메모 (Rails 8 B2B 영업 자동화, 옥상골프 SaaS, ERP/MES 관점)
- (영업 자동화) ‘신간이 없는 날’일수록, 기존 워크플로우에 MCP를 붙일 때 ROI가 바로 나오는 지점(리드 수집 → 리서치 → CRM 입력 → 후속메일)을 먼저 자동화하는 편이 좋습니다. Rails 8에서는 background job(예: Solid Queue) + webhook 수신(리드 폼/캘린더) + MCP tool로 “데이터 정합성 검사/중복 제거”를 넣으면 운영 품질이 올라갑니다.
- (옥상골프 SaaS) 결제/예약/출입(키오스크) 이벤트는 API 표준화가 잘 되어 있어, MCP 서버 신간보다 ‘기존 API 변경로그’ 모니터링이 더 중요합니다. 모델/에이전트는 바뀌어도, 이벤트 스키마 안정성이 제품 안정성을 좌우합니다.
- (ERP/MES) 현장 시스템은 릴리즈 빈도가 낮으니, AI API는 “모델 추가”보다 “deprecation/제한 변경”이 리스크 포인트입니다. 변경로그를 매일 체크하고, LLM 호출 계층에 모델명/엔드포인트를 추상화해두면 마이그레이션 비용이 급감합니다.
