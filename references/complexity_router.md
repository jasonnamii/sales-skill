# 딜 복잡도 라우터

**1차 분기 기준:** 모든 세일즈 요청의 시작점. 사이클·의사결정자수(DM)·ACV로 복잡도 판정 → 방법론 블렌딩 매칭.

---

## 복잡도 매트릭스

| 복잡도 | 사이클 | DM수 | ACV | 1차 방법론 | 2차 블렌딩 |
|--------|--------|------|-----|-----------|----------|
| **Light** | ≤30일 | 1명 | <$10K | BANT·SNAP | - |
| **Mid** | 30-90일 | 2-4명 | $10K-$100K | SPIN·Solution Selling | Sandler 선택적 |
| **Heavy** | 90-180일+ | 5+명 | $100K+ | MEDDIC·MEDDPICC | Challenger·ABM |
| **한국Heavy** | Pre-RFP 3-6개월 포함 불확정 | 복수+관계영업 | 불확정 | MEDDIC + Pre-RFP 한국오버레이 | Challenger·ABM·부트캠프영업 |

---

## 판정 로직 (Python 의사코드)

```python
def route(cycle_days, dm_count, acv_usd, is_korea_enterprise):
    if is_korea_enterprise and (cycle_days > 90 or "RFP" in context):
        return "한국Heavy"
    if cycle_days >= 90 or dm_count >= 5 or acv_usd >= 100000:
        return "Heavy"
    if cycle_days >= 30 or dm_count >= 2 or acv_usd >= 10000:
        return "Mid"
    return "Light"
```

**우선순위:** 한국Heavy > Heavy > Mid > Light. 임계값 중 어느 하나라도 상위 조건 충족 시 상위 레벨로 승격.

---

## 방법론 블렌딩 조합

| 상황 | 조합 | 이유 |
|------|------|------|
| 트랜잭셔널·빠른 의사결정 | BANT + SNAP | 빠른 퀄·분석마비 회피 |
| 중형 솔루션·복수 DM | SPIN + Solution Selling | 니즈 페인 발굴 + 솔루션 매핑 |
| 엔터프라이즈 복합 | MEDDIC + Challenger | 퀄리피케이션 + 인사이트 주도 |
| 엔터프라이즈 + 바이잉커미티 | MEDDPICC + ABM | Paper Process·Competition 포함 + 계정 단위 접근 |
| 한국 대형 | MEDDIC + Pre-RFP 관계영업 + 부트캠프 | 글로벌 퀄 + 한국 관계영업 오버레이 |
| 공공조달 | MEDDIC + 나라장터 대응 | RFP 전 판짜기 + 공공 평가기준 정렬 |

---

## 금지 조합

- 단일 방법론 강요 (BANT만 / MEDDIC만) → 2025 블렌딩 표준 위배
- Light에 MEDDPICC 적용 → 오버엔지니어링, 사이클 지연
- 한국 엔터프라이즈에 BANT 단독 → Pre-RFP 관계영업 누락

---

## Gotchas

| 함정 | 대응 |
|------|------|
| ACV 불명 | 사이클·DM수 2개 기준으로 판정. ACV 무시 가능 |
| 도메인이 B2C인데 복잡도 적용 시도 | B2C는 복잡도 라우터 대신 AIDA·AARRR 퍼널 중심. D3 도메인 오버레이 참조 |
| 한국 엔터프라이즈인데 "한국Heavy" 무시 | 한국 기업+엔터프라이즈+사이클 90일+ = 자동 승격 |
