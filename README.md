# Michael Jennings

Former FBI senior intelligence analyst and supervisor (24 years). Now building data tools through AI-assisted development.
Houston, Texas · [LinkedIn](https://linkedin.com/in/jenningsmt) · [mikejennings.dev](https://mikejennings.dev)

## What this is

I spent my career turning large, messy, multi-source data into decisions for investigators, prosecutors, and senior leaders. In 2026 I started building the tools myself.

I direct AI coding assistants (Claude and GPT-family models) to write the code. I own the problem definition, the data model, the architecture, verification, and every release decision. These projects use the Elite Dangerous exploration community's open galaxy data as a live sandbox: a 100+ GB dataset covering more than 200 million star systems, with real users and no sensitive data.

## How I work with AI

- **Specification first.** Requirements and design notes are written before any code is generated.
- **Guardrails.** Documented architecture rules that every assistant has to follow.
- **Independent review.** Code from one model is reviewed adversarially by another, then by me, and checked by tests before it is released.
- **Validate against authoritative sources.** Outputs are confirmed against external data, never accepted on a model's say-so.
- **Human in the loop by design.** I piloted an autonomous multi-agent workflow, measured its real coordination and verification costs, and went back to a tighter human-in-the-loop model.
- **Lessons learned.** A written record of what went wrong and what changed because of it.

## Projects, and the analytic problem behind each

| Project | What it does | Analytic pattern |
|---|---|---|
| [Monops: Entity Screening Toolkit](https://github.com/jenningsmt/entity-screening-toolkit) | Screens researchers and organizations for foreign affiliations by reconciling declared ties against open sanctions, corporate ownership, grant, and bibliometric data, with explainable scoring and an analyst reviewing every match. [Live demo](https://mikejennings.dev) | Entity resolution and due-diligence screening (research security / KYC) |
| [ED Sector Surveyor](https://github.com/jenningsmt/ed-sector-surveyor) | Streams a 113 GB compressed dataset into per-sector SQLite databases, infers likely-but-unrecorded systems from naming-pattern gaps, and keeps only candidates an external catalog confirms are new | Large-scale streaming ETL; generate-then-validate lead generation against an authoritative source |
| [ED Colony Scout](https://github.com/jenningsmt/ed-colony-scout) | Ranks targets with an editable scoring rubric and tests reachability as multi-hop jump chains | Explainable, adjustable scoring; network reachability analysis |
| [ED Expedition Ledger](https://github.com/jenningsmt/ed-expedition-ledger) | Ingests live event logs into SQLite with hash-based de-duplication and exports per-leg Excel and CSV reports | Idempotent, auditable ingestion; structured reporting from raw event data |
| [Ring Density Monitor](https://github.com/jenningsmt/ring-density-monitor) | Compares each new observation to a population baseline in real time and flags outliers | Real-time monitoring and anomaly flagging |

## Stack

Python · SQLite · Tkinter · PyInstaller / Inno Setup · GitHub Actions · unittest / pytest · Excel and Power BI for analysis

<sub>The Elite Dangerous tools are unofficial fan projects, not affiliated with Frontier Developments.</sub>
