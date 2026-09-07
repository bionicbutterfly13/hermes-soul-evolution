# Blog series source plan

## Authority and sequence

Dr. Mani requested a public record of the motivation, research, decisions, potential pitfalls, code and examples behind Hermes Soul Evolution. Quill owns all blog drafting and revision, including the eventual titles. This file is an operational source plan, not article prose.

The next step is to compare researched approaches and settle the initial design, then revise the personality. Runtime repairs are deferred. Each issue F02-F07 has a requested blog post and GSD feature stream; the actual GSD workflow must create those streams before they are reported as initialized.

## Opening source packets

| Packet | Material to provide Quill | Evidence requirement |
| --- | --- | --- |
| Motivation | Daily organization, reliable delegation, bounded overnight work, useful reflection and relationship continuity; the selected executive-operator tone | Use the user's stated aims. Do not invent personal history, feelings or outcomes. |
| Research | Inspectable SOUL examples, practitioner reports, memory and reflection research; reasons an approach may or may not fit | Direct outbound citations, source dates, commercial interests and limits. Begin with the [baseline references](baseline-001.md#research-references). |
| Decisions | Options considered, the chosen initial design, rejected alternatives and what would change the decision | Record an actual decision before presenting it as settled. Preserve the user's corrections. |

## One post and feature stream per issue

F01 is a positive baseline loading check. The six issues below retain the finding IDs from [Baseline 001](baseline-001.md).

| Finding | Issue-specific post subject | Example or experiment to develop | Present state |
| --- | --- | --- | --- |
| F02 | A registered scheduler that produces no report | A minimal scheduled task with an artifact, timestamp and visible failure record; distinguish registration from execution | Startup failure observed; cause undiagnosed; GSD feature setup pending |
| F03 | Daily routines with stale execution evidence | A freshness check that distinguishes an old successful run from current operation | Stale evidence recorded; GSD feature setup pending |
| F04 | Overnight preparation versus useful overnight work | One bounded task with a finite budget, recoverable failure and an artifact; later compare source-linked reflection with the outcome | Preparation-only adapter inspected; execution experiment not run; GSD feature setup pending |
| F05 | Memory service health versus continuity in the agent | Recover an earlier decision and its correction in a fresh profile session and scheduled run | Historical recall errors; current agent-level continuity unverified; GSD feature setup pending |
| F06 | Delivered results versus accepted specialist work | Check a returned artifact against explicit acceptance criteria, including a missing-artifact case | Historical acceptance probe failed; GSD feature setup pending |
| F07 | Relationship continuity as observable behavior | Interrupt a task, change a priority, correct a fact and return in a fresh session; assess follow-through and user experience | Instruction gap identified; user trial not run; GSD feature setup pending |

These are proposed experiment designs, not implementation or test results. Runtime repair is not a prerequisite for reviewing the options or revising the persona.

## Requirements for every post's source packet

- Motivation and the specific question being investigated.
- Dated evidence, its origin and its limits, including failures and contrary results.
- Options considered and the actual decision, with its reason.
- Potential pitfalls grounded in the observed problem or cited research.
- Links to relevant source documentation and code. Pin code links to a commit when reproducibility depends on the version.
- Exact verification method, observed results, unresolved questions and the next experiment.
- The user's actual reaction, verbatim when supplied; no invented first-person account.
- Quill draft status and the eventual published URL, once each exists.

## Code and Google Colab

No runnable project examples or Google Colab notebooks have been published or executed for this baseline.

Add a code example only with its input, expected behavior, run command, environment requirements and observed test result. Mark examples that use synthetic data explicitly; a local demonstration does not prove live Hermes reliability.

If an experiment is actually run in Google Colab, add the committed notebook, a working Colab link and a record of the execution date, runtime dependencies and observed output. Until then, keep Colab listed as a possible experiment environment and do not add a placeholder badge or success claim.

## Publication status

This initial repository contains research documentation and source packets. Blog drafts, issue feature setup, code examples and Colab experiments remain pending their respective workflows.
