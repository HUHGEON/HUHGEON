<picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/HUHGEON/HUHGEON/main/cards/win-top-dark.svg"><img width="100%" src="https://raw.githubusercontent.com/HUHGEON/HUHGEON/main/cards/win-top-light.svg" alt="~/heo-geon · zsh"></picture>

`❯` **Backend · API · Database · Async · Realtime**

# 백엔드를 만들고, 데이터로 결과를 검증합니다.

저는 화면 뒤에서 데이터가 흐르는 구조를 설계하는 백엔드 개발자입니다.

**API 설계와 ERD·DB 모델링**부터 캐싱 · 비동기 처리 · 장애 복구까지, 서버의 뒷단을 탄탄하게 만드는 것.
복잡한 요구사항을 **명확한 데이터 모델과 안정적인 API**로 풀어내는 것.
그것이 제가 백엔드 개발자로서 추구하는 방향입니다.

`명지대학교 컴퓨터공학과 · 2020.03 ~ 2026.02`
`LG U+ 유레카 백엔드 과정 수료 · 2026.04 ~ 2026.10`
`엠트리센 백엔드 개발 인턴 · 2025.08 ~ 2026.01`
`SQLD · 2025.06`
`★ 명지대 캡스톤디자인 금상 · 음성인식 키오스크`
`★ 코드잇 데모데이 대상 · 조각집`

[포트폴리오 ↗](https://huhgeon.github.io/portfolio/) · [요약 PDF](https://huhgeon.github.io/portfolio/heo-geon-portfolio.pdf) · [기술 블로그 ↗](https://huhgeon.github.io) · [Email](mailto:rjs2337@naver.com)

## Projects

<table>
<tr><td colspan="2" valign="top">

#### [스마트폰 사전예약 (NOVA)](https://github.com/Nova-Grandis/be) →

담당: 회원 인증 · 상품 · 리뷰 · 장바구니 · 럭키드로우 · 공통 모듈(JWT 검증 · 읽기 캐시)

- 백엔드 저장소 커밋 **677/1,420** 으로 최다 기여, 동시성 결함 **4종**을 재현 시험으로 운영 전에 잡아 수정
- 부하 시험에서 catalog 네 대 중 한 대만 막히는 것을 태스크별 지표로 확인해 ALB 분배를 처리 중 요청이 적은 쪽으로 변경, 대기열 입장 속도 가정이 틀려 끊기던 시험 판정을 실제 설정값 기반 계산으로 수정

`Java 25` `Spring Boot 4.1` `MySQL 8.4` `Valkey` `AWS SQS` `ECS Fargate`

</td></tr>
<tr><td width="50%" valign="top">

#### [선착순 쿠폰 발급 시스템](https://github.com/coupon-yaho/cy-be) →

담당: 검증 배치 · 시드 생성기 · 부하 시험 결과 DB 대조

- 이력 **534만 행**을 재생하는 검증 배치 설계·구현, 오류 **700건**을 주입한 데이터에서 기대 검출 **800행**을 누락 0 · 오탐 0으로 확인
- 팀의 잠금 방식 개선 과정에서 부하 시험 결과를 DB와 대조해 500 req/s 성공 응답 중앙값 1초 이상 회차 **4/7 → 0/7** 검증

`Java 21` `Spring Boot` `Spring Batch` `MySQL` `Redis` `Kafka`

</td><td width="50%" valign="top">

#### [라이브 커머스 채팅 서버](https://github.com/sago-panda/sapari-be) →

- 서로 다른 서버에 연결된 시청자 간 채팅을 Redis Pub/Sub 전달 파이프라인으로 중계
- 권한 · 레이트리밋 · 욕설 마스킹 · 저장 · 발행을 하나의 전송 파이프라인 안에서 단계별로 분리

`Spring WebFlux` `WebSocket` `Redis` `MongoDB`

</td></tr>
<tr><td width="50%" valign="top">

#### [음성인식 키오스크](https://github.com/Say-It-It-s-OK/nlp) → &nbsp; `★ 캡스톤디자인 금상`

- LLM으로 intents를 추출하고 API 서버를 호출하는 오케스트레이터 구조로 NLP 서버 설계
- LLM 출력을 intents **9종** · filters 스키마로 정형화해 한 문장에 담긴 여러 요청을 순차 실행으로 변환

`FastAPI` `gpt-4o-mini` `Express` `MongoDB` `Swagger`

</td><td width="50%" valign="top">

#### [해야지 (haeyaji)](https://github.com/haeyaji/haeyaji-nlp) →

- 로컬 LLM(EXAONE)의 오분류 · 없는 장소 추천을 규칙 라우팅 · RAG · 스키마 강제로 줄이고 시나리오 채점 **59/80**으로 남은 한계까지 확인
- 느린 LLM 호출로 커넥션 풀이 고갈되지 않도록 추천 게이트웨이 트랜잭션 분리, 맥락별 개인화 가중치 학습

`FastAPI` `Ollama · EXAONE` `Spring Boot` `MySQL` `Redis`

</td></tr>
</table>

## Stats

<img width="49%" src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=HUHGEON&theme=github_dark" alt="활동 통계" /> <img width="49%" src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=HUHGEON&theme=github_dark" alt="커밋 기준 주력 언어" />

<a href="https://github.com/Baek-Seunghyun/ai-coding-usage-card"><img width="100%" src="https://raw.githubusercontent.com/HUHGEON/HUHGEON/main/cards/ai-usage-full.svg" alt="AI usage" /></a>

<a href="https://github.com/TOKENPHAGE"><img width="100%" src="https://api.tokenphage.com/badge/HUHGEON?theme=grass-claude&mode=dark" alt="Tokenphage" /></a>

<picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/HUHGEON/HUHGEON/main/cards/win-bottom-dark.svg"><img width="100%" src="https://raw.githubusercontent.com/HUHGEON/HUHGEON/main/cards/win-bottom-light.svg" alt="main · ~/heo-geon · 6 projects"></picture>
