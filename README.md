# sales-engine

🇰🇷 [한국어 README](./README.ko.md)

**Sales engine organizing theory, funnel, metrics, tooling, and Korean context into 5 layers × 6 domains × 3 modes. A deal-complexity router blends methodologies (BANT·MEDDIC·SPIN·Challenger·Sandler·SNAP). Korea overlay (Pre-RFP, bootcamp sales, Narajangteo, channel distribution, Coupang/Naver) is on by default.**

## Prerequisites

- **Claude Cowork or Claude Code** environment

## Goal

B2B/B2C sales requires methodology blending, not single-framework enforcement. This skill organizes the full sales operation — qualification theory (L1), funnel stages (L2), KPIs and forecasting (L3), RevTech stack (L4), and Korea-specific overlays (L5) — into a routable system. Given a deal's complexity (Light/Mid/Heavy/Korea-Heavy), the right mix of methodologies is matched automatically.

## When & How to Use

Invoked on sales diagnosis, sales playbook design, or execution-phase scripts (cold outbound, RFP response, demo, closing). Three modes: **M1 Diagnose** (current pipeline → 5-layer × domain matrix), **M2 Design** (goal → full playbook), **M3 Execute** (situation → scripts/templates). Six domains covered: B2B SaaS, Enterprise, B2C, D2C, Retail, B2G (public procurement).

## Use Cases

| Scenario | Prompt | What Happens |
|---|---|---|
| Pipeline health check | `"우리 SaaS 세일즈 진단해줘"` | M1 / D1 SaaS / Mid → MEDDIC+SPIN blended diagnosis with 5-layer matrix, top-3 bottlenecks, risk flags |
| Public procurement RFP | `"나라장터 RFP 대응 플레이북"` | M2 / D6 B2G / Korea-Heavy → MEDDIC + Pre-RFP + evaluation-sheet reverse engineering |
| Enterprise cold outbound | `"ABM 콜드 이메일 5개"` | M3 / D2 Enterprise / Heavy → Challenger-style sequences, ABM targeting |
| Retail entry | `"쿠팡 입점 영업 전략"` | M2 / D5 Retail / Mid → MD-relationship playbook with Korean overlay |

## Key Features

- **5-Layer Architecture** — METHOD (9 methodologies), FUNNEL (5-stage meta-funnel), METRIC (4-tier KPIs + forecasting), STACK (4-tier RevTech), KOREA (5 Korean patterns)
- **Deal-Complexity Router** — Light/Mid/Heavy/Korea-Heavy → methodology matching (BANT → MEDDIC → MEDDPICC + ABM + Pre-RFP)
- **6 Domains** — B2B SaaS, Enterprise, B2C, D2C, Retail, B2G, each with dedicated overlay
- **Vendor-Neutral** — Salesforce/HubSpot/Gong referenced only as category examples (2026 MCP·AI Agent era-proof)
- **Korea Overlay** — Pre-RFP relationship sales, bootcamp sales, Narajangteo, Coupang/Naver, channel/reseller networks (default On)
- **3 Modes** — Diagnose · Design · Execute, MECE coverage of sales requests

## Works With

- **[copywriting-engine](https://github.com/jasonnamii/copywriting-engine)** — Message-level copy delegated downstream
- **[negotiation-skill](https://github.com/jasonnamii/negotiation-skill)** — Negotiation phase delegated downstream
- **[biz-skill](https://github.com/jasonnamii/biz-skill)** — Business strategy (upstream of sales)
- **[management-skill](https://github.com/jasonnamii/management-skill)** — Sales org hiring & comp
- **[bp-guide](https://github.com/jasonnamii/bp-guide)** — Pitch decks and IR

## Installation

```bash
git clone https://github.com/jasonnamii/sales-engine.git ~/.claude/skills/sales-engine
```

## Update

```bash
cd ~/.claude/skills/sales-engine && git pull
```

Skills placed in `~/.claude/skills/` are automatically available in Claude Code and Cowork sessions.

## Part of Cowork Skills

This is one of 25+ custom skills. See the full catalog: [github.com/jasonnamii/cowork-skills](https://github.com/jasonnamii/cowork-skills)

## License

MIT
