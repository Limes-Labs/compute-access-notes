# Compute Access Notes

> Research log for [Limes Labs](https://limeslabs.eu). Last updated: June 2026.

We are **not claiming access**. We are recording what we learn while pursuing legitimate paths for open European AI training.

---

## Summary (June 2026)

| Path | Fit for Limes | Status |
| --- | --- | --- |
| EuroHPC AI Factory **Playground** | Experiments, contributor onboarding | Theoretical — need eligible entity |
| **Fast Lane** (≤50k GPUh) | Fine-tune 7B-class open models | Researching application requirements |
| **Large Scale** (>50k GPUh) | Pretrain / large fine-tune | Long shot without industry partner |
| **IT4LIA TRY/Medium** | Italian/EU consortium path via CINECA | Outreach planned |
| **LUMI AI Factory** | Nordic/Baltic open-model precedent (Tilde) | Reference case, not Limes-specific |
| Laptop / MPS | limes-nanogpt char runs | **Working** |
| Commercial EU GPU (Scaleway, etc.) | Paid fallback | Document when budget exists |

---

## EuroHPC access mechanics

**Portal:** https://access.eurohpc-ju.europa.eu/

**Eligible users (per Access Policy Apr 2025):**
- Public and private users in **EU Member States**
- Users in countries **associated to DEP or Horizon Europe**
- Industrial innovation large-scale: emphasis on **industry** applicants (startups/SMEs)

**2025–2026 reality:** AI Factories initially use **existing** EuroHPC systems (LUMI, Leonardo, MN5, MeluXina, etc.) while AI-optimised partitions (LISA, new IT4LIA system, etc.) roll out.

**Partition availability:** Large Scale docs note Leonardo & MareNostrum 5 may be **unavailable** at times due to demand — applications should name fallback partitions.

---

## IT4LIA notes

- Services operational since **April 2025**
- Packages: TRY / Medium / Large — include GPU hours + support + training
- Eligible: startups, SMEs, PA, academia — **no-cost** tiers for eligible actors
- New **€290M** AI system contract (E4 + Dell), Apr 2026
- **LISA** on Leonardo: first AI-native EuroHPC partition (~650 PF mixed precision cited)

**Open questions for Limes:**
1. Can a loose contributor network apply via a **host university** (e.g. Italian, Slovenian, Austrian partners in IT4LIA consortium)?
2. Is char-level / educational open-source work compelling for TRY tier?
3. Who signs DPA / affiliation agreement?

**Contacts to use:**
- info-it4lia@cineca.it
- support-it4lia@cineca.it
- Form: https://forms.office.com/e/swchU8P4C5

---

## Precedents worth citing

| Project | Compute | Lesson |
| --- | --- | --- |
| **TildeOpen 30B** | 2M GPU hours on LUMI | SME + EuroHPC factory can ship open weights |
| **OpenEuroLLM** | BSC, SURF, consortium | EU-funded multilingual open stack |
| **nanoGPT / nanochat** | Consumer → cloud | Start tiny, document configs, scale with receipts |

---

## Limes nanogpt → factory narrative

**Phase 0 (now):** char-level on laptop; publish configs, losses, samples  
**Phase 1:** BPE tokenizer + multilingual shards; eurobench perplexity tasks  
**Phase 2:** 7B fine-tune proposal with public eval plan + model card  
**Phase 3:** Fast Lane or IT4LIA Medium for fine-tune; Large Scale only with partners  

Artifacts required before serious outreach:
- [x] Public GitHub trainer ([limes-nanogpt](https://github.com/Limes-Labs/limes-nanogpt))
- [x] Constitution + eval rubric ([limes-constitution](https://github.com/Limes-Labs/limes-constitution))
- [ ] Reproducible benchmark numbers on [eurobench](https://github.com/Limes-Labs/eurobench)
- [ ] Model card from [template](https://github.com/Limes-Labs/model-card-template)
- [ ] Legal entity or university MOU

---

## Contact log

| Date | Org | Channel | Question | Response | Next step |
| --- | --- | --- | --- | --- | --- |
| — | EuroHPC helpdesk | — | Eligibility for unincorporated open-source collective | *pending* | Send after entity/partner identified |
| — | IT4LIA | form | TRY package for open-weight European LM benchmark project | *pending* | Draft 1-pager + link eurobench |

*We will publish rows as contacts happen — no fabricated progress.*

---

## References

- EuroHPC Access Policy (Apr 2025 PDF)
- Large Scale AI Factory Access page (rolling cut-offs 2026–2027)
- IT4LIA FAQ (Dec 2025)
- EC — Europe's Open-Source AI Landscape report (Dec 2025)
- Limes [infrastructure map](https://github.com/Limes-Labs/european-ai-infrastructure-map/blob/main/MAP.md)

## Contribute

Add sourced notes via PR or issue. Join: https://limeslabs.eu/join