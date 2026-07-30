# 글로벌 프레임워크 부록 — 돈 버는 개발

이미 사업 아이템·매출이 있는 스타트업 개발자 기준으로 재구성한 지식 베이스. 프레임워크/서명은 원문 유지.

## 1. 서적별 실행 규칙

### The Lean Startup — Eric Ries
- **Build-Measure-Learn 루프**: MVP는 "가장 작은 제품"이 아니라 "루프를 최소 노력으로 가장 빨리 도는 버전". 기존 제품 신기능도 풀스펙 대신 루프 1회전 분량으로 쪼개서 출시.
- **Validated Learning**: 기능 출시 전 "이 기능이 검증하려는 가설"을 먼저 문장으로 쓴다. 없으면 빌드 금지.
- **Innovation Accounting**: vanity metric(총 가입자 수 등) 대신 코호트 기준 학습 지표로 성과 보고.

### The Mom Test — Rob Fitzpatrick
- 3대 규칙: (1) 아이디어 말고 상대의 삶/업무를 물어라 (2) 미래 가정 대신 과거 구체 사실을 물어라 (3) 말은 적게, 듣기는 많이.
- **나쁜 데이터 3종**: 칭찬 / 가정형 미래("있으면 좋겠다") / 위시리스트 — 전부 노이즈, 의사결정에서 제외.
- 기존 제품 적용: 기능 요청이 오면 "그 문제를 지금 어떻게 해결 중인가"부터 캐묻는다. 대안 없이 "있으면 좋을 듯"인 요청은 백로그 최하단.

### Zero to One — Peter Thiel
- **10x 규칙**: 20% 개선은 전환 마찰을 못 이긴다. 10배 나은 지점에만 자원 집중, feature parity 경쟁 지양.
- **독점 4요소**: 독자 기술 / 네트워크 효과 / 규모의 경제 / 브랜드 — 기능이 아무것도 강화 안 하면 우선순위 하향.

### Rework — 37signals
- 제약(리소스 부족)을 변명이 아니라 설계 조건으로 써라.
- 핵심 기능 준비되면 즉시 출시, 다듬기는 나중에. "영감엔 유효기간이 있다."
- 광고 대신 가르치는 마케팅(블로그/문서로 제품 가치 증명).

### $100M Offers — Alex Hormozi
- **Value Equation**: `Value = (Dream Outcome × 달성 확신) / (Time Delay × Effort)`. 기능이 4변수 중 최소 1개를 개선하는지 스펙 리뷰에서 명시적으로 답하게 한다.
- 기능을 낱개로 팔지 말고 결과(outcome) 단위로 묶어 포지셔닝.

### Start Small, Stay Small / The SaaS Playbook — Rob Walling
- **Stair Step Method**: 단일 채널·단순 상품 → 안정적 소액 매출 → 확장. 신규 기능 라인도 작게 검증 후 본 제품에 통합.
- 니치 우선: 작은 시장의 큰 조각이 초기엔 더 방어 가능.
- 기능 개발도 "이번 매출로 회수 가능한가" 기준으로 승인.

### Lean Analytics — Croll & Yoskovitz
- **OMTM(One Metric That Matters)**: 지금 단계에서 리스크가 가장 큰 지표 하나만 전사가 본다.
- 5단계: Empathy → Stickiness → Virality → Revenue → Scale. 매출 단계 이상이면 OMTM 후보는 LTV:CAC·순이익률·Churn 계열이지 가입자 수가 아니다.
- 게이트 통과 전에 다음 단계 지표에 투자하는 것은 낭비 신호.

### Hooked — Nir Eyal
- **Hook Model**: Trigger → Action → Variable Reward → Investment. 리텐션 기능 설계 시 4단계 중 빈 곳을 진단.
- Investment(사용자가 쌓은 데이터/평판/커스터마이징)가 클수록 스위칭 코스트↑ → churn 방어 기능으로 우선 검토.

