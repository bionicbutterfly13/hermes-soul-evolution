# Research synthesis for feature planning

**Status:** Existing research reused, not a new search or a live test.
**Sources:** docs/baseline-001.md, docs/series-plan.md and docs/research/runtime-personality.md.

## Stack and responsibility

This repository is documentation and reproducible synthetic experiments. Markdown, Python standard-library unittest and JSON fixtures are sufficient for the planned examples. GSD provides project/phase planning; Quill owns editorial prose. The live Hermes installation is outside this public repository.

## Feature implications

- F02 needs a concrete success artifact and failure state; launchd registration alone proved neither.
- F03 needs timestamps and runner state interpreted together, with a single active owner for each routine.
- F04 needs a finite task budget, artifact acceptance and source-linked reflection; the inspected adapter permits preparation only.
- F05 needs correct-bank recovery of a changed fact in fresh and scheduled sessions; service health and missing profile config are individually insufficient.
- F06 needs artifact and acceptance evidence independent from transport completion.
- F07 needs continuity behaviors and user assessment, plus a controlled comparison of the actual three client conditions.

## Dependencies

The public synthetic examples can proceed independently. Live F03 scheduling reconciliation depends on the F02 ownership/acceptance contract. Live F04 integrated overnight trials depend on F02 scheduling, F05 memory and F06 artifact acceptance. F05's scheduled leg depends on F02. F07's initial design discussion has no runtime repair dependency.

## Pitfalls

Avoid treating operator observations as platform-wide findings, transport status as acceptance, memory-service health as agent continuity, fluent reflection as changed later behavior, and model labels as proof of matched runtime inputs. Preserve failure evidence and unknowns. Never let a checked-in experiment protocol imply the experiment ran.

## Source-linked design evidence

- [Claudia seeded SOUL at inspected revision](https://github.com/kbanc85/claudia-autonomous/blob/177236207991ed7ccec6de16a9458ecdcf9c1b3f/claudia_cli/default_soul.py): inspectable instructions; not validated daily autonomy.
- [Felix first-person interview](https://www.bankless.com/podcast/building-a-million-dollar-zero-human-company-with-openclaw-nat-eliason): nightly review and delegation experience; commercially interested account.
- [Lex's six-month account](https://notesbylex.com/6-months-of-openclaw): individual routine experience, not benchmark evidence.
- [Hermes delegation](https://hermes-agent.nousresearch.com/docs/user-guide/features/delegation/): reference semantics; installed behavior still needs verification.
- [Generative Agents](https://arxiv.org/html/2304.03442v2): source-linked reflection research in a simulated setting.
- [LongMemEval](https://arxiv.org/html/2410.10813v2): changed information, retrieval and abstention; not complete executive reliability.

## Package Legitimacy Audit

No package-manager installation tasks. Planned Python examples use the standard library. Adding a dependency requires a fresh legitimacy audit before any install plan.

## Validation Architecture

Use standard-library unittest for concrete fixture behavior, including failure cases. Use GSD frontmatter/structure/decision-coverage checks for plans. Validate local Markdown links and public-content exclusions before pushing. Human judgments of attentiveness and actual Quill authorship cannot be proven by a string-presence check.

## Unknowns retained

The scheduler's exact startup cause, current agent-level continuity and a successful specialist acceptance trial remain unverified. Initial behavior selection is in progress. Quill dispatch is blocked by access to its actual workflow. No comparative model test or Colab run is claimed.
