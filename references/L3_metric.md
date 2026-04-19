# L3 METRIC — KPI·벤치마크·포캐스팅

세일즈 지표 4계층 + 유닛이코노믹스 + 포캐스팅 방법론. 도메인별 KPI 오버레이.

---

## KPI 4계층 구조

| 계층 | 지표 | 주기 |
|------|------|------|
| **활동(Activity)** | 콜 수·이메일 수·미팅 수·데모 수 | 일간 |
| **파이프라인(Pipeline)** | Pipeline Coverage·Stage별 전환률·Velocity | 주간 |
| **수익(Revenue)** | 신규ARR·Win Rate·ACV·Sales Cycle | 주간·월간 |
| **효율(Efficiency)** | CAC·LTV:CAC·CAC Payback·Magic Number·Quota Attainment | 월간·분기 |

---

## 핵심 벤치마크 (B2B SaaS 기준)

| 지표 | 헬시 | 톱티어 | 출처 |
|------|------|--------|------|
| Pipeline Coverage | 3-5x | 4-6x | Outreach, Fullcast |
| 엔터프라이즈 Win Rate | 20-30% | 35%+ | Monetizely |
| SMB 사이클 | 30-60일 | <30일 | Monetizely |
| 엔터프라이즈 사이클 | 90-180일 | <90일 | Monetizely |
| NRR (Net Revenue Retention) | 110%+ | 130%+ | ChurnZero |
| GRR (Gross Revenue Retention) | 90%+ | 95%+ | ChurnZero |
| LTV:CAC | 3:1 | 4-6:1 | FinancialModelsLab |
| CAC Payback | <18개월 | <12개월 | Monetizely |
| Forecast Accuracy | ±10% | ±5% | Monetizely |

---

## 도메인별 KPI 오버레이

### D1 B2B SaaS
ARR · NRR · GRR · Logo Retention · ACV · CAC Payback · Magic Number · Rule of 40

### D2 엔터프라이즈
ACV (크게) · Deal Size · Win Rate · Sales Cycle · Pipeline Coverage · Champion Score · Quota Attainment

### D3 B2C
Conversion Rate · AOV · CAC · Repeat Purchase Rate · NPS

### D4 D2C
ROAS · LTV · AOV · Repeat Rate · Cohort Retention · CAC by Channel
- ROAS 2025: Meta 2.2x · TikTok 1.4x · Google 4.5x · 헬시 D2C 4-6x
- LTV:CAC 헬시 3:1 · 프리미엄 4-6:1

### D5 리테일
매장당 매출 · SKU당 매출 · 재고회전율 · MD 입점률 · 수수료율 (쿠팡·네이버 10% / 홈쇼핑 20%)

### D6 B2G
입찰 참여율 · 낙찰률 · 평균 계약액 · 갱신률 · 평가점수

---

## 포캐스팅 방법론 3종

| 방법 | 로직 | 적합 | 한계 |
|------|------|------|------|
| **Weighted Pipeline** | ∑(딜금액 × Stage별 확률) | 대부분 | Stage 확률 캘리브레이션 필요 |
| **Historical** | 과거 Win Rate × 현재 파이프라인 | 데이터 충분한 조직 | 시장변화 미반영 |
| **AI-driven** | ML 모델 (Gong/Outreach) | 대규모 파이프라인·고품질 데이터 | 도입·튜닝 비용 |

**2025 권장:** Weighted + AI-driven 병행, Historical은 보정용.

---

## 추적 주기 (Cadence)

| 주기 | 지표 |
|------|------|
| **일간** | 활동지표·신규 리드·Top 딜 상태 |
| **주간** | Pipeline Coverage·신규ARR·Win Rate·Slippage·리딩지표 |
| **월간** | NRR·GRR·CAC Payback·Magic Number·Quota Attainment·Capacity |
| **분기** | Segment·가격모델별 전체 효율 리뷰·가격패키징 임팩트 |

---

## 한국 조정 메모

글로벌 벤치마크를 한국에 그대로 적용 금지:
- 한국 SaaS NRR은 글로벌 110%+ 대비 95-105% 수준 관찰(업계 컬럼 기반, 정량 공개 부족)
- 엔터프라이즈 사이클은 Pre-RFP 3-6개월 별도 가산 필요
- D2C ROAS는 한국 Meta·네이버 혼합 — 벤치마크 그대로 적용 주의
- 공공조달 KPI는 글로벌에 없음 → D6 자체 정의 사용

---

## Sources
- [Outreach Pipeline Coverage](https://www.outreach.ai/resources/blog/sales-pipeline-coverage-ratio)
- [Monetizely SaaS Metrics 2025](https://www.getmonetizely.com/articles/the-saas-sales-metrics-that-matter-most-in-2025-and-how-to-use-them)
- [ChurnZero CS Metrics](https://churnzero.com/blog/customer-success-revenue-metrics-that-matter/)
- [Financial Models Lab SaaS KPIs](https://financialmodelslab.com/blogs/kpi-metrics/saas)
- [Upcounting Ecommerce ROAS 2025](https://www.upcounting.com/blog/average-ecommerce-roas)
