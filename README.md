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

| 파일 | 내용 |
|---|---|
| `SKILL.md` | 핵심 진단 프레임워크 — 병목 진단(AARRR + 개발 생산성), 기능 투자 판단 게이트 7개, 돈-체크 테이블(표준 출력물), 롤아웃/사후검증, 한국 맞춤 체크 |
| `references/global-frameworks.md` | 서적 11권 실행 규칙(Lean Startup, Mom Test, Zero to One, $100M Offers, Lean Analytics, Hooked, Traction 등), 지표 공식·벤치마크(LTV:CAC, NRR, Rule of 40, Burn Multiple), YC/Paul Graham 지혜, 비용 사고, 검증 사다리 |
| `references/korea-playbook.md` | 토스·당근·배민·무신사·쿠팡에서 뽑은 기능 단위 교훈, 국내 실패 패턴, 한국 시장 특수성(플랫폼 리스크·PG/인앱결제·B2B 결재 문화·정부지원사업 함정), 한국식 검증 채널 |

## 설치

```bash
git clone https://github.com/animepics/leoreo.git
ln -s "$(pwd)/leoreo" ~/.claude/skills/leoreo
```

또는 복사 설치:

```bash
cp -r leoreo ~/.claude/skills/leoreo
```

## 사용

Claude Code에서:

```
/leoreo 이번 스프린트에 뭐부터 해야 돈이 되지?
leoreo 이 기능 만들 가치 있나? — 관리자 대시보드 리뉴얼
돈 버는 개발 관점에서 지금 로드맵 진단해줘
```

결론은 항상 셋 중 하나로 나온다: **착수 / 더 싼 검증부터 / 하지 마라** — 근거 숫자와 함께.

## 왜 leoreo인가

Leorio + Oreo = Le Oreo. 헌터가 된 이유가 돈인 남자. 이 스킬의 정신적 지주다.
