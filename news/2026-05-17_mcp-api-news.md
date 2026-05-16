## 🆕 오늘의 신간 (2026-05-17)

### MCP 서버 신간

오늘(어제~오늘 기준) 발표된 신규 MCP 서버/메이저 업데이트는 확인되지 않았습니다.

### AI/LLM API 신간

오늘(어제~오늘 기준) 공개된 대형 신규 API 릴리즈는 확인되지 않았습니다.

### 마이너 업데이트

- GitHub MCP Server: Secret scanning 기능이 GA(일반 제공)로 전환됨(기존 2026년 3월부터 프리뷰).  
  - 종류: MCP 서버  
  - 무엇이 새로운지: GA 전환 + 기존 Push Protection 커스터마이징을 그대로 반영(탐지/바이패스 동작 일관성).  
  - 핵심 기능: 커밋/PR 전에 코드 변경분에서 노출된 시크릿을 탐지.  
  - 가격/라이선스: 별도 가격 언급은 없으나, 리포지토리에 GitHub Secret Protection 필요(일부는 Advanced Security 플러그인과 연동).  
  - ⭐: ⭐ (GitHub 공식)  
  - 출처: https://github.blog/changelog/2026-05-05-secret-scanning-with-github-mcp-server-is-now-generally-available/

- ⭐ OpenAI: GPT-5.5 / GPT-5.5 Pro가 2026-04-24에 API 제공 시작(참고용; 오늘자 신간은 아님).  
  - 종류: API  
  - 무엇이 새로운지: 신규 모델군 + 1M 컨텍스트 + 에이전틱 작업 최적화.  
  - 핵심 기능: 계획/툴사용/검증을 포함한 멀티스텝 자동화에 강점.  
  - 가격/라이선스: gpt-5.5 입력 $5/1M tok, 출력 $30/1M tok; gpt-5.5-pro 입력 $30/1M, 출력 $180/1M(페이지 기재).  
  - ⭐: ⭐ (OpenAI 공식)  
  - 출처: https://openai.com/index/introducing-gpt-5-5/

### 💡 CTO 메모 (Rails 8 B2B 영업 자동화, 옥상골프 SaaS, ERP/MES 관점)

- Rails 8 B2B 영업 자동화: MCP/에이전트가 ‘쓰기(write)’ 권한을 가지는 순간(리드 생성/수정, 이메일 발송, CRM 업데이트)부터 감사를 위한 로깅·권한(least privilege)·승인흐름이 핵심입니다. Secret scanning 같은 보안 기능은 “초기 세팅 비용 대비 리스크 절감”이 커서 빠르게 기본값으로 넣는 게 유리합니다.
- 옥상골프 SaaS: 예약/결제/정기권/현장 키오스크 연동은 결국 외부 API 연동의 연속입니다. ‘오늘 신간 없음’ 같은 날이라도, MCP 서버의 변화(특히 보안/권한/감사)는 운영 리스크를 직접 줄이므로 릴리즈 노트를 정기적으로 점검하는 루틴을 추천합니다.
- ERP/MES: 현장 시스템은 네트워크/계정 권한이 보수적이어서, MCP 도입 시 “읽기 전용(조회)”부터 시작해 점진적으로 ‘승인된 쓰기’로 확장하는 방식이 안전합니다. GitHub Secret scanning GA 같은 변화는 개발/운영 경계에서 사고를 줄이는 데 바로 도움됩니다.
