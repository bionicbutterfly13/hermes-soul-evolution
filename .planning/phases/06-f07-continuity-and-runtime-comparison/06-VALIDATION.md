---
phase: 6
slug: f07-continuity-and-runtime-comparison
status: planned
nyquist_compliant: true
wave_0_complete: false
created: 2026-09-07
---

# Phase 6 validation strategy

## Test Infrastructure

Python standard-library unittest; no package installation.
Quick command: `python3 -m unittest discover -s examples/f07_continuity -p 'test_*.py'`.
Run each plan's specific test command, including its separate reflection/comparison directory where present. Public example tests must be bounded local fixture tests and complete within 60 seconds.

## Sampling Rate

Run the owning test command after each code task and all phase example tests after an implementation wave. Use deterministic fixture time, no watchers, providers or live services. Read and validate documents after their task and inspect all staged content before commit.

## Per-Task Verification Map

| Task ID | Plan | Wave | Requirements | Threat Ref | Secure Behavior | Test Type | Automated Command | File Exists | Status |
|---|---|---|---|---|---|---|---|---|---|
| 06-01-01 | 01 | 1 | F07-01, F07-02 | T-06-02/T-06-03 | Public synthetic data and honest provenance | behavior | See task automated command in PLAN.md | Created by first example task | pending |
| 06-01-02 | 01 | 1 | F07-01, F07-02 | T-06-02/T-06-03 | Public synthetic data and honest provenance | artifact plus evidence review | See task automated command in PLAN.md | Created by owning task | pending |
| 06-02-01 | 02 | 1 | F07-03 | T-06-02/T-06-03 | Public synthetic data and honest provenance | behavior | See task automated command in PLAN.md | Created by first example task | pending |
| 06-02-02 | 02 | 1 | F07-03 | T-06-02/T-06-03 | Public synthetic data and honest provenance | artifact plus evidence review | See task automated command in PLAN.md | Created by owning task | pending |
| 06-03-01 | 03 | 2 | F07-04, F07-05 | T-06-02/T-06-03 | Public synthetic data and honest provenance | artifact plus evidence review | See task automated command in PLAN.md | Created by owning task | pending |
| 06-03-02 | 03 | 2 | F07-04, F07-05 | T-06-02/T-06-03 | Public synthetic data and honest provenance | artifact plus evidence review | See task automated command in PLAN.md | Created by owning task | pending |
| 06-03-03 | 03 | 2 | F07-04, F07-05 | T-06-02/T-06-03 | Public synthetic data and honest provenance | artifact plus evidence review | See task automated command in PLAN.md | Created by owning task | pending |

## Wave 0 Requirements

Each first example task owns its tests and fixtures, runs a failing behavior check before implementation, then makes it pass. No test scaffold has been executed or claimed complete during planning. Document checks use Python directly after their target files are written.

## Manual-Only Verifications

| Behavior | Requirement | Why Human/External Evidence | Check |
|---|---|---|---|
| Actual Quill authorship | F07-05 | JSON syntax cannot prove a real writer/run | Inspect actual workflow receipt and returned artifact; no substitute |
| Source-faithful public claims | All phase requirements | Automated fields cannot establish factual support | Review dated sources, contrary evidence and private-content exclusions |
| Attentiveness | F07-02 | This is the user's assessment | Record Dr. Mani's actual rating; leave unknown if absent |

## Validation Sign-Off

All tasks contain automated checks and specific acceptance criteria; behavior tests include failure cases. Nyquist coverage here describes the plan contract, not executed tests. Quill access remains blocked, and no live capability or Colab execution is claimed.
