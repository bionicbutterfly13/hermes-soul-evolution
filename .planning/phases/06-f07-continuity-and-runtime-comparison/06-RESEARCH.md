# Phase 6: Continuity and runtime comparison - Research

**Method:** Existing research and dated audit reused; no new live test.
**Evidence:** docs/baseline-001.md (F07); .planning/research/SUMMARY.md; docs/research/runtime-personality.md.

## Findings and Constraints

- R-01: The SOUL instruction gap is an interpretation, not a causal diagnosis. The user chose executive-operator tone and Claudia-first review; no matched runtime experiment has run.
- R-02: A warmer paragraph, one output, or a shared model label can be mistaken for continuity or a platform personality effect.
- R-03: Record candidate behaviors in order: Claudia first, then selective Felix ownership/follow-through, with Lex as a routine reference. Preserve the exact executive-operator wording. Use adopted/rejected/pending columns with decision provenance, and do not manufacture a finalized SOUL. Define an interruption/correction/priority-change fresh-session trial and a seven-day observation protocol; user attentiveness ratings and operational evidence stay separate. No active SOUL edits.
- R-04: Quill must author the issue post from a cited evidence packet; actual dispatch access is currently blocked.
- R-05: Public examples use synthetic fixtures, explicit commands and retained verification; no private runtime data, unrun Colab claim or unsupported live result.

## Architectural Responsibility Map

| Component | Owner and responsibility |
|---|---|
| Public examples | This feature's examples/f07_continuity/ directory; synthetic behavior only |
| Live runtime | Outside this repository; later scoped implementation after source inspection |
| Editorial draft | Actual Quill workflow; no coordinating-agent substitute |
| Claim review | Operator verifies provenance and public content before any push |

## Validation Architecture

Primary command: `python3 -m unittest discover -s examples/f07_continuity -p 'test_*.py'`.

Failure cases: interrupted commitment resumes with supported commitment ID; changed priority uses the newest user instruction; corrected fact excludes superseded value; absent relevant history yields explicit unknown; unsupported familiarity or promised completion is flagged. Score observable evidence only; leave attentiveness for the user's actual rating.

Examples/tests do not exist yet; the first example task creates them and runs meaningful behavior assertions before implementation. Protocol and source-packet documents require readback, local-link checks and claim/evidence review. Quill provenance and user attentiveness require actual external evidence, not mere field presence.

## Package Legitimacy Audit

No package installations are planned. Use the Python standard library. Audit any proposed new dependency before revising the plan.

## Uncertainty and Non-goals

Additional comparisons pending: Dr. Mani's Second Mind decision-as-object architecture, Assaf Magen's The Personal AI Operating System and two Tiago Forte videos. No findings or adopted changes from those comparisons are asserted. The exact selected Claudia article title is recorded as D-11 in CONTEXT.md; a title is not evidence of an unrecorded adoption decision.

The SOUL instruction gap is an interpretation, not a causal diagnosis. The user chose executive-operator tone and Claudia-first review; no matched runtime experiment has run. No current-state improvement is inferred. Root-cause fixes, service starts, active memory writes and live personality installation remain outside this phase's public example implementation.
