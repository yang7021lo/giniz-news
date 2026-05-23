## 🆕 오늘의 신간 (2026-05-24)

### MCP 서버 신간
- Splunk MCP Server for Splunk Platform 1.1.3
  - 종류: MCP 서버
  - 무엇이 새로운지: 마이너 업데이트(버그픽스)
  - 핵심 기능: Splunk Platform을 MCP 도구로 연결해 검색/운영 자동화를 지원
  - 가격/라이선스: Splunk 제품 정책에 따름(문서에 명시 없음)
  - 출처: Splunk MCP Server release notes (May 19, 2026) https://help.splunk.com/en/splunk-enterprise/mcp-server-for-splunk-platform/1.1/mcp-server-release-notes

### AI/LLM API 신간
- ⭐ Google Gemini CLI v0.43.0
  - 종류: API/SDK(개발자 도구)
  - 무엇이 새로운지: 신규 릴리즈
  - 핵심 기능: 세션 export/import, 호스트명 표시, subagent protocol 지원, OAuth/샌드박싱/도구처리 개선
  - 가격/라이선스: (Releasebot 요약에 명시 없음)
  - 출처: Releasebot Google updates (Gemini CLI v0.43.0, 2026-05-22) https://releasebot.io/updates/google

- ⭐ pkg.go.dev API 공개
  - 종류: API
  - 무엇이 새로운지: 신규 출시
  - 핵심 기능: Go 모듈/패키지 메타데이터(검색, 버전, 심볼, imports, 취약점)에 대한 GET-only 프로그램 접근 제공
  - 가격/라이선스: 무료(공개 API, 과금 언급 없음)
  - 출처: Releasebot Google updates (pkg.go.dev API, 2026-05-21) https://releasebot.io/updates/google

### 한국형/공공 API 신간 (있을 때만)
- 서울열린데이터광장: 2026-05-23 수정 데이터(예: 서울시 대부업체 정보 / 위생처리업 현황 / 기타 위생용품 제조업 현황)
  - 종류: 공공 데이터(오픈API/다운로드 데이터)
  - 무엇이 새로운지: 데이터 갱신(수정일자 기준)
  - 핵심 기능: 서울시 행정/사업체 현황 데이터 최신화
  - 가격/라이선스: 공공데이터 정책에 따름(페이지에 개별 항목 링크는 확인 불가)
  - 출처: 서울열린데이터광장 공공데이터 목록(수정일자 2026-05-23 표시) https://data.seoul.go.kr/dataList/datasetList.do

### 마이너 업데이트
- Google Antigravity 2.0.6
  - 종류: 개발자 플랫폼(에이전트 개발)
  - 무엇이 새로운지: IDE 통합 추가 및 개선
  - 핵심 기능: 에이전트/워크플로 개발 환경 통합 강화
  - 가격/라이선스: (Releasebot 요약에 명시 없음)
  - 출처: Releasebot Google updates (Antigravity 2.0.6, 2026-05-22) https://releasebot.io/updates/google

### 💡 CTO 메모 (Rails 8 B2B 영업 자동화, 옥상골프 SaaS, ERP/MES 관점)
- Rails 8 B2B 영업 자동화: Gemini CLI의 세션 export/import는 ‘리드 조사 → 요약 → 메일 초안 → CRM 업데이트’ 같은 에이전트 파이프라인을 재현/회고하기 좋습니다(세션을 아카이브해서 실패 케이스 재학습 루프에 투입).
- 옥상골프 SaaS: 패키지/버전/취약점 API(pkg.go.dev)는 결제/예약/IoT 연동 등 서비스가 커질수록 공급망 리스크 점검이 중요해지는데, 배포 파이프라인에서 의존성 상태를 자동 체크하는 데 유용합니다.
- ERP/MES: Splunk MCP 서버 버그픽스(커스텀 툴 생성 안정화)는 ‘로그/알람 → 원인분석 → 조치 실행’ 자동화에서 tool 정의/생성 단계가 막히는 리스크를 줄여, 운영 자동화의 신뢰도를 조금이라도 올려줍니다.
