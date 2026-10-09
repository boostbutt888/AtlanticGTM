# Atlantic UWB Go-To-Market Plan — handover context

**Current version:** v0.10 · 7 October 2026 · Owner: JC (product and vertical owner, STYL Solutions)
**Status:** Preliminary, internal. Not for customers. All prices in SGD before GST (US$1 = S$1.28 for USD inputs).

This file travels with the deck so another person can pick it up. Update the version history every time the deck is refined.

---

## 1. Purpose and audience

- **What it is:** the go-to-market execution plan for the Atlantic UWB products. It covers what we sell, to whom, how deals run, prices, costs, seven worked examples with breakeven and return, margin checks, and the open items.
- **Audience:** CEO and Sales Director. JC presents it as product and vertical owner.
- **Goal of the session:** five decisions (slide 3) and owners for the 12 open items (slide 57).

## 2. Governing documents and sources

| Source | Role |
|---|---|
| CIO Office: STYL Product Sheet Process Guide v1.0 (3 Oct 2026) | **The framework.** Six stages per product (scope, facts, market, price, write, release), six price rules, margin and discount rules, STE writing rules, release checklist. Wins over earlier inputs. |
| CIO Office: Precision RTLS Hospital Sales Sheet v1.0 and Product Team Brief v1.0 (draft for review) | Ward prices, product facts, healthcare market size, competitors, stress test, Proxximos price check. |
| Atlantic Product–Market–Customer Map (Sep 2026) | Products, markets, named accounts. |
| JC inputs (6–7 Oct 2026) | Supply terms, install day rates, engineer-day cost, pilot pool, staffing. Superseded where the CIO documents conflict (see slide 56). |
| Model scripts | `model_v10.py` (SGD, three-part pricing, breakeven, ROI, 24-month and quote margins). Earlier USD models `cash.py` and `deal2.py` are kept for v0.9 comparison. |
| Claude Docs "Atlantic UWB proposal" | Original proposal. Not updated since v0.3. |

## 3. The uniform framework (from the CIO)

- **Every quote has three parts:** software per unit per year + hardware service per unit per month (STYL owns the hardware) + set-up one time (site survey, installation per anchor, integration).
- **Price unit = what the buyer budgets in:** bed (Ward), 1,000 m² (Operations RTLS, Flow), gate (Gates).
- **Packages:** three maximum per product, one marked "start here". Two host options: cloud (included) or self-hosted (S$95,000 platform fee per deployment; customer provides servers). Core / Operate / Sovereign editions are retired.
- **Rules:** minimum software fee S$60,000 per site per year (Gates S$250,000 per operator); 3-year contract; extra tags S$800 per 10; no quote below 30% gross margin; target 40% per customer over 24 months; Sales Director approves discounts up to 20%, CEO above; no discount on minimum or platform fee.
- **Pilots:** fixed fee, fixed duration, credited to year 1 if the customer buys. Ward S$40,000 / 90 days; Operations S$25,000 (hardened S$35,000); Flow S$60,000; Gates S$120,000 / 120 days.
- **Evidence:** every technical claim needs Engineering confirmation; every market fact carries a confidence tag (Certain / Likely / Guessing); Guessing never goes into a Sales Sheet.
- **Writing:** Simplified Technical English (ASD-STE100), target 80%.

## 4. Products, prices and release status

| Product | Unit | Software / unit / year | Hardware / unit / month | Status |
|---|---|---|---|---|
| Precision RTLS · Ward | Bed | S$450 | S$30 bays, S$60 1–2 bed rooms | CIO sheet v1.0, stage 5; sign-offs pending |
| Precision RTLS · Operations | 1,000 m² | S$9,000 | S$250 (hardened S$500) | Proposal (mine), stage 1–4 partial |
| Flow & Wayfinding | 1,000 m² public area | S$12,000 | S$250 | Proposal (mine) |
| Hands-free Gates | Gate | S$400 | S$30 | Proposal (mine) |

Simulate is a workshop tool and a paid gate study (S$28,000). Occupancy, Device Ops and Environmental Sensing use no UWB and are not priced here.

**Key product facts (Engineering, via CIO):** ±20 cm accuracy (badge on a person); 2 positions each second; 1 anchor serves 8 tags at one time; badge needs a charge each week; not medical grade; no help button. **Not yet confirmed:** hardened kit, gate throughput with the 8-tag limit, passenger phones per anchor.

## 5. Headline numbers (v0.10, preliminary)

| Example | Product | First PO | Year 1 | 3-yr ROI | 24-month margin |
|---|---|---|---|---|---|
| TTSH, 500 beds, self-hosted | Ward | Month 9 | S$544K | 227% | 73% |
| CAG terminal, 25,000 m² | Flow | Month 11 | S$498K | 93% | 51% |
| SATS/dnata cargo, 2 sites | Operations | Month 8 | S$494K | 92% | 50% |
| LTA, 720 gates | Gates | Month 17 | S$1.22M | 88% | 47% |
| MOE via DBS, 5 schools | Operations | Month 16 | S$868K | 140% | 61% |
| 3PL warehouse, 1 site | Operations | Month 6 | S$120K | 39% | 35% (below 40% target) |
| Construction site, hardened | Operations | Month 8.5 | S$182K | 62% | 43% |