### Traction — Weinberg & Mares
- **Bullseye Framework**: 19개 채널 브레인스토밍 → 3~4개 저비용 테스트 → 1개에 집중. 성장 정체 진단 시 "검증 안 해본 채널이 몇 개 남았나"부터 센다.
- **Engineering as Marketing**: 무료 툴/계산기/공개 데이터셋으로 채널 자체를 만든다 — 개발 리소스를 마케팅 자산으로 전환하는 고ROI 옵션.

### Obviously Awesome — April Dunford
- 포지셔닝 5요소: 경쟁 대안 → 고유 속성 → 가치 → 타겟 → 카테고리. 기능 전에 "이 기능이 없으면 고객이 쓸 대안"부터 정의.
- 신기능 실패 시 포지셔닝 문제인지 기능 결함인지 먼저 구분.

### Crossing the Chasm — Geoffrey Moore
- Early Adopter(비전 구매)와 Early Majority(실용 구매)는 구매 심리가 다르다. "레퍼런스 고객 있나"를 묻는 고객이 늘면 캐즘 진입 신호.
- **Bowling Alley**: 한 세그먼트의 whole product(연동/문서/지원 포함) 완성에 집중 후 인접 확장. 로드맵을 여러 세그먼트에 분산하지 마라.

## 2. 지표 공식 · 벤치마크

> 벤치마크는 2025~2026년 SaaS 업계 리서치 기준. 회사 스테이지에 따라 하방 이탈이 정상.

### Unit Economics
- **CAC** = 총 마케팅/영업 비용 ÷ 신규 고객 수
- **LTV** = ARPU × Gross Margin% × 평균 고객 수명(≈ 1/월 churn)
- **LTV:CAC**: 건강 범위 **3:1~5:1**. 3 미만 = 구조 문제(제품/가격/타겟), 5 초과 = 성장 투자 과소.
- **CAC Payback** = CAC ÷ (월 ARPU × Gross Margin%). **12개월 이내 건강**, 세일즈 어시스트 12~18개월 허용, 24개월+ 위험.
- 함정: LTV:CAC 4:1이어도 payback 30개월이면 현금이 먼저 마른다. 둘 다 봐라.

### SaaS Metrics
- **MRR/ARR**, ARR = MRR × 12
- **Customer Churn** = 이탈 고객 ÷ 기간 시작 고객 × 100
- **Gross Revenue Churn** = (해지+다운그레이드 MRR) ÷ 시작 MRR × 100
- **NRR** = (시작 MRR + Expansion − Contraction − Churn) ÷ 시작 MRR × 100. **<100% 적신호, 110~120% 양호, 120%+ elite**
- **Rule of 40**: 성장률% + 이익률% ≥ 40
- **Burn Multiple** = 순 현금 소진 ÷ 신규 ARR 순증. **<1.0x 이상적, >2x 경고**
- **Gross Margin**: SaaS 건강 범위 **75~85%**. 서비스/온보딩 인건비가 매출원가를 잡아먹는 지점이 흔한 병목.

### AARRR (Pirate Metrics) — Dave McClure
Acquisition → Activation → Retention → Referral → Revenue. 병목 진단 = 전환율이 가장 낮은 구간 찾기.

### 기능 단위 ROI 스코어링
- **RICE** = (Reach × Impact × Confidence) ÷ Effort (Intercom). 우선순위 논쟁을 변수 단위로 쪼개 합의.
- **ICE** = Impact × Confidence × Ease (Sean Ellis). 빠른 growth 실험용.
- **WSJF** = Cost of Delay ÷ 작업기간 (Reinertsen/SAFe). Cost of Delay = 미룰 때 단위 시간당 잃는 매출+비용.
- **기술부채**: 스프린트 용량 ~15% 상시 배정이 실무 기준선. 항목별로 "매출 작업 지연 / 지원비용 증가 / 컴플라이언스 리스크" 중 하나에 답해야 백로그 정식 항목.

## 3. YC / Paul Graham / 인디해커

