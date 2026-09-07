# Phase 3: Bounded overnight work and reflection - Research

**Method:** Existing research and dated audit reused; no new live test.
**Evidence:** docs/baseline-001.md (F04); .planning/research/SUMMARY.md.

## Findings and Constraints

- R-01: The inspected adapter ranked at most 25 open cards and forbade worker dispatch, project edits and memory updates. Startup repair alone would still produce preparation only.
- R-02: A preparation report can be presented as overnight work, while fluent reflection can be mistaken for improved behavior.
- R-03: Define an integrated overnight trial for one explicitly assigned task with finite limits, a source snapshot, expected artifact, independent acceptance and recoverable failure record. Require F02 scheduled execution, F05 correct-bank fresh/scheduled continuity and F06 artifact acceptance before a later live trial. State that the inspected adapter prepares priorities/decisions/limitations and grants none of these execution capabilities.
- R-04: Quill must author the issue post from a cited evidence packet; actual dispatch access is currently blocked.
- R-05: Public examples use synthetic fixtures, explicit commands and retained verification; no private runtime data, unrun Colab claim or unsupported live result.

## Architectural Responsibility Map

| Component | Owner and responsibility |
|---|---|
| Public examples | This feature's examples/f04_overnight/ directory; synthetic behavior only |
| Live runtime | Outside this repository; later scoped implementation after source inspection |
| Editorial draft | Actual Quill workflow; no coordinating-agent substitute |
| Claim review | Operator verifies provenance and public content before any push |

## Validation Architecture

Primary command: `python3 -m unittest discover -s examples/f04_overnight -p 'test_*.py'`.

Failure cases: one assigned task with finite attempt/time budgets -> running; existing artifact satisfying acceptance and review -> accepted; exceeded budget -> timed_out; interrupted child with no trustworthy outcome -> unknown; unknown -> explicit recovery_decision. Do not auto-resume or mark an unknown task complete.

Examples/tests do not exist yet; the first example task creates them and runs meaningful behavior assertions before implementation. Protocol and source-packet documents require readback, local-link checks and claim/evidence review. Quill provenance and user attentiveness require actual external evidence, not mere field presence.

## Package Legitimacy Audit

No package installations are planned. Use the Python standard library. Audit any proposed new dependency before revising the plan.

## Uncertainty and Non-goals

The inspected adapter ranked at most 25 open cards and forbade worker dispatch, project edits and memory updates. Startup repair alone would still produce preparation only. No current-state improvement is inferred. Root-cause fixes, service starts, active memory writes and live personality installation remain outside this phase's public example implementation.
