# Phase 4: Memory continuity - Research

**Method:** Existing research and dated audit reused; no new live test.
**Evidence:** docs/baseline-001.md (F05); .planning/research/SUMMARY.md.

## Findings and Constraints

- R-01: Service health and connector reads succeeded during the dated audit; four latest explicit profile recall results from 2-4 September were errors. No fresh profile recall or retention trial ran.
- R-02: Healthy memory infrastructure and a readable file do not prove the agent retained or recovered the intended correction.
- R-03: Separate live checks for HTTP service health, actual profile recall, automatic session-end retention, bank selection, correction handling, fresh-session recovery and scheduled-session recovery. Use synthetic seeded data only in a separately authorized live test and define cleanup before seeding. F02 evidence gates the scheduled leg. Record legacy/shared/environment fallback as an unresolved configuration possibility; absent profile config is not a diagnosis.
- R-04: Quill must author the issue post from a cited evidence packet; actual dispatch access is currently blocked.
- R-05: Public examples use synthetic fixtures, explicit commands and retained verification; no private runtime data, unrun Colab claim or unsupported live result.

## Architectural Responsibility Map

| Component | Owner and responsibility |
|---|---|
| Public examples | This feature's examples/f05_memory/ directory; synthetic behavior only |
| Live runtime | Outside this repository; later scoped implementation after source inspection |
| Editorial draft | Actual Quill workflow; no coordinating-agent substitute |
| Claim review | Operator verifies provenance and public content before any push |

## Validation Architecture

Primary command: `python3 -m unittest discover -s examples/f05_memory -p 'test_*.py'`.

Failure cases: older fact then explicit correction -> latest supported fact and source IDs; different bank -> abstain; new process loading saved synthetic facts -> corrected fact; no evidence -> abstain; future-dated evidence beyond as_of -> excluded. Never use an unrelated bank to fill a gap.

Examples/tests do not exist yet; the first example task creates them and runs meaningful behavior assertions before implementation. Protocol and source-packet documents require readback, local-link checks and claim/evidence review. Quill provenance and user attentiveness require actual external evidence, not mere field presence.

## Package Legitimacy Audit

No package installations are planned. Use the Python standard library. Audit any proposed new dependency before revising the plan.

## Uncertainty and Non-goals

Service health and connector reads succeeded during the dated audit; four latest explicit profile recall results from 2-4 September were errors. No fresh profile recall or retention trial ran. No current-state improvement is inferred. Root-cause fixes, service starts, active memory writes and live personality installation remain outside this phase's public example implementation.