- **Make Something People Want** (YC): 신기능마다 "이걸 원하는 특정 사람이 실존하나"부터.
- **Do Things That Don't Scale** (PG): 신기능은 소수 핵심 고객에게 수동으로 먼저 붙여보고(컨시어지) 자동화는 나중에. 성장은 꾸준한 %성장의 복리다.
- **Default Alive vs Default Dead** (PG, 2015): 분기마다 계산 — `runway(개월) > 흑자 전환까지 필요한 개월`인가?
- **Ramen Profitable** (PG): Default Dead → Alive 전환의 최소 기준선.
- **실패 원인 1위 = 니즈 부재** (CB Insights ~42%, 2위 현금 고갈 29%, 3위 팀 23%). 기능 사후 부검도 이 순서로.
- **PMF 신호**: 입소문, 자연 증가, 영업 없이 팔림 (Andreessen). **Sean Ellis 40% Test** — "못 쓰게 되면 매우 실망" ≥40%면 PMF 근거, 60%+ 최상위.
- **levels.io 전술**: 결제까지 붙인 못생긴 랜딩을 먼저 내고 돈이 들어오는지만 본다. 실결제가 되는 최소 완성품만 인정. Build in Public으로 시장 신호를 외부 압력으로 전환.

## 4. 비용 사고

### FinOps
- Inform(비용 가시화) → Optimize(낭비 제거) → Operate(예측 내재화). 배포 전 IaC 단계에서 비용 추정(Infracost류)을 습관화.
- 기능 배포 시 "예상 인프라 증분 비용 vs 예상 매출 기여"를 항상 나란히 적는다.

### Build vs Buy
- 핵심 질문: 차별화 지점인가? Yes → Build, No → Buy. 결제·인증·이메일·모니터링을 자체 구축하는 건 엔지니어 시간을 매출 무관 작업에 태우는 것.
- 기본값: **먼저 사고, 필요해지면 만든다.**

### 엔지니어 시간 원가
- Fully-loaded 비용 = 연봉의 **1.25~2배** ÷ 연 근무시간 (복지·세금·장비·채용비 포함). 어림값 시니어 $100~150/시간.
- 스프린트 1주(1인)를 쓰는 기능은 최소 그 주의 fully-loaded 비용만큼 매출/절감 기대치가 있어야 승인.

## 5. 검증 사다리 (저비용 → 고비용)

| 단계 | 방법 | 비용 | 확인 대상 |
|---|---|---|---|
| 1 | 고객 인터뷰 (Mom Test) | 최저 | 문제가 실재하는가 |
| 2 | 랜딩페이지 / Fake Door | 낮음 | 수요가 있는가 (클릭/신청) |
| 3 | 사전결제 / 크라우드펀딩 커밋 | 중저 | 지갑이 열리는가 |
| 4 | Concierge / Wizard-of-Oz 수작업 | 중 | 워크플로우가 실제 가치 있는가 |
| 5 | 프로덕션 기능 | 최고 | 스케일 가능한 실사용 데이터 |

- 이전 단계 신호 없이 다음 단계 진입 금지. "수요 검증 → 전달 검증 → 자동화" 순서.
- **Kill Criteria는 사전에 숫자로**: 랜딩 전환 <X%, 사전결제 <Y건, 재사용률 <Z% → 중단.
- **위양성 신호**: 칭찬 / "있으면 쓸 것 같아요" / 선결제 없는 구두 약속 / 참여도 높은데 결제 0. 진짜 신호는 돈과 시간이 실제로 움직였는가뿐.

## 출처

Paul Graham 에세이(Do Things That Don't Scale, Default Alive or Default Dead), CB Insights 스타트업 포스트모템, 각 서적 원서(위 서명 참조), Intercom RICE, SAFe WSJF, Amplitude AARRR/Hooked 해설, ChartMogul·Wall Street Prep·CloudZero SaaS 벤치마크, FinOps Foundation, Sean Ellis PMF Survey.
