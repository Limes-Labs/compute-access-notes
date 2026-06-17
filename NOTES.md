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

**Primary source URLs:** access modes https://www.eurohpc-ju.europa.eu/ai-factories/ai-factories-access-modes_en, access calls https://www.eurohpc-ju.europa.eu/ai-factories/ai-factories-access-calls_en, Industrial Innovation Terms of Reference https://www.eurohpc-ju.europa.eu/document/download/bd7aa666-bdf3-4436-b5ec-0b34a781e817_en?filename=Terms+of+Reference+-+AIF+Access+Calls.pdf

**Eligible users (per Access Policy Apr 2025):**
- Public and private users in **EU Member States**
- Users in countries **associated to DEP or Horizon Europe**
- Industrial innovation large-scale: emphasis on **industry** applicants (startups/SMEs)

**2025–2026 reality:** AI Factories initially use **existing** EuroHPC systems (LUMI, Leonardo, MN5, MeluXina, etc.) while AI-optimised partitions (LISA, new IT4LIA system, etc.) roll out.

**Partition availability:** Large Scale docs note Leonardo & MareNostrum 5 may be **unavailable** at times due to demand — applications should name fallback partitions.

---

## IT4LIA notes

**Primary source URLs:** homepage https://it4lia-aifactory.eu/, packages https://it4lia-aifactory.eu/what-we-can-do-for-you/, FAQ https://it4lia-aifactory.eu/faq/, contact https://it4lia-aifactory.eu/contact-us/, infrastructure https://it4lia-aifactory.eu/about-it4lia/hpc-technological-infrastructure/

- Services operational since **April 2025**
- Packages: TRY / Medium / Large — include GPU hours + support + training
- Eligible: startups, SMEs, PA, academia — **no-cost** tiers for eligible actors
- New **€290M** AI system contract (E4 + Dell), Apr 2026
- **LISA** on Leonardo: first AI-native EuroHPC partition (~650 PF mixed precision cited)

**Open questions for Limes:**
1. Can a loose contributor network apply via a **host university** (e.g. Italian, Slovenian, Austrian partners in IT4LIA consortium)?
2. Is char-level / educational open-source work compelling for TRY tier?
3. Who signs DPA / affiliation agreement?

**Contacts to use (public IT4LIA contact page):**
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

## Contact log policy

Contacts must be logged only after they happen. Planned messages belong in draft sections, not in the contact log. See [GUIDE.md](GUIDE.md#no-fabricated-progress-contact-log-policy).

## Actual contact log

| Date | Org | Channel | Question | Response | Next step |
| --- | --- | --- | --- | --- | --- |
| — | — | — | — | — | No contacts logged yet |

## Draft questions, not yet sent

| Org | Channel | Draft question | Missing before sending |
| --- | --- | --- | --- |
| EuroHPC helpdesk | Helpdesk form | Eligibility for unincorporated open-source collective | Eligible entity or partner candidate |
| IT4LIA | Consultation form or support email | TRY package fit for open-weight European LM benchmark project | Draft 1-pager, compute estimate, eurobench links |

---

## References

- Compute Access Starter Kit: [docs/compute-access-starter-kit.md](docs/compute-access-starter-kit.md)
- Eligibility matrix: [docs/eurohpc-eligibility-matrix.md](docs/eurohpc-eligibility-matrix.md)
- Application path guide: [docs/application-path-guide.md](docs/application-path-guide.md)
- Source register: [data/sources.csv](data/sources.csv)
- Contact log: [data/contact-log.csv](data/contact-log.csv)
- EuroHPC Access Policy: https://www.eurohpc-ju.europa.eu/document/download/30614065-6dd6-4206-8065-fc97948e5e2c_en?filename=EuroHPC+JU+Access+Policy+-+Version+2025.12.pdf
- EuroHPC AI Factories access calls: https://www.eurohpc-ju.europa.eu/ai-factories/ai-factories-access-calls_en
- EuroHPC AI Factories access modes: https://www.eurohpc-ju.europa.eu/ai-factories/ai-factories-access-modes_en
- EuroHPC Industrial Innovation Terms of Reference: https://www.eurohpc-ju.europa.eu/document/download/bd7aa666-bdf3-4436-b5ec-0b34a781e817_en?filename=Terms+of+Reference+-+AIF+Access+Calls.pdf
- IT4LIA FAQ: https://it4lia-aifactory.eu/faq/
- IT4LIA packages: https://it4lia-aifactory.eu/what-we-can-do-for-you/
- EC — Europe's Open-Source AI Landscape report (Dec 2025)
- Limes [infrastructure map](https://github.com/Limes-Labs/european-ai-infrastructure-map/blob/main/MAP.md)

## Contribute

Add sourced notes via PR or issue. Join: https://limeslabs.eu/join
