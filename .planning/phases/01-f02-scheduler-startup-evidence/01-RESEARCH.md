# Phase 1: Scheduler startup evidence - Research

**Method:** Existing research and dated audit reused; no new live test.
**Evidence:** docs/baseline-001.md (F02); .planning/research/SUMMARY.md.

## Findings and Constraints

- R-01: The 7 September audit recorded EX_CONFIG, invocation counts and no proactive report files. The exact startup cause was not diagnosed.
- R-02: Registration or repeated invocations can be mistaken for successful scheduled output.
- R-03: Document a bounded read-only live diagnosis for the one dedicated scheduler: inspect its actual command, environment variable names only, working directory, permissions and dated failure evidence; stop at the current root-cause uncertainty. Define the proposed success proof as a scheduler-triggered artifact with matching run ID, expected report path and timestamps, plus visible failure status. Identify one scheduler owner. No restart or repair is run by this example.
- R-04: Quill must author the issue post from a cited evidence packet; actual dispatch access is currently blocked.
- R-05: Public examples use synthetic fixtures, explicit commands and retained verification; no private runtime data, unrun Colab claim or unsupported live result.

## Architectural Responsibility Map

| Component | Owner and responsibility |
|---|---|
| Public examples | This feature's examples/f02_scheduler/ directory; synthetic behavior only |
| Live runtime | Outside this repository; later scoped implementation after source inspection |
| Editorial draft | Actual Quill workflow; no coordinating-agent substitute |
| Claim review | Operator verifies provenance and public content before any push |

## Validation Architecture

Primary command: `python3 -m unittest discover -s examples/f02_scheduler -p 'test_*.py'`.

Failure cases: registration_only -> registered_only; invocation_without_artifact -> invoked_no_artifact; artifact_with_matching_run_id_and_timestamp -> succeeded; startup_exit_78 -> startup_failed. A success envelope without an existing matching artifact is not success.

Examples/tests do not exist yet; the first example task creates them and runs meaningful behavior assertions before implementation. Protocol and source-packet documents require readback, local-link checks and claim/evidence review. Quill provenance and user attentiveness require actual external evidence, not mere field presence.

## Package Legitimacy Audit

No package installations are planned. Use the Python standard library. Audit any proposed new dependency before revising the plan.

## Uncertainty and Non-goals

The 7 September audit recorded EX_CONFIG, invocation counts and no proactive report files. The exact startup cause was not diagnosed. No current-state improvement is inferred. Root-cause fixes, service starts, active memory writes and live personality installation remain outside this phase's public example implementation.
