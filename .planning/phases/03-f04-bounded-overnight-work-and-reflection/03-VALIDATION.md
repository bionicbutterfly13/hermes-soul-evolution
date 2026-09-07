---
phase: 3
slug: f04-bounded-overnight-work-and-reflection
status: planned
nyquist_compliant: true
wave_0_complete: false
created: 2026-09-07
---

# Phase 3 validation strategy

## Test Infrastructure

Python standard-library unittest; no package installation.
Quick command: `python3 -m unittest discover -s examples/f04_overnight -p 'test_*.py'`.
Run each plan's specific test command, including its separate reflection/comparison directory where present. Public example tests must be bounded local fixture tests and complete within 60 seconds.

## Sampling Rate

Run the owning test command after each code task and all phase example tests after an implementation wave. Use deterministic fixture time, no watchers, providers or live services. Read and validate documents after their task and inspect all staged content before commit.

## Per-Task Verification Map

| Task ID | Plan | Wave | Requirements | Threat Ref | Secure Behavior | Test Type | Automated Command | File Exists | Status |
|---|---|---|---|---|---|---|---|---|---|
| 03-01-01 | 01 | 1 | F04-01, F04-03 | T-03-02/T-03-03 | Public synthetic data and honest provenance | behavior | See task automated command in PLAN.md | Created by first example task | pending |
| 03-01-02 | 01 | 1 | F04-01, F04-03 | T-03-02/T-03-03 | Public synthetic data and honest provenance | artifact plus evidence review | See task automated command in PLAN.md | Created by owning task | pending |
| 03-02-01 | 02 | 1 | F04-02 | T-03-02/T-03-03 | Public synthetic data and honest provenance | behavior | See task automated command in PLAN.md | Created by first example task | pending |
| 03-02-02 | 02 | 1 | F04-02 | T-03-02/T-03-03 | Public synthetic data and honest provenance | artifact plus evidence review | See task automated command in PLAN.md | Created by owning task | pending |
| 03-03-01 | 03 | 2 | F04-04 | T-03-02/T-03-03 | Public synthetic data and honest provenance | artifact plus evidence review | See task automated command in PLAN.md | Created by owning task | pending |
| 03-03-02 | 03 | 2 | F04-04 | T-03-02/T-03-03 | Public synthetic data and honest provenance | artifact plus evidence review | See task automated command in PLAN.md | Created by owning task | pending |

## Wave 0 Requirements

Each first example task owns its tests and fixtures, runs a failing behavior check before implementation, then makes it pass. No test scaffold has been executed or claimed complete during planning. Document checks use Python directly after their target files are written.

## Manual-Only Verifications

| Behavior | Requirement | Why Human/External Evidence | Check |
|---|---|---|---|
| Actual Quill authorship | F04-04 | JSON syntax cannot prove a real writer/run | Inspect actual workflow receipt and returned artifact; no substitute |
| Source-faithful public claims | All phase requirements | Automated fields cannot establish factual support | Review dated sources, contrary evidence and private-content exclusions |

## Validation Sign-Off

All tasks contain automated checks and specific acceptance criteria; behavior tests include failure cases. Nyquist coverage here describes the plan contract, not executed tests. Quill access remains blocked, and no live capability or Colab execution is claimed.
