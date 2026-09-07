# Phase 6 multi-source coverage audit

**Status:** Plan coverage checked; no requirement or live behavior is marked completed.

| Source | ID | Item | Plan | Status | Notes |
|---|---|---|---|---|---|
| CONTEXT | D-11 | Exact user-selected Claudia article title | 06-03 | COVERED | Task 2 and must_haves preserve the title |
| GOAL | Phase 6 | Continuity and runtime comparison with public examples, protocol and actual Quill post | 06-01, 06-02, 06-03 | COVERED | Execution pending |
| REQ | F07-01 | F07-01 from REQUIREMENTS.md | 06-01 | COVERED | Not executed |
| REQ | F07-02 | F07-02 from REQUIREMENTS.md | 06-01 | COVERED | Not executed |
| REQ | F07-03 | F07-03 from REQUIREMENTS.md | 06-02 | COVERED | Not executed |
| REQ | F07-04 | F07-04 from REQUIREMENTS.md | 06-03 | COVERED | Not executed |
| REQ | F07-05 | F07-05 from REQUIREMENTS.md | 06-03 | COVERED | Quill access blocked |
| RESEARCH | R-01 | R-01 from phase RESEARCH.md | 06-01, 06-02, 06-03 | COVERED | Dated evidence and limits preserved |
| RESEARCH | R-02 | R-02 from phase RESEARCH.md | 06-01, 06-02, 06-03 | COVERED | Dated evidence and limits preserved |
| RESEARCH | R-03 | R-03 from phase RESEARCH.md | 06-01, 06-02, 06-03 | COVERED | Dated evidence and limits preserved |
| RESEARCH | R-04 | R-04 from phase RESEARCH.md | 06-03 | COVERED | Dated evidence and limits preserved |
| RESEARCH | R-05 | R-05 from phase RESEARCH.md | 06-01, 06-02, 06-03 | COVERED | Dated evidence and limits preserved |
| CONTEXT | D-01 | Preserve "Executive operator: decisive, concise, and focused on getting things finished." | 06-01, 06-03 | COVERED | No decision silently dropped |
| CONTEXT | D-02 | Track GSD plans and reviewed documentation in the approved public GitHub project. | 06-01 | COVERED | No decision silently dropped |
| CONTEXT | D-03 | Keep this finding in its own feature branch/worktree and produce its own Quill issue post. | 06-01 | COVERED | No decision silently dropped |
| CONTEXT | D-04 | Actual Quill alone drafts and revises blogs; current workflow access is blocked, so never substitute prose. | 06-03 | COVERED | No decision silently dropped |
| CONTEXT | D-05 | Include direct citations and tested code examples; add Colab links only after actual execution. | 06-01, 06-02, 06-03 | COVERED | No decision silently dropped |
| CONTEXT | D-07 | Planning does not authorize live repairs, provider calls, service operations or active SOUL changes. | 06-01, 06-03 | COVERED | No decision silently dropped |
| CONTEXT | D-09 | Separate dated observations, history, inference, synthetic results and unrun live proposals. | 06-01, 06-02, 06-03 | COVERED | No decision silently dropped |
| CONTEXT | D-10 | Review all public content and omit secrets, private task/client data, transcripts and absolute host paths. | 06-01, 06-03 | COVERED | No decision silently dropped |
| CONTEXT | D-06 | Claudia first, selective Felix, initial design before personality revision. | 06-01, 06-03 | COVERED | No decision silently dropped |
| CONTEXT | D-08 | Hermes, Codex desktop, Codex CLI in Warp; comparison unrun. | 06-02 | COVERED | No decision silently dropped |

## Dependencies and ownership

Additional locked decision D-11 is COVERED by 06-03 Task 2 and must_haves: the exact selected title is passed to Quill. The new named comparisons remain pending research and introduce no accepted design change.

- 06-01: needs existing baseline and research; creates examples/f07_continuity/continuity_scoring.py, examples/f07_continuity/test_continuity_scoring.py, examples/f07_continuity/cases.json, examples/f07_continuity/README.md, docs/features/f07/protocol.md, docs/features/f07/decisions.md; checkpoint: no planned human checkpoint, actual Quill access failures remain blocking.
- 06-02: needs existing baseline and research; creates examples/f07_comparison/comparison_manifest.py, examples/f07_comparison/test_comparison_manifest.py, examples/f07_comparison/cases.json, examples/f07_comparison/README.md, docs/features/f07/runtime-comparison.md; checkpoint: no planned human checkpoint, actual Quill access failures remain blocking.
- 06-03: needs 06-01, 06-02; creates docs/features/f07/source-packet.json, docs/features/f07/quill-brief.md, posts/f07-issue.md, posts/f07-provenance.json, posts/00-motivation.md, posts/01-research.md, posts/02-decisions.md, posts/opening-provenance.json; checkpoint: no planned human checkpoint, actual Quill access failures remain blocking.

Same-wave plans have exclusive files. Research and decision preparation do not grant runtime authority. Deferred live interventions and optional unrun Colab execution are not dropped implementation requirements; they are explicit current-task boundaries. Quill requirements are planned but blocked until the actual workflow is accessible.
