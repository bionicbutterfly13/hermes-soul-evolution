# Phase 5: Specialist artifact acceptance - Research

**Method:** Existing research and dated audit reused; no new live test.
**Evidence:** docs/baseline-001.md (F06); .planning/research/SUMMARY.md.

## Findings and Constraints

- R-01: Historical delegation transport counts were enumerated, but the named Engineering acceptance probe timed out at 210 seconds, left no expected artifact and had no independent review.
- R-02: Completed or delivered status can falsely stand in for an artifact that actually meets the request.
- R-03: Specify the specialist packet and a later live acceptance probe with an actual artifact, checked criteria and required independent review. Preserve the historical timeout and absent artifact. Require returned error/unknown state to remain visible even if the envelope was delivered. Do not reinterpret the 26 transport records as an artifact-quality percentage.
- R-04: Quill must author the issue post from a cited evidence packet; actual dispatch access is currently blocked.
- R-05: Public examples use synthetic fixtures, explicit commands and retained verification; no private runtime data, unrun Colab claim or unsupported live result.

## Architectural Responsibility Map

| Component | Owner and responsibility |
|---|---|
| Public examples | This feature's examples/f06_acceptance/ directory; synthetic behavior only |
| Live runtime | Outside this repository; later scoped implementation after source inspection |
| Editorial draft | Actual Quill workflow; no coordinating-agent substitute |
| Claim review | Operator verifies provenance and public content before any push |

## Validation Architecture

Primary command: `python3 -m unittest discover -s examples/f06_acceptance -p 'test_*.py'`.

Failure cases: delivered envelope with missing artifact -> rejected_missing_artifact; existing artifact with failed criterion -> rejected_criteria; required independent review absent -> rejected_review; reviewer equals implementer -> rejected_review; all artifact/evidence/criteria/review checks pass -> accepted.

Examples/tests do not exist yet; the first example task creates them and runs meaningful behavior assertions before implementation. Protocol and source-packet documents require readback, local-link checks and claim/evidence review. Quill provenance and user attentiveness require actual external evidence, not mere field presence.

## Package Legitimacy Audit

No package installations are planned. Use the Python standard library. Audit any proposed new dependency before revising the plan.

## Uncertainty and Non-goals

Historical delegation transport counts were enumerated, but the named Engineering acceptance probe timed out at 210 seconds, left no expected artifact and had no independent review. No current-state improvement is inferred. Root-cause fixes, service starts, active memory writes and live personality installation remain outside this phase's public example implementation.
