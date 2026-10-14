# hanaML

hanaML is an independent AI lab in Los Angeles. We study what it takes to trust agents and small models with long,
consequential work, publish each paper with its code, and build on the results in our own products and in applied
work for clients. More at [hanaml.com](https://hanaml.com).

**Research areas:** rules and approvals for what agents may do; testing agents on long jobs; retrieval and grounding;
memory that people can read; training and serving models; small models on the device. Each is described, with its
projects, on [hanaml.com/research](https://hanaml.com/research).

## Papers

Each paper is a technical report with a PDF, a paper repo holding its reference implementation, and a companion
post. Within a research project, a later paper builds on the earlier ones.

| Date | Paper | Project | PDF | Code |
| --- | --- | --- | --- | --- |
| 2025-10-21 | [Distilling a frontier model into an 8B domain specialist](https://hanaml.com/research/papers/distilling-domain-agents) | [Model factory](https://hanaml.com/research/model-factory) | [PDF](https://hanaml.com/papers/distilling-domain-agents.pdf) | [distilling-domain-agents](https://github.com/hanaml-lab/distilling-domain-agents) |
| 2025-11-12 | [DRIFT: Drift-Bounded Distillation of One-Step Video Diffusion into Integer Recurrent Students](https://hanaml.com/research/papers/ondevice-video-sr) | [On-device video](https://hanaml.com/research/on-device-video) | [PDF](https://hanaml.com/papers/ondevice-video-sr.pdf) | [ondevice-video-sr](https://github.com/hanaml-lab/ondevice-video-sr) |
| 2025-12-09 | [The cost of reliability in long agent runs](https://hanaml.com/research/papers/cost-of-reliability-long-runs) | [Durable agents](https://hanaml.com/research/durable-agents) | [PDF](https://hanaml.com/papers/cost-of-reliability-long-runs.pdf) | [cost-of-reliability-long-runs](https://github.com/hanaml-lab/cost-of-reliability-long-runs) |
| 2026-01-20 | [Calibrating model judges against human labels](https://hanaml.com/research/papers/calibrating-llm-judges) | [Trustworthy evals](https://hanaml.com/research/trustworthy-evals) | [PDF](https://hanaml.com/papers/calibrating-llm-judges.pdf) | [calibrating-llm-judges](https://github.com/hanaml-lab/calibrating-llm-judges) |
| 2026-02-24 | [GATE: Gap-Adaptive Mixing of On-Policy Distillation and Verifiable Rewards for Small Domain Specialists](https://hanaml.com/research/papers/domain-distillation-rl) | [Model factory](https://hanaml.com/research/model-factory) | [PDF](https://hanaml.com/papers/domain-distillation-rl.pdf) | [domain-distillation-rl](https://github.com/hanaml-lab/domain-distillation-rl) |
| 2026-04-08 | [Bitemporal knowledge graphs as long-term memory for assistants](https://hanaml.com/research/papers/temporal-graphrag-memory) | [Grounded knowledge](https://hanaml.com/research/grounded-knowledge) | [PDF](https://hanaml.com/papers/temporal-graphrag-memory.pdf) | [temporal-graphrag-memory](https://github.com/hanaml-lab/temporal-graphrag-memory) |
| 2026-05-14 | [Knowing When to Submit: Calibrated Completion Verifiers for Budgeted Search over Coding and Terminal Agent Trajectories](https://hanaml.com/research/papers/verifier-search-agents) | [Durable agents](https://hanaml.com/research/durable-agents) | [PDF](https://hanaml.com/papers/verifier-search-agents.pdf) | [verifier-search-agents](https://github.com/hanaml-lab/verifier-search-agents) |
| 2026-07-08 | [Claim-level citation verification for agentic retrieval over financial filings](https://hanaml.com/research/papers/agentic-rag-citation-verification) | [Grounded knowledge](https://hanaml.com/research/grounded-knowledge) | [PDF](https://hanaml.com/papers/agentic-rag-citation-verification.pdf) | [agentic-rag-citation-verification](https://github.com/hanaml-lab/agentic-rag-citation-verification) |
| 2026-08-19 | [TIDE: Hazard-Scheduled, Budget-Constrained Memory Consolidation for Long-Horizon LLM Agents](https://hanaml.com/research/papers/agent-memory-consolidation) | [Grounded knowledge](https://hanaml.com/research/grounded-knowledge) | [PDF](https://hanaml.com/papers/agent-memory-consolidation.pdf) | [agent-memory-consolidation](https://github.com/hanaml-lab/agent-memory-consolidation) |
| 2026-10-07 | [Verifier Perturbation Testing: Trace-Independent Detection of Reward Hacking in RL-Trained Coding Agents](https://hanaml.com/research/papers/detecting-reward-hacking) | [Trustworthy evals](https://hanaml.com/research/trustworthy-evals) | [PDF](https://hanaml.com/papers/detecting-reward-hacking.pdf) | [detecting-reward-hacking](https://github.com/hanaml-lab/detecting-reward-hacking) |

## System repos

The lab's infrastructure. Each system repo serves one research project, carries its methods into code that runs
offline in CI, and says in its README which results it reproduces and which it only reports.

| Repo | Project | What it is |
| --- | --- | --- |
| [hana-agents](https://github.com/hanaml-lab/hana-agents) | [Durable agents](https://hanaml.com/research/durable-agents) | A durable runtime for long agent jobs: journalled replay with idempotent tool calls, Cedar policies at the tool boundary with argument provenance, TLA+-checked approval rules, and a browser task environment. |
| [hana-evals](https://github.com/hanaml-lab/hana-evals) | [Trustworthy evals](https://hanaml.com/research/trustworthy-evals) | Evaluation of long, multi-stage jobs: check placement, pass^k, verifier perturbation testing, and model judges calibrated against human labels. |
| [hana-knowledge](https://github.com/hanaml-lab/hana-knowledge) | [Grounded knowledge](https://hanaml.com/research/grounded-knowledge) | Grounded answers over documents: hybrid retrieval with cited spans, bitemporal graph memory, memory consolidation, and claim-level citation checks. |
| [hana-models](https://github.com/hanaml-lab/hana-models) | [Model factory](https://hanaml.com/research/model-factory) | The model factory: distil and post-train small domain models, run them on the device, and measure serving cost and latency. |
| [vsr-mobile](https://github.com/hanaml-lab/vsr-mobile) | [On-device video](https://hanaml.com/research/on-device-video) | Causal video super-resolution, 270p to 1080p, with exports and a playback pipeline for phones and edge boards. |
| [agentic-index](https://github.com/hanaml-lab/agentic-index) | [Benchmarks](https://hanaml.com/benchmarks) | The method and scoring code of the hanaML Agentic Index, which ranks frontier models on agentic work from Artificial Analysis' data, fetched at run time with your own API key. |

## Models

| Model | What it does | Repo |
| --- | --- | --- |
| [llama-toolcall-guard-1b](https://hanaml.com/models/llama-toolcall-guard-1b) | Screens a proposed tool call before an agent runs it: allow, ask or block. | hana-agents |
| [judge-7b](https://hanaml.com/models/judge-7b) | Judges pairs of answers against a rubric, trained to ignore order and length, with calibrated scores. | hana-evals |
| [rerank-m](https://hanaml.com/models/rerank-m) | Reranks retrieved passages for a question; runs on a laptop CPU. | hana-knowledge |
| [llama-cite-verify-3b](https://hanaml.com/models/llama-cite-verify-3b) | Checks that a cited passage supports a claim, and quotes the deciding words. | hana-knowledge |
| [clause-extract-8b](https://hanaml.com/models/clause-extract-8b) | Extracts clauses and fields from contracts and claims as schema-valid JSON with source spans. | hana-models |
| [ondevice-summarise-1b](https://hanaml.com/models/ondevice-summarise-1b) | Summarises notes and messages on a phone or a laptop, trained with 4-bit quantisation in the loop. | hana-models |
| [vsr-lite](https://hanaml.com/models/vsr-lite) | Upscales video 4x on a streaming device without flicker; 1.9M parameters. | vsr-mobile |

## How to cite

Every repo has a `CITATION.cff`; GitHub's "Cite this repository" button gives APA and BibTeX from it. Each paper's
page on [hanaml.com/research](https://hanaml.com/research) gives its BibTeX, in this form:

```bibtex
@techreport{agarwal2026tide,
  author      = {Agarwal, Manav},
  title       = {{TIDE}: Hazard-Scheduled, Budget-Constrained Memory Consolidation for Long-Horizon {LLM} Agents},
  institution = {hanaML},
  type        = {Technical report},
  year        = {2026},
  url         = {https://hanaml.com/research/papers/agent-memory-consolidation}
}
```

## Contributing and contact

Issues and pull requests are welcome on every repo; each has a `CONTRIBUTING.md`. Please report security issues
privately, as our [security policy](https://github.com/hanaml-lab/.github/blob/main/SECURITY.md) describes. For
research collaboration, consulting or a pilot, write to [info@hanaml.com](mailto:info@hanaml.com) or see
[hanaml.com/contact](https://hanaml.com/contact).