Breakeven is about 4 months after the PO in every example. All examples pass the 30% quote floor.

## 6. Assumptions and open items

- **Register:** A1–A50 on slides 51–55, renumbered in v0.10 around the CIO framework. Columns: value, source (CIO / JC / Map / Mine / benchmark), confidence, status.
- **Changes from v0.9:** slide 56 lists the 12 inputs that the CIO documents replaced.
- **12 open items** (slide 57). Most urgent: approve units and prices for Operations, Flow and Gates (A3, A25–A28); Engineering facts for gates, phones and hardened kit (A13, A17–A19); confirm costs from the bill of materials (A31, A36).

## 7. Editing conventions

- Every variable figure traces to an A-number. Do not remove a label until the assumption is confirmed.
- Footer on every content slide: "STYL · Atlantic UWB go-to-market vX.Y · Preliminary, internal · NN". Change the version in every footer when you bump it.
- Versioning: v0.x while preliminary. v1.0 when management approves the price basis and the five decisions.
- File naming: `<name>_vX.Y_YYYY-MM-DD`. Deck title `Atlantic_UWB_GTM_Plan_vX.Y_YYYY-MM-DD`; this file `Atlantic_UWB_GTM_CONTEXT_vX.Y_YYYY-MM-DD.md`.
- Slide text follows STE: short sentences, active voice, numbers with units, no jargon. Quoted sales lines can be natural speech.

---

## 8. Version history

| Version | Date | By | Changes |
|---|---|---|---|
| v0.1 | 6 Oct 2026 | JC | First deck built from the proposal document: plan, segments, prices, costs, examples, open questions |
| v0.2 | 6 Oct 2026 | JC | Reorganised into 8 sections with divider slides: strategy, segments, framework, prices, costs, examples, margins and ROI, to finalise |
| v0.3 | 6 Oct 2026 | JC | Refactored from JC's red comments on the .pptx. Added ROI and breakeven per segment, ROI by business model (platform, hardware sale, HaaS Hardware, HaaS All-in), subscription costing, assumptions A33–A50 with status colours, and 11 open items |
| v0.4 | 7 Oct 2026 | JC | Added the executive summary slide (slide 2): eight-section agenda, headline numbers, pointer to the five decisions |
| v0.5 | 7 Oct 2026 | JC | Added version, date and owner (JC) to the cover and all footers. Added this context file. Replaced bold tags the slide editor rejects, so all slides can be edited in the browser |
| v0.6 | 7 Oct 2026 | JC | Removed "For the CEO and Sales Director" from the cover; cover now shows owner, version and date only |
| v0.7 | 7 Oct 2026 | JC | File naming convention added: deck title and this context file now include version and date (`_v0.7_2026-10-07`) |
| v0.8 | 7 Oct 2026 | JC | Applied JC's assumption inputs. A7: edge server one installed price, $61.4K at 30% margin. A8: 10-man-day standard install package per site, then per man-day. A13: engineer-day at 50% margin. A24 and A18: about 150 cm is enough for most uses. Added A51–A52 and register page 6. Re-ran the model: pilots now $33–83K, year 1 $135K–1.83M, 3-year ROI 69–159%, HaaS All-in $22,430 a month; breakeven months unchanged. Updated the price, cost, margin, HaaS, segment, summary and open-items slides |
| v0.9 | 7 Oct 2026 | JC | Refactored on the Atlantic Product–Market–Customer Map. Added three slides: the 7 Atlantic products and which are priced here, the product × market matrix, and named accounts per market. Segments now follow the map markets, each tied to one product; manufacturing and industrial safety kept as later. Map won on conflicts, flagged in the register: healthcare on-prem Sovereign (A55, A56), LTA as transit lead (A57), ~10 cm capability (A18). Added A53–A57; 12 open items. Re-ran healthcare and transit: year 1 now $135K–1.73M, ROI 69–159%, gross margin 48–65% |
| v0.10 | 7 Oct 2026 | JC | Rebuilt on the CIO Office framework (Product Sheet Process Guide v1.0; Precision RTLS Ward sheet and brief v1.0). Every UWB product now has one price unit and three parts (software, hardware service, set-up), fixed-fee pilots, a 30% quote floor and 40% 24-month target, and the two-level discount rule. Ward prices taken from the CIO sheet; Operations, Flow and Gates prices proposed in the same structure. Currency changed to SGD. Hardware is now a monthly service; editions, edge-server sale, HaaS options and the 10-day install package retired. Added slides: framework, release status, host options, healthcare market and competitors, stress test, benchmark, cash, changes from v0.9. Register rebuilt (A1–A50) with source and confidence tags. Text rewritten in simplified English. New model model_v10.py: year 1 S$120K–1.22M, 3-yr ROI 39–227%, breakeven ~4 months after PO |
