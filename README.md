# AI Industry Research Agent

Source-grounded industry intelligence · Structured extraction · Human-reviewed research

> **Status: early-stage workflow design.** This public repository currently documents the proposed research process. It does not yet contain an executable agent, automated retrieval pipeline, or validated performance results.

## Purpose

Design a research assistant that turns a scoped question about the AI industry into a traceable briefing. Intended topics include model releases, enterprise adoption, infrastructure, commercial partnerships, and AI governance. The emphasis is on evidence quality and reviewable reasoning.

## Proposed workflow

**Scope → retrieve → extract → cross-check → draft → human review.**

Industry information retrieval starts with a question, date range, geography, and inclusion criteria. The planned retrieval layer prioritizes company announcements, technical documentation, research papers, regulatory publications, and original reporting, while recording publication and event dates separately.

Structured extraction converts each relevant source into consistent fields: organization, event, date, product or technology, commercial significance, source URL, supporting passage, and unresolved questions. Observed facts, source claims, and analyst interpretations remain distinct.

Source cross-verification compares independent evidence for material claims, flags conflicting dates or figures, and identifies when multiple articles repeat the same original announcement. Uncorroborated claims remain explicitly labeled.

Report generation organizes findings into an executive brief, evidence-backed developments, implications, open questions, and references. Each material claim should link to its supporting source.

Human verification is a required publication gate: the reviewer opens cited sources, checks quotations and numerical claims, resolves or documents conflicts, and approves the final report. Generated text is a draft until reviewed.

## Delivery status

| Stage | Current scope |
| --- | --- |
| Implemented | This repository-level project brief, proposed evidence fields, and human-review requirements. |
| In development | Workflow specification and acceptance criteria; software implementation has not been published. |
| Planned | Retrieval connectors, extraction schemas, claim-to-source tracking, report templates, and evaluation fixtures. |

## Evaluation plan

Use a fixed set of research questions and a manually reviewed reference set. Track citation validity, claim support, extraction accuracy, coverage of relevant events, handling of conflicting evidence, latency, and cost. Record model, prompt version, retrieval date, and reviewer corrections. No benchmark scores are claimed at this stage.

## Next milestones

Publish a small source-backed sample briefing with a review record; define a machine-readable extraction schema; implement one bounded retrieval-to-draft path; evaluate it against the reference set before expanding coverage.

## Limitations and responsible use

Public sources can be incomplete, stale, or mutually dependent. Cross-checking supports review but does not guarantee truth. Respect source access conditions and copyright, keep credentials out of the repository, and avoid ingesting confidential materials. Outputs are research drafts, not legal or investment advice.

## Portfolio context

An independent project exploring information retrieval, evidence management, prompt and workflow design, and human oversight. The documented design describes intended behavior; runnable capabilities will be marked implemented only when their code and verification evidence are published.
