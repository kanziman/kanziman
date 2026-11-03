# 황경태 | Backend Engineer

### 업무를 AI로 바꾸고, 통제 가능한 제품으로 만드는 엔지니어

글로벌 5개 리전 콘텐츠 플랫폼과 일 100만 건 금융 데이터 인프라를 개발·운영했습니다. 백엔드 경험을 바탕으로 **반복 업무를 AI로 자동화하고, 사람이 검토하고 승인할 수 있는 흐름까지 설계**합니다.

[포트폴리오](https://brand-design-one.vercel.app/portfolio.html) · [이력서](https://brand-design-one.vercel.app/resume.html) · [이메일](mailto:hwanghkt@naver.com)

## 집중하는 영역

**업무의 AI 전환**  
EV 충전 데이터의 월별 변경 검증을 AI 에이전트로 자동화해 **2~3시간 걸리던 작업을 30분으로 단축**했습니다. 중요 판단은 사람이 승인하도록 구성했습니다. 사양서 기반 챗봇 개발 경험을 바탕으로 위키 검색 시스템을 제안해 사내 플랫폼에 도입했습니다.

**제품의 AI 통제**  
개인 프로젝트 **NexusWiki**에서 **흐름·비용·품질·위험**의 네 측면으로 AI를 통제했습니다. 요청 추적과 Langfuse 관측으로 처리 과정을 확인하고, 토큰 예산과 비용 예약·정산으로 사용량을 관리했습니다. 답변은 검증 후 필요하면 수리하고, 중요 문서 변경은 사람의 승인을 거치도록 구현했습니다.

**AI 에이전트 협업**  
요구사항과 설계를 명세로 정하고, 독립적으로 검증 가능한 기능 단위로 작업을 나눴습니다. 병합 전에는 명세 일치 여부와 권한·데이터 접근을 검증하도록 구성했습니다. 이 과정에서 인증 없이 다른 워크스페이스에 비용을 기록할 수 있던 권한 결함을 발견하고 수정했습니다.

## 대표 프로젝트

### [NexusWiki](https://github.com/kanziman/NexusWiki)
**원문·위키 이중 인용 검색에 답변 검증·비용 정산·변경 승인을 구현한 개인 프로젝트**

- 4채널 하이브리드 검색과 RRF로 원문·위키를 함께 검색하고, 답변의 인용을 검증해 한 번 수리한 뒤에도 위반이 남으면 근거 목록으로 대체합니다.
- 중단된 호출의 비용 예약·후속 정산과 중요 문서 변경 승인을 구현했습니다. Langfuse에는 고객 본문 없이 호출 메타데이터만 전송합니다.

[GitHub](https://github.com/kanziman/NexusWiki) · [서비스](https://www.nexuswiki.net/)

### [channel-voc-demo](https://github.com/kanziman/channel-voc-demo)
**GraphRAG로 고객 상담 문제를 분석하고, 사람 승인 후 GitHub 이슈·Jira 티켓으로 연결하는 에이전트 데모**

- 의미·키워드·그래프 검색을 결합하고, LangGraph로 분석 결과 검토와 승인 흐름을 구현했습니다. 공개 CS 데이터셋 1,200건 기반입니다.

[GitHub](https://github.com/kanziman/channel-voc-demo) · [데모](https://channel-voc-demo.vercel.app/)

### [skillx-map](https://github.com/kanziman/skillx-map)
**여러 AI 개발 도구의 스킬·플러그인을 통합 점검하고, 복구 가능한 삭제를 제공하는 CLI·로컬 웹 UI**

- Claude Code, Codex, Gemini를 지원하며 데이터를 외부로 전송하지 않습니다. 제로 의존성 코어와 플랫폼별 어댑터로 구성했습니다.

[GitHub](https://github.com/kanziman/skillx-map) · [npm](https://www.npmjs.com/package/skillx-map)

<details>
<summary>다른 프로젝트</summary>

- **[입틀막 — 항공 특가 검증 피드](https://deals.nexuswiki.net/deals):** 평소 가격·인접 날짜 가격·관측 시점·신선도를 검증해 특가를 선별합니다. AI가 콘텐츠를 작성하고 사람이 검수합니다.
- **[NSQ — 영어·일본어 쉐도잉 앱](https://github.com/kanziman/nsq):** 공식 대본과 자막의 시간축을 맞춰 화자별 학습을 제공합니다. 일치율이 기준에 못 미치면 임포트를 차단합니다. [서비스](https://nsq-teal.vercel.app/)

</details>

## 기술 기반

Kotlin · Java · Spring Boot · Python · FastAPI · PostgreSQL · Redis · Docker · Kubernetes

## 자격증

[AWS Certified Solutions Architect — Associate](https://www.credly.com/badges/0e84b30f-c0aa-448c-a2ce-d974496f2fea/public_url)

## 연락처

[hwanghkt@naver.com](mailto:hwanghkt@naver.com) · [GitHub @kanziman](https://github.com/kanziman)
