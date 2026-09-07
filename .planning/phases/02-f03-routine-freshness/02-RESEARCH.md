# Phase 2: Routine freshness - Research

**Method:** Existing research and dated audit reused; no new live test.
**Evidence:** docs/baseline-001.md (F03); .planning/research/SUMMARY.md.

## Findings and Constraints

- R-01: The 7 September audit inspected all five legacy definitions; three enabled jobs had old runs/next-run dates, and a 2 September journal existed. None of this proves current operation.
- R-02: An old successful journal and a stale next-run field can mask a stopped scheduling path.
- R-03: Define one routine owner for the morning summary and one for daily reflection, inventorying dedicated versus legacy scheduling candidates without selecting an unverified live winner. Require F02 ownership and acceptance evidence before later scheduling reconciliation. Specify duplicate-owner detection, current runner evidence, last success age and next-run consistency. Preserve the dated historical journal as historical evidence.
- R-04: Quill must author the issue post from a cited evidence packet; actual dispatch access is currently blocked.
- R-05: Public examples use synthetic fixtures, explicit commands and retained verification; no private runtime data, unrun Colab claim or unsupported live result.

## Architectural Responsibility Map

| Component | Owner and responsibility |
|---|---|
| Public examples | This feature's examples/f03_freshness/ directory; synthetic behavior only |
| Live runtime | Outside this repository; later scoped implementation after source inspection |
| Editorial draft | Actual Quill workflow; no coordinating-agent substitute |
| Claim review | Operator verifies provenance and public content before any push |

## Validation Architecture

Primary command: `python3 -m unittest discover -s examples/f03_freshness -p 'test_*.py'`.

Failure cases: stopped runner -> stopped; no last success -> no_history; overdue next run while running -> overdue; old success beyond max_age_seconds -> stale; recent success with future next run -> current. Reject naive timestamps, require a fixed now fixture and document status precedence.

Examples/tests do not exist yet; the first example task creates them and runs meaningful behavior assertions before implementation. Protocol and source-packet documents require readback, local-link checks and claim/evidence review. Quill provenance and user attentiveness require actual external evidence, not mere field presence.

## Package Legitimacy Audit

No package installations are planned. Use the Python standard library. Audit any proposed new dependency before revising the plan.

## Uncertainty and Non-goals

The 7 September audit inspected all five legacy definitions; three enabled jobs had old runs/next-run dates, and a 2 September journal existed. None of this proves current operation. No current-state improvement is inferred. Root-cause fixes, service starts, active memory writes and live personality installation remain outside this phase's public example implementation.
