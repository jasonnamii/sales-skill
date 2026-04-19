# sales-engine

🇺🇸 [English README](./README.md)

**세일즈 이론·퍼널·지표·도구·한국맥락을 5층 × 6도메인 × 3모드로 조직화한 세일즈 엔진. 딜복잡도 라우터로 방법론(BANT·MEDDIC·SPIN·Challenger·Sandler·SNAP) 블렌딩. 한국 오버레이(Pre-RFP·부트캠프영업·나라장터·채널총판·쿠팡네이버) 기본 On.**

## 전제조건

- **Claude Cowork 또는 Claude Code** 환경

## 목적

B2B/B2C 세일즈는 단일 방법론 강요가 아닌 블렌딩이 2025+ 표준입니다. 본 스킬은 세일즈 전주기 — 퀄 이론(L1), 퍼널 스테이지(L2), KPI·포캐스팅(L3), RevTech 스택(L4), 한국 오버레이(L5) — 을 라우팅 가능한 시스템으로 조직화합니다. 딜 복잡도(Light/Mid/Heavy/한국Heavy)에 따라 방법론 조합이 자동 매칭됩니다.

## 사용 시점·방법

세일즈 진단, 플레이북 설계, 실행단(콜드 아웃바운드·RFP 대응·데모·클로즈) 스크립트 요청 시 발동. 3모드: **M1 진단**(현재 파이프라인 → 5층×도메인 매트릭스), **M2 설계**(목표 → 풀 플레이북), **M3 실행**(상황 → 스크립트·템플릿). 6도메인: B2B SaaS·엔터프라이즈·B2C·D2C·리테일·B2G(공공조달).

## 사용 예시

| 상황 | 프롬프트 | 동작 |
|---|---|---|
| 파이프라인 점검 | `"우리 SaaS 세일즈 진단해줘"` | M1/D1 SaaS/Mid → MEDDIC+SPIN 블렌딩 5층 매트릭스 + Top3 병목 + 리스크 |
| 공공조달 RFP | `"나라장터 RFP 대응 플레이북"` | M2/D6 B2G/한국Heavy → MEDDIC + Pre-RFP + 평가표 역설계 |
| 엔터프라이즈 콜드 | `"ABM 콜드 이메일 5개"` | M3/D2 엔터/Heavy → Challenger 화법 + ABM 시퀀스 |
| 리테일 입점 | `"쿠팡 입점 영업 전략"` | M2/D5 리테일/Mid → MD 관계영업 + 한국 오버레이 강 |

## 핵심 기능

- **5층 아키텍처** — METHOD(9방법론)·FUNNEL(5스테이지 메타퍼널)·METRIC(4계층 KPI+포캐스팅)·STACK(4계층 RevTech)·KOREA(한국 5대 패턴)
- **딜 복잡도 라우터** — Light/Mid/Heavy/한국Heavy → 방법론 매칭(BANT → MEDDIC → MEDDPICC+ABM+Pre-RFP)
- **6도메인** — B2B SaaS·엔터프라이즈·B2C·D2C·리테일·B2G, 각각 독립 오버레이
- **벤더 중립** — Salesforce/HubSpot/Gong은 카테고리 예시로만 (2026 MCP·AI Agent 재편에 내성)
- **한국 오버레이** — Pre-RFP 관계영업, 부트캠프영업, 나라장터, 쿠팡·네이버, 채널·리셀러 네트워크 (디폴트 On)
- **3모드** — 진단·설계·실행, 세일즈 요청 MECE 커버

## 연동 스킬

- **[copywriting-engine](https://github.com/jasonnamii/copywriting-engine)** — 문구 카피 하류 위임
- **[negotiation-skill](https://github.com/jasonnamii/negotiation-skill)** — 협상 단계 하류 위임
- **[biz-skill](https://github.com/jasonnamii/biz-skill)** — 사업전략(세일즈의 상류)
- **[management-skill](https://github.com/jasonnamii/management-skill)** — 영업조직 채용·보상
- **[bp-guide](https://github.com/jasonnamii/bp-guide)** — 피치덱·IR

## 설치

```bash
git clone https://github.com/jasonnamii/sales-engine.git ~/.claude/skills/sales-engine
```

## 업데이트

```bash
cd ~/.claude/skills/sales-engine && git pull
```

`~/.claude/skills/` 에 배치된 스킬은 Claude Code·Cowork 세션에서 자동 인식됩니다.

## Cowork Skills

25+ 커스텀 스킬 중 하나입니다. 전체 목록: [github.com/jasonnamii/cowork-skills](https://github.com/jasonnamii/cowork-skills)

## 라이선스

MIT
