# 황경태 | Backend Engineer

글로벌 5개 리전 콘텐츠 플랫폼과 1일 100만 건 금융 데이터 인프라를 개발·운영해 온 백엔드 엔지니어입니다.

AI 시대에 개인이 어떤 역량을 쌓아야 하는지가 요즘 가장 큰 관심사입니다. AI를 충분히 쓰면 한 사람이 할 수 있는 일의 범위가 넓어진다고 보고, 그 힘을 백엔드 경험을 바탕으로 제품 전체를 보는 시야를 키우는 데 쓰고 싶습니다. 그래서 업무 밖에서도 도메인이 다른 프로젝트를 하나씩 만들고 있고, 최근에는 콘텐츠 제작과 이커머스 쪽 자동화도 해 보고 있습니다.

[Portfolio](https://brand-design-one.vercel.app/portfolio.html) · [Resume](https://brand-design-one.vercel.app/resume.html) · [Email](mailto:hwanghkt@naver.com)

---

## Side Projects

### [NexusWiki](https://github.com/kanziman/NexusWiki) (2026.08 - 진행 중)
* **팀 지식 위키 (사내 플랫폼 도입)** | [GitHub](https://github.com/kanziman/NexusWiki) · [서비스](https://www.nexuswiki.net/)
* 회사 사양서 기반 챗봇을 만든 경험에서 출발해, 팀원끼리 지식을 위키로 공유하려고 제안하고 만든 서비스입니다. LLM이 원문을 상호 링크된 위키로 정리하고, 답변마다 원문과 위키 양쪽 출처를 인용합니다.
* 4채널 하이브리드 검색으로 원문과 위키를 함께 인용하고, 채널별 순위와 RRF 기여도를 비교하는 개발용 디버그 뷰어로 검색 단계 문제를 분리해 진단합니다.
* 팀별 데이터 격리는 애플리케이션이 아닌 Postgres RLS로 강제하고, 임베딩 호출은 worker 전용 키와 사설망으로 경계를 나눴습니다.

### [channel-voc-demo](https://github.com/kanziman/channel-voc-demo) (2026)
* **에이전트 · GraphRAG** | [GitHub](https://github.com/kanziman/channel-voc-demo) · [Live Demo](https://channel-voc-demo.vercel.app/)
* 고객 상담(VOC) 대화에서 반복되는 문제의 루트원인과 예상 매출 손실액을 찾아, 사람이 승인하면 GitHub 이슈와 Jira 티켓으로 연결하는 에이전트입니다. (공개 CS 데이터셋 1,200건 기반)
* 의미 검색, 키워드 검색, 그래프 검색을 RRF로 결합한 3중 하이브리드 GraphRAG와 LangGraph 사람 승인 게이트를 구현했고, Vercel 번들 용량 한도를 넘는 문제를 의존성 정리와 외부 임베딩으로 풀어 서버리스로 배포했습니다.

### [입틀막 - 항공 특가 검증 피드](https://deals.nexuswiki.net/deals) (2026.08 - 진행 중)
* **데이터 검증 서비스** | [서비스](https://deals.nexuswiki.net/deals)
* 항공권 가격을 수집해 노선별 평소 가격과 인접 날짜 가격을 대조하고, 실제로 저렴한 특가만 게시하는 서비스입니다. 콘텐츠는 AI 에이전트가 작성하고 사람이 검수합니다.
* 할인율, 서로 다른 시각의 관측 2건, 신선도, 인접일 최저가를 모두 통과해야 특가로 인정하는 검증 게이트를 설계했고, 기준가보다 싸지 않은 건은 문안 생성을 건너뛰도록 했습니다.

### [skillx-map](https://github.com/kanziman/skillx-map) (2026)
* **CLI · 로컬 웹 UI** | [GitHub](https://github.com/kanziman/skillx-map) · [npm](https://www.npmjs.com/package/skillx-map)
* Claude Code, Codex, Gemini에 쌓이는 AI 스킬과 플러그인을 한곳에서 스캔·점검·정리하는 도구입니다. 모든 삭제는 복구 가능한 휴지통으로 가고, 외부로 데이터를 보내지 않습니다.
* 제로 의존성 코어와 플랫폼별 어댑터 구조로 설계했고, npm 출시 후 누적 500+ 다운로드를 기록했습니다.

### [NSQ (No Stupid Questions)](https://github.com/kanziman/nsq) (2026)
* **웹 앱** | [GitHub](https://github.com/kanziman/nsq) · [Live Web](https://nsq-teal.vercel.app/)
* Freakonomics 팟캐스트의 공식 대본과 유튜브 자막의 시간축을 맞춰, 화자가 분리된 영어·일본어 쉐도잉 학습을 제공하는 웹 앱입니다.
* 자동 자막과 공식 대본을 Patience-Diff와 LIS로 정합하고 일치율 85% 미만은 임포트를 막았으며, 소스보다 테스트 코드가 많은 TDD로 개발했습니다.

---

## About

- **AI가 만든 결과는 검증을 거쳐야 믿을 수 있다**: 위키는 출처를 두 번 인용하고, 특가 서비스는 가짜 할인을 걸러 내고, 에이전트는 사람 승인을 거쳐야 티켓을 냅니다. 프로젝트는 달라도 같은 생각에서 나왔습니다.
- **만드는 데서 끝내지 않기**: 회사에서는 새 기능을 붙이는 일만큼 서비스를 안정적으로 굴리는 일도 맡고 있고, 운영에서 반복되는 점검과 검증은 AI로 넘기되 판단이 필요한 지점은 사람이 승인하도록 남겼습니다.

---

## Certifications

<a href="https://www.credly.com/badges/0e84b30f-c0aa-448c-a2ce-d974496f2fea/public_url" target="_blank">
  <img src="https://images.credly.com/images/0e284c3f-5164-4b21-8660-0d84737941bc/image.png" width="120" alt="AWS Certified Solutions Architect – Associate" />
</a>

---

## Contact

- **Email**: [hwanghkt@naver.com](mailto:hwanghkt@naver.com)
- **GitHub**: [@kanziman](https://github.com/kanziman)
