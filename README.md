# leoreo

<p align="center">
  <img src="assets/leoreo.png" alt="Le Oreo" width="360">
</p>

**돈 버는 개발(revenue-driven development)을 강제하는 Claude Code 스킬.**

이미 사업 아이템이 있는 스타트업 개발자를 위한 진단 프레임워크다. 새 창업 아이디어를 만들어주는 도구가 아니다. 개발 + 비즈니스 재무 사고를 같이 하는 사람을 위해, 개발할 때마다 이 질문들을 강제한다:

- 우리의 **진짜 병목**은 무엇인가? 생산성이 어디서 안 나오나?
- 소프트웨어 개발에서는 어디가 병목인가?
- 어디서 돈을 벌고, 어떻게 뚫어야 하나?
- 이 기능의 **인풋(비용) 대비 아웃풋(수익)** 은 얼마인가? 회수 기간은?
- 만들기 전에 더 싸게 검증할 방법은 없나? kill 기준은 숫자로 정했나?

카테고리: **사업 · 개발**

## 뭐가 들어있나

### 스킬 1: `leoreo` — 돈 버는 개발 진단

| 파일 | 내용 |
|---|---|
| `SKILL.md` | 핵심 진단 프레임워크 — 병목 진단(AARRR + 개발 생산성), 기능 투자 판단 게이트 7개, 돈-체크 테이블(표준 출력물), 롤아웃/사후검증, 한국 맞춤 체크 |
| `references/global-frameworks.md` | 서적 11권 실행 규칙(Lean Startup, Mom Test, Zero to One, $100M Offers, Lean Analytics, Hooked, Traction 등), 지표 공식·벤치마크(LTV:CAC, NRR, Rule of 40, Burn Multiple), YC/Paul Graham 지혜, 비용 사고, 검증 사다리 |
| `references/korea-playbook.md` | 토스·당근·배민·무신사·쿠팡에서 뽑은 기능 단위 교훈, 국내 실패 패턴, 한국 시장 특수성(플랫폼 리스크·PG/인앱결제·B2B 결재 문화·정부지원사업 함정), 한국식 검증 채널 |

### 스킬 2: `leoreo-pay` — 한국 결제시스템 & 수익모델

| 파일 | 내용 |
|---|---|
| `leoreo-pay/SKILL.md` | 5단계 설계 순서 강제 — 수익모델 선택 → 가격 설계 → PG 선정 → 구현 불변식 8개 → 한국 규제 체크 |
| `leoreo-pay/references/revenue-models.md` | 수익모델 14종 분류표(구현 난이도 포함), 가격 설계(value-based, 티어, charm pricing), 구독 벤치마크(연간 할인 15~20%, trial 전환율, freemium 2~5%), take rate 벤치마크(앱스토어·배민·쿠팡), AI 시대 하이브리드 과금 |
| `leoreo-pay/references/korea-pg.md` | PG 지형도(토스페이먼츠·KG이니시스·KCP·나이스), 포트원 vs 직연동, 결제수단별 함정, 빌링키 제약, 인앱결제 수수료, 전금법 개정·전자상거래법·현금영수증, 해외 판매(Paddle/MoR vs 해외법인+Stripe) |
| `leoreo-pay/references/payment-engineering.md` | 상태 머신, 금액 위변조 검증, 멱등성, 웹훅(서명·중복·순서·유실), 대사/이중장부, 환불, dunning, 보안, 시나리오 테스트 체크리스트 |

## 설치

```bash
git clone https://github.com/animepics/leoreo.git
ln -s "$(pwd)/leoreo" ~/.claude/skills/leoreo
ln -s "$(pwd)/leoreo/leoreo-pay" ~/.claude/skills/leoreo-pay
```

또는 복사 설치:

```bash
cp -r leoreo ~/.claude/skills/leoreo
cp -r leoreo/leoreo-pay ~/.claude/skills/leoreo-pay
```

## 사용

Claude Code에서:

```
/leoreo 이번 스프린트에 뭐부터 해야 돈이 되지?
leoreo 이 기능 만들 가치 있나? — 관리자 대시보드 리뉴얼
돈 버는 개발 관점에서 지금 로드맵 진단해줘

/leoreo-pay 구독 결제 붙이려는데 설계해줘
leoreo-pay 우리 서비스 수익모델 뭐가 맞아? 가격은?
PG 뭐 써야 하고 빌링 어떻게 구현해?
```

`leoreo`의 결론은 항상 셋 중 하나: **착수 / 더 싼 검증부터 / 하지 마라** — 근거 숫자와 함께.
`leoreo-pay`는 수익모델 → 가격 → PG → 구현 → 규제 순서를 강제한다.

## 왜 leoreo인가

Leorio + Oreo = Le Oreo. 헌터가 된 이유가 돈인 남자. 이 스킬의 정신적 지주다.
