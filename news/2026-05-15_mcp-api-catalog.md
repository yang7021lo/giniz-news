# MCP·AI API 전수 카탈로그 — 2026-05-15

> 현존하는 주요 MCP 서버와 AI/LLM API를 **기능별·용도별·가격별**로 정리한 카탈로그.
> ⭐ = 공식·공공·신뢰도 높은 제공자 (Anthropic·OpenAI·Google·Microsoft·AWS 등 대형사 또는 MCP 레퍼런스).
> 작성: 2026-05-15 KST. 신간 업데이트는 매일 아침 8시 [GitHub 레포](https://github.com/yang7021lo/giniz-news)에 자동 추가.

## 📑 목차

1. [MCP 서버 — Anthropic 공식 레퍼런스](#1-mcp-서버--anthropic-공식-레퍼런스)
2. [MCP 서버 — 대기업/공식 파트너](#2-mcp-서버--대기업공식-파트너)
3. [MCP 서버 — 개발자 도구](#3-mcp-서버--개발자-도구)
4. [MCP 서버 — 데이터베이스](#4-mcp-서버--데이터베이스)
5. [MCP 서버 — 생산성·협업](#5-mcp-서버--생산성협업)
6. [MCP 서버 — 검색·웹](#6-mcp-서버--검색웹)
7. [MCP 서버 — 클라우드·인프라](#7-mcp-서버--클라우드인프라)
8. [MCP 서버 — 디자인·크리에이티브](#8-mcp-서버--디자인크리에이티브)
9. [MCP 서버 — 결제·페이먼트](#9-mcp-서버--결제페이먼트)
10. [MCP 프레임워크·SDK (서버 빌드용)](#10-mcp-프레임워크sdk-서버-빌드용)
11. [MCP 관리·게이트웨이·레지스트리](#11-mcp-관리게이트웨이레지스트리)
12. [AI/LLM API — 텍스트 생성 (LLM)](#12-aillm-api--텍스트-생성-llm)
13. [AI/LLM API — 이미지 생성](#13-aillm-api--이미지-생성)
14. [AI/LLM API — 음성 (STT/TTS)](#14-aillm-api--음성-stttts)
15. [AI/LLM API — 임베딩·검색](#15-aillm-api--임베딩검색)
16. [AI/LLM API — 멀티모달·비전](#16-aillm-api--멀티모달비전)
17. [AI/LLM API — 영상 생성](#17-aillm-api--영상-생성)
18. [CTO 메모 — 한국 B2B SaaS 빌더 관점](#18-cto-메모--한국-b2b-saas-빌더-관점)
19. [🇰🇷 한국 공공 API (data.go.kr 외)](#19--한국-공공-api-datagokr-외)
20. [🇰🇷 한국 민간 API (대기업·SaaS)](#20--한국-민간-api-대기업saas)
21. [🇰🇷 한국 MCP 생태계](#21--한국-mcp-생태계)
22. [🏠 실생활 활용 MCP](#22--실생활-활용-mcp)
23. [🎯 실생활 시나리오별 MCP 조합 추천 (한국 기준)](#23--실생활-시나리오별-mcp-조합-추천-한국-기준)

---

## 1. MCP 서버 — Anthropic 공식 레퍼런스

> [github.com/modelcontextprotocol/servers](https://github.com/modelcontextprotocol/servers) 공식 레포의 **활성 레퍼런스**. 모두 **무료/오픈소스 (MIT)**.

| 이름 | 용도 | 비고 |
|---|---|---|
| ⭐ **Fetch** | 웹 콘텐츠 가져오기 → 마크다운 변환 | LLM이 URL 읽을 때 필수 |
| ⭐ **Filesystem** | 파일 시스템 안전 접근 (읽기/쓰기) | 권한 제어 가능 |
| ⭐ **Git** | 로컬 Git 저장소 조작 | 커밋·브랜치·로그 |
| ⭐ **Memory** | 지식그래프 기반 영속 메모리 | 대화 컨텍스트 유지 |
| ⭐ **Sequential Thinking** | 다단계 추론 (체인 오브 쏘트) | 복잡 문제 풀이 |
| ⭐ **Time** | 시간·타임존 변환 | 스케줄링·로그 |
| ⭐ **Everything** | 모든 MCP 기능 테스트 서버 | 학습·디버깅용 |

**아카이브된 레퍼런스** (서드파티에 이관됨): AWS KB Retrieval, Brave Search, EverArt, GitHub, GitLab, Google Drive, Google Maps, PostgreSQL, Puppeteer, Redis, Sentry, Slack, SQLite — 대부분 같은 이름의 서드파티 또는 공식 버전으로 대체.

---

## 2. MCP 서버 — 대기업/공식 파트너

| 이름 | 제공자 | 용도 | 가격 |
|---|---|---|---|
| ⭐ **GitHub Official** | GitHub/Microsoft | 레포·이슈·PR 관리 | 무료 (계정 필요) |
| ⭐ **Playwright** | Microsoft | 브라우저 자동화·E2E 테스트 | 무료 |
| ⭐ **Chrome DevTools** | Google | 크롬 직접 제어, 디버깅, 성능 분석 | 무료 |
| ⭐ **AWS Documentation** | AWS | AWS 공식 문서 검색·추천 | 무료 |
| ⭐ **AWS Labs** | AWS | DynamoDB, Bedrock, S3 등 AWS 서비스 | 종량 (AWS 요금) |
| ⭐ **Cloudflare** | Cloudflare | Workers·R2·D1·KV 관리 | freemium |
| ⭐ **Stripe** | Stripe | 결제·고객·인보이스 | 거래 수수료 |
| ⭐ **Notion** | Notion | 페이지·DB 읽기/쓰기 | 무료 (워크스페이스 필요) |
| ⭐ **Linear** | Linear | 이슈·프로젝트 관리 | freemium |
| ⭐ **Slack** | Salesforce/Zencoder 유지보수 | 메시지·채널 | freemium |
| ⭐ **Atlassian (Jira/Confluence)** | Atlassian Cloud | 이슈·문서 | freemium |
| ⭐ **Figma** | Figma | 디자인 파일·컴포넌트 읽기 | freemium |
| ⭐ **Sentry** | Sentry | 에러·이슈 검색 | freemium |
| ⭐ **Vercel** | Vercel | 배포·프로젝트 관리 | freemium |
| ⭐ **Supabase** | Supabase | DB·Auth·Storage | freemium |
| ⭐ **Brave Search** | Brave | 웹·로컬 검색 (privacy-first) | freemium (월 2000건 무료) |

---

## 3. MCP 서버 — 개발자 도구

| 이름 | 용도 | 제공자 | 가격 |
|---|---|---|---|
| **Storybook** | UI 컴포넌트 스토리 자동 생성 | 공식 (Storybook) | 무료 |
| **Searchcode** | 공개 Git 코드 검색·인덱스 | 공식 (searchcode) | 무료 |
| **Context7** | 라이브러리·프레임워크 최신 문서 | ⭐ Upstash | freemium |
| **Claude Flow** | 멀티에이전트 오케스트레이션 | 커뮤니티 (ruvnet) | 무료/OSS |
| **Context Mode** | 컨텍스트 소비 98% 절감 (SQLite 세션) | 커뮤니티 (mksglu) | 무료/OSS |
| **MCP CLI Client** | LLM ↔ MCP 도구 호출 CLI | 커뮤니티 | 무료 |
| **OpenMCP Client** | VSCode/Cursor/Trae용 MCP 디버거 | 커뮤니티 | 무료 |
| **codemirror-mcp** | CodeMirror에 MCP 리소스 멘션 | 커뮤니티 | 무료 |

---

## 4. MCP 서버 — 데이터베이스

| 이름 | 용도 | 가격 |
|---|---|---|
| ⭐ **PostgreSQL** (서드파티 공식) | 읽기 전용 DB 접근·스키마 검사 | 무료 |
| ⭐ **SQLite** (서드파티) | 로컬 SQLite·BI 쿼리 | 무료 |
| ⭐ **Redis** (서드파티) | Redis 키-밸류 스토어 | 무료 |
| **DuckDB** | DuckDB SQL 쿼리 (분석용) | 무료 |
| **MongoDB** | NoSQL 문서 조작 | 무료 |
| **MySQL** | MySQL 쿼리 | 무료 |
| **ClickHouse** | 컬럼형 분석 DB | 무료 |
| **Neo4j** | 그래프 DB | 무료 |
| **Pinecone** | 벡터 DB | freemium |
| **Qdrant** | 벡터 DB (OSS) | 무료/유료 |
| **Weaviate** | 벡터 DB (OSS) | 무료/유료 |

---

## 5. MCP 서버 — 생산성·협업

| 이름 | 용도 | 가격 |
|---|---|---|
| ⭐ **Google Drive** | 파일 검색·읽기 | 무료 (Google 계정) |
| ⭐ **Google Calendar** | 일정 CRUD | 무료 |
| ⭐ **Gmail** | 메일 검색·발송 | 무료 |
| ⭐ **Microsoft 365** | Outlook·OneDrive·Teams | freemium |
| **Office Word** | Word 문서 생성·편집 | 무료 (OSS) |
| **Office Excel** | Excel 시트 조작 | 무료 (OSS) |
| **Obsidian** | 노트 DB 검색·편집 | 무료 |
| **Todoist** | 할일 관리 | freemium |
| ⭐ **Asana** | 프로젝트 관리 | freemium |

---

## 6. MCP 서버 — 검색·웹

| 이름 | 용도 | 가격 |
|---|---|---|
| ⭐ **Brave Search** | privacy-first 웹·로컬 검색 | freemium |
| ⭐ **Tavily Search** | AI 에이전트용 검색 API | freemium ($0.005/쿼리) |
| ⭐ **Perplexity** | Perplexity 검색·답변 | freemium |
| **Firecrawl** | 웹사이트 → 마크다운 크롤링 | freemium ($16~/월) |
| **SerpAPI** | Google·Bing·Yandex SERP | $50~/월 |
| **Exa Search** | 임베딩 기반 시멘틱 웹 검색 | freemium |
| **DuckDuckGo** | 익명 웹 검색 | 무료 |

---

## 7. MCP 서버 — 클라우드·인프라

| 이름 | 용도 | 가격 |
|---|---|---|
| ⭐ **AWS Labs (전체)** | DynamoDB·S3·Bedrock·Lambda 등 | AWS 종량 |
| ⭐ **Cloudflare** | Workers·R2·D1·KV·Pages | freemium |
| ⭐ **Vercel** | 배포·로그·환경변수 | freemium |
| ⭐ **Railway** | 백엔드 호스팅·DB | freemium |
| ⭐ **Fly.io** | 글로벌 배포 | 종량 |
| ⭐ **Heroku** | PaaS | 유료 |
| **Kubernetes** | 클러스터 관리 | 무료 (OSS) |
| **Docker** | 컨테이너 조작 | 무료 |
| **Terraform** | IaC 플랜·apply | 무료 (OSS) |

---

## 8. MCP 서버 — 디자인·크리에이티브

| 이름 | 용도 | 가격 |
|---|---|---|
| ⭐ **Figma** | 디자인 파일 읽기·컴포넌트 추출 | freemium |
| ⭐ **Blender (Anthropic 후원)** | 3D 모델·렌더 자동화 | 무료 (OSS) |
| **Photoshop** | PS 액션·레이어 조작 | 유료 (Adobe) |
| **Canva** | 디자인 자동화 | freemium |
| **EverArt** | AI 이미지 생성 (다중 모델) | 유료 |

---

## 9. MCP 서버 — 결제·페이먼트

| 이름 | 용도 | 가격 |
|---|---|---|
| ⭐ **Stripe** | 결제·구독·인보이스 | 거래 수수료 (2.9%+30¢) |
| **PayMCP** | MCP 도구를 유료 엔드포인트로 만드는 데코레이터 | OSS + 거래 수수료 |
| **Toss Payments** (커뮤니티) | 토스 결제 연동 | 거래 수수료 |
| **Iamport** (커뮤니티) | 아임포트 통합결제 | 거래 수수료 |

---

## 10. MCP 프레임워크·SDK (서버 빌드용)

> 직접 MCP 서버를 만들 때 쓰는 SDK·프레임워크.

| 이름 | 언어 | 비고 |
|---|---|---|
| ⭐ **MCP TypeScript SDK** | TS/JS | 공식 |
| ⭐ **MCP Python SDK** | Python | 공식 |
| ⭐ **MCP Java SDK** | Java | 공식 |
| ⭐ **MCP C# SDK** | .NET | 공식 |
| ⭐ **MCP Ruby SDK** | Ruby | 공식 (Rails 8 빌더에 적합) |
| **FastMCP** | TypeScript | 빠른 서버 빌드 |
| **FastAPI → MCP** | Python | FastAPI 엔드포인트 자동 노출 (Tadata) |
| **MCP-Framework** | TS | CLI 포함 |
| **mxcp** | Python | YAML+SQL+Python, ETL·인증·모니터링 내장 |
| **MCP Plexus** | Python | 멀티테넌트·OAuth 2.1 |
| **Spring AI MCP** | Java | Spring Boot 자동 구성 |
| **Quarkus MCP** | Java | Quarkus 통합 |
| **Anubis MCP** | Elixir | 고성능, LiveView 스타일 |
| **mcp_sse** | Elixir | SSE 구현 |
| **Foxy Contexts** | Go | Golang MCP |
| **Foobara MCP Connector** | Ruby | Foobara 명령 노출 |
| **PHP MCP Server** | PHP | 코어 PHP 구현 |
| **R mcptools** | R | R 기반 MCP |
| **Perl SDK** | Perl | Perl 구현 |
| **SAP ABAP MCP SDK** | ABAP | S/4HANA·R/3 |
| **Vercel MCP Adapter** | TS | Next/Nuxt/Svelte 통합 |
| **AgentR Universal SDK** | Python | 자격증명 관리 내장 |
| **PayMCP** | Py/TS | 결제 데코레이터 |

---

## 11. MCP 관리·게이트웨이·레지스트리

| 이름 | 용도 | 가격 |
|---|---|---|
| ⭐ **Smithery** | MCP 서버 레지스트리 (가장 큰 디렉토리) | 무료 |
| ⭐ **PulseMCP** | 커뮤니티 허브+뉴스레터, API 제공 | 무료 |
| ⭐ **mcp.run** | 호스팅 레지스트리+컨트롤 플레인 | freemium |
| ⭐ **Lunar.dev MCPX** | 오픈소스 엔터프라이즈 컨트롤 플레인 | OSS+유료 지원 |
| **Klavis AI** | 오픈소스 MCP 인프라, Slack/Discord 클라이언트 | OSS |
| **Toolbase** | MCP 데스크톱 매니저 (몇 번 클릭으로 설치) | 무료 |
| **ToolHive** (Stacklok) | MCP 배포·관리 유틸 | OSS |
| **mcp-dockmaster** | Windows/Linux/macOS UI | OSS |
| **MCP Router** | Win/macOS 앱, 인증 처리 | 무료 |
| **MCP Linker** | Tauri 크로스 플랫폼 GUI | OSS |
| **mcp-manager** | Claude Desktop용 웹 UI | OSS |
| **mcp-get** | CLI 설치 도구 | OSS |
| **mcpm** | Homebrew 스타일 매니저 | OSS |
| **mcp-guardian** | MCP 프록시·제어 (EQTY Lab) | OSS |
| **MCPWatch** | 보안 취약점 스캐너 | OSS |
| **Webrix MCP Gateway** | 엔터프라이즈 SSO·RBAC·감사 | 유료 |
| **mcp.natoma.ai** | 호스팅 MCP 플랫폼 (Natoma Labs) | freemium |
| **OpenTools** | 오픈 레지스트리 | 무료 |
| **MCPRepository.com** | MCP 서버 인덱스 | 무료 |
| **MCPServers.com** | 큐레이션 디렉토리+설치 가이드 | 무료 |
| **MCP Hunt** | 트렌딩 MCP 실시간 추적 | 무료 |
| **MCPHub** | macOS/Windows GUI 데스크톱 (Jeamee) | OSS |
| **Awesome MCP Servers** (punkpeye, wong2, appcypher) | 큐레이션 리스트 | 무료 (GitHub) |

---

## 12. AI/LLM API — 텍스트 생성 (LLM)

| 이름 | 제공자 | 강점 | 가격 (입력/출력, 100만 토큰) |
|---|---|---|---|
| ⭐ **Claude Opus 4.7** | Anthropic | 코딩·복잡 추론·긴 컨텍스트 | $15 / $75 |
| ⭐ **Claude Sonnet 4** | Anthropic | 가성비, 에이전트 워크플로 | $3 / $15 |
| ⭐ **Claude Haiku 4** | Anthropic | 초고속·저비용 | $0.80 / $4 |
| ⭐ **GPT-5** | OpenAI | 종합 성능, 멀티모달 | $5 / $20 (추정) |
| ⭐ **GPT-4o** | OpenAI | 멀티모달·실시간 | $2.5 / $10 |
| ⭐ **GPT-4o mini** | OpenAI | 저비용 | $0.15 / $0.60 |
| ⭐ **Gemini 2.5 Pro** | Google | 200만 토큰 컨텍스트, 멀티모달 | $1.25 / $10 |
| ⭐ **Gemini 2.5 Flash** | Google | 초고속·대량 처리 | $0.075 / $0.30 |
| ⭐ **Mistral Large 2** | Mistral | 유럽산, 오픈소스 옵션 | $2 / $6 |
| **Mistral Small** | Mistral | 저비용 | $0.20 / $0.60 |
| **Llama 3.3 70B** | Meta (호스팅: Groq, Together) | OSS, 자체 호스팅 가능 | $0.59 / $0.79 (Groq) |
| **DeepSeek V3** | DeepSeek | OSS, 코딩 강점 | $0.14 / $0.28 |
| **DeepSeek R1** | DeepSeek | 추론 특화 OSS | $0.55 / $2.19 |
| **Qwen 2.5 Max** | Alibaba | OSS, 다국어 | $1.6 / $6.4 |
| ⭐ **Perplexity Sonar** | Perplexity | 웹 검색 통합 답변 | $1 / $1 + 검색비 |
| **xAI Grok 3** | xAI | 실시간 X 데이터 | $2 / $10 |
| **Cohere Command R+** | Cohere | RAG·다국어 | $2.5 / $10 |
| **HyperCLOVA X** | Naver | 한국어 특화 ⭐ (한국 빌더에 추천) | 별도 문의 |
| **A.X** | SK Telecom | 한국어 특화 | 별도 문의 |

---

## 13. AI/LLM API — 이미지 생성

| 이름 | 제공자 | 강점 | 가격 |
|---|---|---|---|
| ⭐ **DALL·E 3** | OpenAI | 텍스트 정확도, GPT 통합 | $0.04~0.12/장 |
| ⭐ **Imagen 3** | Google | 사실적·텍스트 렌더링 | $0.03~/장 |
| ⭐ **Midjourney API** | Midjourney | 예술성 최상 | $10~/월 구독 |
| **Stable Diffusion 3.5** | Stability AI | OSS, 자체 호스팅 가능 | freemium |
| **Flux Pro 1.1** | Black Forest Labs | 사진급 사실감 | $0.04~/장 |
| **Ideogram 2.0** | Ideogram | 텍스트가 들어간 이미지 | freemium |
| **Recraft V3** | Recraft | 벡터·로고 생성 | freemium |
| **Leonardo.ai** | Leonardo | 게임 에셋 | freemium |
| **Adobe Firefly** | Adobe | 상업적 안전, CC 통합 | 구독 |

---

## 14. AI/LLM API — 음성 (STT/TTS)

| 이름 | 종류 | 강점 | 가격 |
|---|---|---|---|
| ⭐ **OpenAI Whisper API** | STT | 다국어 정확도 | $0.006/분 |
| ⭐ **Deepgram Nova-3** | STT | 실시간·저지연 | $0.0043/분 |
| ⭐ **AssemblyAI Universal-2** | STT | 화자분리·감정 | $0.37~/시간 |
| **Google Speech-to-Text** | STT | 다국어 강점 | $0.016/분 |
| **Azure Speech** | STT/TTS | 엔터프라이즈 | 종량 |
| **Naver Clova Speech** ⭐ | STT (한국어) | 한국어 1위 | 종량 |
| ⭐ **ElevenLabs** | TTS | 자연스러운 음성·복제 | $5~/월 |
| ⭐ **OpenAI TTS** | TTS | 6종 음성 | $15/100만 자 |
| **PlayHT** | TTS | 800+ 음성 | freemium |
| **Resemble AI** | TTS·음성복제 | 실시간 | 종량 |

---

## 15. AI/LLM API — 임베딩·검색

| 이름 | 제공자 | 강점 | 가격 |
|---|---|---|---|
| ⭐ **OpenAI text-embedding-3-large** | OpenAI | 최고 성능 | $0.13/100만 토큰 |
| ⭐ **OpenAI text-embedding-3-small** | OpenAI | 가성비 | $0.02/100만 토큰 |
| ⭐ **Voyage AI** | Voyage (Anthropic 추천) | RAG 특화 | $0.10~/100만 토큰 |
| **Cohere Embed v3** | Cohere | 다국어 강점 | $0.10/100만 토큰 |
| **Jina Embeddings v3** | Jina | OSS+API | freemium |
| **BGE-M3** | BAAI | OSS, 다국어 | 무료 (셀프호스팅) |

---

## 16. AI/LLM API — 멀티모달·비전

| 이름 | 용도 | 가격 |
|---|---|---|
| ⭐ **GPT-4o Vision** | 이미지 이해·OCR | 텍스트 가격 동일 |
| ⭐ **Claude (모든 모델)** | 이미지·차트·문서 이해 | 텍스트 가격 동일 |
| ⭐ **Gemini Vision** | 이미지·영상 이해 | 텍스트 가격 동일 |
| **AWS Rekognition** | 객체·얼굴·검열 | 종량 |
| **Google Vision API** | OCR·라벨링 | 종량 |
| **Azure Computer Vision** | OCR·분석 | 종량 |
| **Naver Clova OCR** ⭐ | 한국어 OCR 1위 | 종량 |

---

## 17. AI/LLM API — 영상 생성

| 이름 | 제공자 | 강점 | 가격 |
|---|---|---|---|
| ⭐ **Sora** | OpenAI | 최고 품질, 긴 클립 | $20~/월 구독 |
| ⭐ **Veo 3** | Google | 사운드 동시 생성 | API 베타 |
| ⭐ **Runway Gen-3** | Runway | 프로 영상 편집 | $12~/월 |
| **Luma Dream Machine** | Luma | 빠른 생성 | freemium |
| **Kling 2.0** | Kuaishou | 가성비 | freemium |
| **Pika 2.0** | Pika | 짧은 클립 특화 | freemium |
| **Hailuo (MiniMax)** | MiniMax | 중국발 강자 | freemium |

---

## 18. CTO 메모 — 한국 B2B SaaS 빌더 관점

> Rails 8 영업 자동화 / 옥상골프 SaaS / ERP·MES 제조업 솔루션 관점에서 우선순위.

### 즉시 도입 검토 (오늘이라도)
- **MCP Ruby SDK** ⭐ — Rails 8 영업 자동화 플랫폼에 MCP 서버 직접 노출 → Claude/GPT/Perplexity 어디서든 동일 도구 호출, **벤더 락인 회피**
- **Stripe MCP + PayMCP** — 결제 워크플로우를 LLM이 직접 실행
- **Playwright MCP** ⭐ — 영업 데모 자동화·웹 스크래핑(현재 작업 중인 도메인과 직결)
- **HyperCLOVA X / Naver Clova OCR** ⭐ — 한국어 처리·한국어 문서 OCR이 필요한 ERP/MES에 필수
- **Context7 MCP** — Rails 8·HTMX·FastAPI 최신 문서를 LLM이 항상 정확히 참조

### B2B 기회 (직접 만들 만한 신규 SaaS)
1. **한국형 MCP 게이트웨이** ⭐ — Webrix·Lunar.dev의 한국판 (SSO·RBAC·감사·한글 UI). 시장 공백 큼
2. **제조업용 MCP 번들** — 도어·금속창호 ERP/MES에 ERP·CAD·공정·재고 MCP 묶음 제공
3. **영업 자동화 MCP 마켓플레이스** — 영업 페르소나별 MCP 도구 큐레이션
4. **MCP Shadow IT 거버넌스** — 한국 기업의 MCP 도입 거버넌스 (Qualys 한국판)

### 조심해야 할 것
- **MCP Shadow IT 리스크** — 사내 도입 시 권한·감사 필수 (Qualys 보고서 참고)
- **가격 변동성** — LLM API 가격은 분기마다 바뀜. 추상화 레이어 필수
- **한국어 모델 선택** — 영어권 모델만 쓰면 한국어 도메인 성능 떨어짐. HyperCLOVA X·A.X 혼합 운용 고려

---


---

## 19. 🇰🇷 한국 공공 API (data.go.kr 외)

> 모두 **공식 정부/공공기관 제공, 대부분 무료** (트래픽 제한 있음). ⭐는 활용량 최상위.
> 공통: [공공데이터포털 data.go.kr](https://www.data.go.kr)에서 인증키 신청.

### 부동산·국토
| 이름 | 제공처 | 용도 | 가격 |
|---|---|---|---|
| ⭐ **국토교통부 아파트 매매 실거래가** | 국토교통부 | 아파트 매매가 조회 | 무료 |
| ⭐ **아파트 전월세 실거래가** | 국토교통부 | 전월세 시세 | 무료 |
| **상업업무용 부동산 실거래가** | 국토교통부 | 상가·오피스 거래 | 무료 |
| **건축물대장 정보** | 국토교통부 | 건축물 면적·용도 | 무료 |
| **공시지가** | 국토교통부 | 토지·주택 공시가 | 무료 |
| **부동산 종합정보** | 한국부동산원 | 시세·통계 | 무료 |

### 사업자·기업
| 이름 | 제공처 | 용도 |
|---|---|---|
| ⭐ **사업자등록 진위확인** | 국세청 | 사업자번호 유효성 검증 (B2B 필수) |
| ⭐ **사업자등록 상태조회** | 국세청 | 휴·폐업 여부 |
| **법인 기본정보** | 대법원 | 등기 기본 정보 |
| **나라장터 입찰공고** | 조달청 | 공공조달 입찰 |

### 기상·환경
| 이름 | 제공처 | 용도 |
|---|---|---|
| ⭐ **기상청 동네예보·중기예보** | 기상청 | 단·중기 날씨 |
| ⭐ **기상청 초단기실황** | 기상청 | 실시간 1km 격자 |
| **기상청 지진정보** | 기상청 | 지진 통보 |
| ⭐ **에어코리아 대기오염 정보** | 환경부 | 미세먼지·오존 |
| **수질·수문** | 환경부/한강홍수통제소 | 강수·하천 수위 |

### 교통·이동
| 이름 | 제공처 | 용도 |
|---|---|---|
| ⭐ **국가대중교통정보 (TAGO)** | 국토교통부 | 버스·지하철·기차 통합 |
| ⭐ **버스도착정보** | 서울/지자체 | 실시간 버스 도착 |
| ⭐ **지하철 실시간 도착** | 서울교통공사 | 실시간 도착·혼잡도 |
| **고속도로 교통정보** | 한국도로공사 | 실시간 정체·CCTV |
| **택시 호출** | 국토부 (계획) | 호출 인터페이스 |
| **항공편 운항정보** | 공항공사 | 출도착·지연 |
| **KTX·SRT 운임·시간표** | 코레일·SR | 조회 (예매는 별도) |

### 의료·복지
| 이름 | 제공처 | 용도 |
|---|---|---|
| ⭐ **건강보험심사평가원 (HIRA)** | 심평원 | 병원·약국 검색, 진료비, 약가 |
| **국민건강보험공단** | 건보공단 | 건강검진·요양기관 |
| **식약처 의약품/식품 정보** | 식약처 | 의약품·식품 안전 |
| **코로나·감염병 정보** | 질병관리청 | 발생 통계 |
| **복지로 복지서비스** | 보건복지부 | 복지 지원금·서비스 검색 |

### 행정·시민
| 이름 | 제공처 | 용도 |
|---|---|---|
| ⭐ **도로명주소 검색** | 행정안전부 | 주소 정규화 (필수) |
| **우편번호 조회** | 우정사업본부 | 우편번호 |
| **공공기관 채용정보** | 인사혁신처 | 공무원·공공기관 채용 |
| **국가법령정보** | 법제처 | 법령·조례·판례 |
| **민원24** | 행정안전부 | 민원 신청 정보 |

### 경제·금융
| 이름 | 제공처 | 용도 |
|---|---|---|
| ⭐ **한국은행 ECOS 경제통계** | 한국은행 | 환율·금리·통화량 |
| ⭐ **금융감독원 DART** | 금감원 | 공시·재무제표 |
| **KRX 주식 시세** | 한국거래소 | 종목·시세·지수 |
| **국세청 환율** | 국세청 | 관세 적용 환율 |
| **수출입 무역통계** | 관세청 | 무역 통계 (대체 서비스로 일부 이관) |

### 관광·문화
| 이름 | 제공처 | 용도 |
|---|---|---|
| **한국관광공사 TourAPI** | 관광공사 | 관광지·축제·숙박 |
| **문화체육관광부 공연전시** | 문체부 | 공연·전시 정보 |
| **국립국어원 표준국어대사전** | 국립국어원 | 사전 |

---

## 20. 🇰🇷 한국 민간 API (대기업·SaaS)

### 카카오
| 이름 | 용도 | 가격 |
|---|---|---|
| ⭐ **카카오맵** | 지도·길찾기·장소검색 | 일일 무료 한도 |
| ⭐ **카카오 로그인 (KOE)** | OAuth 소셜 로그인 | 무료 |
| ⭐ **카카오톡 메시지** | 알림톡·친구톡·나에게 보내기 | 메시지 단가 |
| ⭐ **카카오페이** | 결제·정기결제·송금 | 거래 수수료 |
| ⭐ **카카오모빌리티** | 카카오T 호출·내비게이션 | 종량 |
| **카카오 비즈니스 API** | 비즈채널·상담톡 | 종량 |
| **카카오 i (AI)** | 음성·번역·OCR | 종량 |

### 네이버
| 이름 | 용도 | 가격 |
|---|---|---|
| ⭐ **네이버 지도 API v3** | 지도·지오코딩·길찾기 | 일일 무료 한도 |
| ⭐ **네이버 검색 API** | 블로그·뉴스·쇼핑 검색 | 무료 (일 25,000건) |
| ⭐ **네이버 로그인** | OAuth | 무료 |
| ⭐ **NAVER Cloud Platform** | 클라우드 전체 | freemium |
| ⭐ **Clova Speech (STT)** | 한국어 STT 1위 | 종량 |
| ⭐ **Clova OCR** | 한국어 OCR 1위 (영수증·신분증·문서) | 종량 |
| ⭐ **Clova Voice (TTS)** | 자연 음성 합성 | 종량 |
| ⭐ **HyperCLOVA X / HyperCLOVA HCX** | 한국어 LLM | 별도 |
| **Papago 번역** | 한↔영·한↔일·한↔중 | 종량 |
| **CLOVA Studio** | 한국어 임베딩·도구 | 종량 |
| ⭐ **네이버 스마트스토어 API** | 주문·상품·정산 | 무료 (판매자) |
| **네이버 광고 API** | 광고 운영 자동화 | 무료 (광고주) |

### 결제·금융
| 이름 | 용도 | 가격 |
|---|---|---|
| ⭐ **토스페이먼츠** | PG 결제 (카드·간편·계좌) | 2.5~3.3% |
| ⭐ **토스페이** | 토스 간편결제 | 거래 수수료 |
| ⭐ **카카오페이 결제** | PG·간편결제 | 거래 수수료 |
| ⭐ **네이버페이 결제** | PG·포인트 | 거래 수수료 |
| **아임포트 (포트원)** | 멀티PG 통합 (15개+) | freemium |
| **NICE페이먼츠** | PG 결제 | 거래 수수료 |
| **KG이니시스** | PG 결제 | 거래 수수료 |
| **다날** | 휴대폰·카드 결제 | 거래 수수료 |
| ⭐ **금융결제원 오픈뱅킹** | 입출금·잔액·송금 (전 은행) | 무료 (이용기관 등록) |
| **신한·KB·우리·하나은행 OpenAPI** | 은행별 직접 연동 | 무료/협의 |
| ⭐ **쿠콘 (Coocon)** | 스크래핑 기반 금융·공공 데이터 통합 | 유료 |
| **하이픈 (hyphen.im)** | 배달앱·이커머스 스크래핑 API | 유료 |

### 커머스·생활
| 이름 | 용도 | 가격 |
|---|---|---|
| ⭐ **쿠팡 파트너스 API** | 제휴 마케팅·상품 검색 | 무료 |
| **쿠팡 윙 (셀러)** | 주문·재고·정산 | 무료 (판매자) |
| **11번가 셀러 API** | 주문·상품 관리 | 무료 |
| **G마켓·옥션 ESM** | 주문·상품 | 무료 |
| **카페24 API** | 쇼핑몰 운영 자동화 | freemium |
| **NHN커머스 (고도몰)** | 쇼핑몰 운영 | freemium |
| **배달의민족 (하이픈 경유)** | 매출·정산·리뷰 | 유료 (스크래핑) |
| **요기요 (스크래핑 API)** | 매출·주문 | 유료 |
| **당근 비즈프로필** | 동네 비즈 운영 | 무료 |
| **야놀자/여기어때 (제휴)** | 숙박 (B2B 제휴 필요) | 협의 |

### 통신·메시징
| 이름 | 용도 | 가격 |
|---|---|---|
| ⭐ **NHN Toast/Cloud SMS, 알림톡** | SMS·LMS·카톡 알림 | 건당 |
| ⭐ **SOLAPI (구 쿨에스엠에스)** | SMS·카톡·이메일 통합 | 건당 |
| **세종텔레콤·LG유플러스 알림톡** | 카톡 알림톡 | 건당 |
| **NICE평가정보 본인인증** | 휴대폰·아이핀 본인인증 | 건당 |
| **KCB 본인인증** | 본인인증 | 건당 |

### 모빌리티
| 이름 | 용도 | 가격 |
|---|---|---|
| ⭐ **카카오T API (카카오모빌리티)** | 택시·대리·주차 호출 | 종량 |
| **TMAP API** | 내비게이션·POI·물류 | freemium |
| **쏘카 / 그린카** | 카셰어링 (B2B 제휴) | 협의 |

---

## 21. 🇰🇷 한국 MCP 생태계

> 한국 MCP 서버는 아직 초기 단계. 대부분 커뮤니티가 만든 비공식 래퍼.

| 이름 | 카테고리 | 가격 | 비고 |
|---|---|---|---|
| **kakao-map-mcp** (커뮤니티) | 지도 | 무료 | 카카오맵 API 래퍼 |
| **naver-search-mcp** (커뮤니티) | 검색 | 무료 | 네이버 검색 API 래퍼 |
| **naver-map-mcp** (커뮤니티) | 지도 | 무료 | 네이버 지도 v3 |
| **kma-weather-mcp** (커뮤니티) | 날씨 | 무료 | 기상청 동네예보 |
| **data-go-kr-mcp** (커뮤니티) | 공공 | 무료 | 공공데이터포털 범용 래퍼 |
| **dart-mcp** (커뮤니티) | 금융 | 무료 | DART 공시 검색 |
| **ecos-mcp** (커뮤니티) | 경제 | 무료 | 한국은행 ECOS |
| **roadname-address-mcp** | 주소 | 무료 | 도로명주소 정규화 |
| **toss-payments-mcp** | 결제 | OSS | 토스페이먼츠 래퍼 |
| **iamport-mcp** (커뮤니티) | 결제 | OSS | 포트원 통합 |
| **clova-ocr-mcp** | OCR | 종량 | 네이버 클로바 OCR |
| **papago-mcp** | 번역 | 종량 | 파파고 |
| **coupang-partners-mcp** | 커머스 | 무료 | 쿠팡 파트너스 |
| **kakao-talk-bot-mcp** | 메시징 | OSS | 카카오톡 알림톡 |

> *⚠️ 한국형 MCP는 공식 제공자가 거의 없음 → **B2B 기회**. 정식 SDK·게이트웨이 부재.*

---

## 22. 🏠 실생활 활용 MCP

### 스마트홈·IoT
| 이름 | 용도 | 가격 |
|---|---|---|
| ⭐ **Home Assistant MCP** | 조명·온도·보안·가전 통합 제어 | 무료 (OSS) |
| **SmartThings MCP** (커뮤니티) | 삼성 SmartThings 가전 | 무료 |
| **Philips Hue MCP** | 조명 제어 | 무료 |
| **Matter/Thread MCP** | 표준 IoT 프로토콜 | 무료 |
| **Tuya MCP** | 중국발 IoT 브랜드 통합 | 무료 |

### 일정·생산성
| 이름 | 용도 | 가격 |
|---|---|---|
| ⭐ **Google Calendar MCP** | 일정 CRUD·회의 예약 | 무료 |
| ⭐ **Apple Calendar (CalDAV) MCP** | 맥/아이폰 캘린더 | 무료 |
| ⭐ **Outlook Calendar MCP** | MS 365 캘린더 | freemium |
| **Reminders.app MCP** | 애플 미리알림 | 무료 |
| **Todoist MCP / TickTick MCP** | 할일 관리 | freemium |
| **Cal.com MCP** | 미팅 예약 자동화 | freemium |

### 메일·메시지
| 이름 | 용도 | 가격 |
|---|---|---|
| ⭐ **Gmail MCP** | 메일 검색·발송·필터 | 무료 |
| ⭐ **Outlook MCP** | MS 메일 | freemium |
| ⭐ **Apple Mail (IMAP) MCP** | 범용 IMAP | 무료 |
| **WhatsApp MCP** (커뮤니티) | 왓츠앱 메시지 | 무료 |
| **Telegram MCP** | 텔레그램 봇 | 무료 |
| **Discord MCP** | 디스코드 | 무료 |
| **iMessage MCP** (Mac) | 아이메시지 | 무료 |

### 날씨
| 이름 | 용도 | 가격 |
|---|---|---|
| ⭐ **OpenWeatherMap MCP** | 전 세계 날씨 | freemium |
| ⭐ **Athenium Weather MCP** | 대화형 날씨 인텔리전스 | freemium |
| **AccuWeather MCP** | 상세 예보 | freemium |
| ⭐ **기상청 동네예보 MCP** | 한국 단·중기 예보 | 무료 |

### 지도·내비게이션
| 이름 | 용도 | 가격 |
|---|---|---|
| ⭐ **Google Maps MCP** | 지도·길찾기·POI | freemium |
| ⭐ **카카오맵 MCP** | 한국 지도 | freemium |
| ⭐ **네이버 지도 MCP** | 한국 지도 | freemium |
| **TMAP MCP** | 한국 내비 | freemium |
| **Apple Maps MCP** | 애플 지도 | 무료 |
| **OpenStreetMap MCP** | OSS 지도 | 무료 |

### 쇼핑·이커머스
| 이름 | 용도 | 가격 |
|---|---|---|
| ⭐ **Amazon MCP** (커뮤니티) | 상품·가격 검색 | 무료 |
| ⭐ **쿠팡 MCP** (커뮤니티) | 상품·가격·리뷰 | 무료 |
| **Shopify MCP** | 쇼피파이 스토어 운영 | freemium |
| **eBay MCP** | 이베이 검색·구매 | freemium |
| **AliExpress MCP** | 알리 상품 | 무료 |

### 음식·배달
| 이름 | 용도 | 가격 |
|---|---|---|
| **Yelp MCP** | 식당 검색·리뷰 (해외) | freemium |
| **OpenTable MCP** | 식당 예약 | freemium |
| **카탈로그 미정** | 한국 배달앱(배민·요기요)은 공식 MCP 부재 | — |
| ⭐ **레시피 검색 MCP** (Spoonacular 등) | 레시피·영양 | freemium |

### 여행·이동
| 이름 | 용도 | 가격 |
|---|---|---|
| ⭐ **Travel MCP Server** | 항공·숙박·환율·날씨 통합 | freemium |
| **Skyscanner MCP** | 항공권 검색 | freemium |
| **Booking.com MCP** | 숙박 검색 | freemium |
| **Airbnb MCP** (커뮤니티) | 숙박 | 무료 |
| **Uber MCP** | 우버 호출 | freemium |
| **Google Flights MCP** | 항공권 | freemium |

### 건강·피트니스
| 이름 | 용도 | 가격 |
|---|---|---|
| ⭐ **Apple Health MCP** | 활동·심박·수면 데이터 | 무료 (OSS) |
| **Google Fit MCP** | 구글 핏 | 무료 |
| **Garmin Connect MCP** | 가민 워치 데이터 | 무료 |
| **Fitbit MCP** | 핏빗 | 무료 |
| **Strava MCP** | 러닝·사이클 | freemium |
| **MyFitnessPal MCP** (커뮤니티) | 식단 기록 | freemium |
| **Withings MCP** | 체중·혈압 | freemium |

### 미디어·엔터테인먼트
| 이름 | 용도 | 가격 |
|---|---|---|
| ⭐ **YouTube MCP** | 영상 검색·자막·요약 | 무료 |
| ⭐ **YouTube Music MCP** | 음악 검색·재생 | 무료 |
| ⭐ **Spotify MCP** | 플레이리스트·재생 | freemium |
| **Apple Music MCP** | 애플 뮤직 | 구독 |
| **Netflix MCP** (비공식) | 시청 기록 | — |
| **Plex/Jellyfin MCP** | 미디어 서버 | 무료 |
| **IMDb MCP** | 영화·드라마 정보 | freemium |

### 뉴스·정보
| 이름 | 용도 | 가격 |
|---|---|---|
| ⭐ **RSS Reader MCP** | 모든 RSS 피드 | 무료 (npm) |
| **NewsAPI MCP** | 글로벌 뉴스 검색 | freemium |
| **Hacker News MCP** | HN 상위 | 무료 |
| **Reddit MCP** | 서브레딧·댓글 | 무료 |
| ⭐ **네이버 뉴스 MCP** (커뮤니티) | 한국 뉴스 | 무료 |

### 금융·가계부
| 이름 | 용도 | 가격 |
|---|---|---|
| ⭐ **Plaid MCP** | 미국·캐나다 은행 통합 | freemium |
| **YNAB MCP** | 가계부 (You Need A Budget) | 구독 |
| ⭐ **오픈뱅킹 MCP** (커뮤니티) | 한국 전 은행 계좌·거래 | 무료 (이용기관) |
| **토스 가계부 MCP** (커뮤니티) | 토스 자산·소비 | 비공식 |

### 보안·인증
| 이름 | 용도 | 가격 |
|---|---|---|
| ⭐ **1Password MCP** | 비밀번호·시크릿 | 구독 |
| **Bitwarden MCP** | 오픈소스 비번 매니저 | freemium |
| **Authy MCP** (커뮤니티) | TOTP 2FA | 무료 |

---

## 23. 🎯 실생활 시나리오별 MCP 조합 추천 (한국 기준)

### "출근 준비" 시나리오
- 기상청 동네예보 MCP (오늘 날씨)
- 카카오맵 MCP (출근 경로·교통 상황)
- Google Calendar MCP (오늘 일정)
- Gmail MCP (밤사이 메일 요약)
- 네이버 뉴스 MCP (관심 분야 헤드라인)

### "식당 정하기" 시나리오
- 카카오맵 MCP (주변 식당)
- 네이버 검색 MCP (블로그 리뷰)
- 카카오톡 MCP (친구에게 추천 전송)

### "가계부 자동화" 시나리오
- 오픈뱅킹 MCP (계좌 거래 내역)
- Clova OCR MCP (영수증 자동 입력)
- Google Sheets MCP (가계부 시트 누적)

### "B2B 영업 자동화" 시나리오 (CTO 본업)
- 국세청 사업자등록 진위확인 MCP (리드 검증)
- DART 공시 MCP (재무 상태)
- 카카오톡 알림톡 MCP (영업 메시지)
- HubSpot/Salesforce MCP (CRM 기록)
- Slack MCP (내부 공유)

### "옥상골프 SaaS" 시나리오 (사이드 프로젝트)
- 기상청 MCP (영업일·강수)
- 카카오맵 MCP (위치·길찾기)
- 토스페이먼츠 MCP (예약 결제)
- 카카오톡 알림톡 MCP (예약 안내)
- Google Calendar MCP (예약 일정)

## 📌 출처

- [modelcontextprotocol/servers (GitHub 공식)](https://github.com/modelcontextprotocol/servers)
- [PulseMCP 서버 디렉토리](https://www.pulsemcp.com/servers)
- [Smithery 레지스트리](https://smithery.ai)
- [Anthropic Newsroom](https://www.anthropic.com/news)
- [Firecrawl - 2026 베스트 MCP 서버](https://www.firecrawl.dev/blog/best-mcp-servers-for-developers)
- [Obot.ai - 엔터프라이즈 MCP 게이트웨이 13선](https://obot.ai/blog/the-13-best-mcp-gateways-for-enterprise-teams/)
- [Qualys - MCP Shadow IT 분석](https://blog.qualys.com/product-tech/2026/03/19/mcp-servers-shadow-it-ai-qualys-totalai-2026)
- 각 제공자 공식 가격 페이지 (Anthropic, OpenAI, Google, Mistral, DeepSeek, ElevenLabs, Deepgram 등 — 2026-05 기준)

---

*이 카탈로그는 신간이 나올 때마다 매일 아침 8시 KST에 자동 업데이트됩니다.*
*가격은 2026년 5월 기준이며 변동 가능. 도입 전 공식 페이지에서 재확인 필요.*
