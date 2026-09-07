# Hermes Soul Evolution

## Project record

- Owner: Dr. Mani.
- Record: baseline-001.
- Research date: 6 September 2026, America/New_York.
- Local audit date: 7 September 2026, compiled at 09:40 America/New_York.
- Status: research and read-only baseline completed; reviewing researched options and settling the initial design. Persona revision follows; runtime repairs remain deferred.
- Intended audience: public project documentation and source material for a blog series.
- Public repository: [bionicbutterfly13/hermes-soul-evolution](https://github.com/bionicbutterfly13/hermes-soul-evolution). Publication history is recorded in Git.

## Intended behavior

The requested operator organizes the day and follows through during it, delegates work reliably, reports verified results, performs bounded overnight work, reflects on its own decisions and produces useful insights. It should maintain continuity through remembered priorities, commitments and corrections.

The selected relationship style is exactly: **"Executive operator: decisive, concise, and focused on getting things finished."**

This record separates instruction text, observed execution, historical results and proposed behavior. It describes one local installation; it is not a benchmark of Hermes or a general verdict about the platform.

## Baseline findings

### F01: Current identity loaded in the latest recorded CLI session

**Verified:** the stored system prompt for the latest recorded Chief of Staff CLI session contains the complete current profile `SOUL.md` verbatim. That session started on 6 September at 22:16 local time.

**Method:** open profile `state.db` read-only; join `sessions` to `system_prompts`; compare the stored prompt to the current SOUL text.

**Limit:** this proves loading in that session. It does not prove a currently active agent, instruction adherence or successful follow-through.

### F02: Dedicated daily scheduler fails before producing a report

**Verified:** launchd reports the dedicated job registered with a 60-second interval, `state = xpcproxy`, 591 runs and `last exit code = 78: EX_CONFIG`. The entire intended `workspace/proactive/` report directory contains no files.

**Method:** inspect the named service with read-only `launchctl print`; enumerate the complete report directory.

**Limit:** the exact startup cause has not been diagnosed. A service registration or an invocation count is not proof of successful scheduled work. No restart or service change was made.

### F03: Earlier daily routines have stale execution evidence

**Verified:** all five legacy job definitions were inspected. Three enabled jobs last recorded runs on 2 September, with next-run timestamps still on 3 September. The morning summary and daily metacognitive journal are among them. Gateway state records exit on 2 September at 17:35 local time; the active-session registry is empty. The 2 September journal output exists.

**Method:** read profile `cron/jobs.json`, query `cron/executions.db` read-only, inspect gateway lifecycle state and the active-session registry, and inspect the latest journal output.

**Limit:** historical output does not establish that any routine is operating now. No legacy task was changed during the audit.

### F04: The new overnight adapter permits preparation only

**Verified source behavior:** the adapter supplies a ranked snapshot of at most 25 open task-board cards. The model invocation permits the skills toolset and explicitly forbids worker dispatch, project edits, memory updates and other tools. Its output schema consists of `priorities`, `decisions` and `limitations`. It does not supply previous reports, conversation history or a reflection history.

**Evidence locator:** profile `scripts/cos-proactive-run.py`, functions `agent_command()` and `execute()`.

**Consequence:** repairing startup alone would enable a task-board preparation report. It would not establish overnight project execution, cross-day reflection or the requested continuity.

### F05: Memory service health does not establish agent memory continuity

**Verified during the audit:** the configured local Hindsight service returned `status: healthy` and `database: connected`. The research connector could read knowledge pages. Chief of Staff configuration selected Hindsight.

**Verified history:** the four latest explicit Chief of Staff recall results, dated 2-4 September, contain errors. No fresh Chief of Staff recall was invoked during the audit.

**Configuration limit:** the profile-local `hindsight/config.json` is absent. The installed plugin supports legacy shared configuration and environment fallback, so that absence alone is not a diagnosis. The fallback configuration was not inspected.

**Still unverified:** automatic retention, correct memory-bank selection in the running profile, recovery of a relevant earlier decision in a new session, and the same recovery during a scheduled run.

### F06: Result transport and verified specialist delivery differ

**Verified recorded states:** all 26 persisted asynchronous delegation records were enumerated: 18 completed, 4 error and 4 unknown; 25 marked delivered and one dropped. Their returned envelopes contained 40 child results: 34 completed, 2 interrupted and 4 failed.

**Separate acceptance evidence:** the latest named Engineering probe reported a 210-second timeout. Its expected artifact is still absent. Independent review did not run.

**Method:** query profile `state.db` read-only; inspect the saved acceptance output and installation-result report; check the expected artifact's existence.

**Limit:** these counters are process and transport states. They are not a measured artifact-quality success rate. The saved Engineering probe is historical evidence, not a new test run during this audit.

### F07: Relationship continuity lacks concrete acceptance behavior

**Verified instruction text:** the SOUL emphasizes concise output, pushback, shipping, priorities and remembering corrections.

**Interpretation:** it gives little concrete guidance for returning after interruptions, checking its own promises or making continuity observable to the user. That may contribute to a flat or pressuring interaction, but this audit did not test a causal explanation for the user's experience.

**Proposed test:** interrupt a task, change a priority, correct one fact and return in a fresh session. Check whether the agent recovers the relevant reason, honors the correction and resumes useful work without blame or invented familiarity. The user evaluates whether the interaction feels attentive.

## Research references

| Reference | Useful evidence | Limit |
| --- | --- | --- |
| [Claudia's actual seeded SOUL](https://github.com/kbanc85/claudia-autonomous/blob/177236207991ed7ccec6de16a9458ecdcf9c1b3f/claudia_cli/default_soul.py) | Inspectable identity and continuity instructions | Daily proactive behavior was still in progress at inspection; not operational validation |
| [Nat Eliason's Felix interview](https://www.bankless.com/podcast/building-a-million-dollar-zero-human-company-with-openclaw-nat-eliason) | First-person description of nightly review and specialist supervision, including a delegation failure | Commercially interested first-person account |
| [Lex's six-month account](https://notesbylex.com/6-months-of-openclaw) | Maintained daily organizing routine and reported failures | One user's account; not a delegation benchmark |
| [Hermes delegation reference](https://hermes-agent.nousresearch.com/docs/user-guide/features/delegation/) | Documented result delivery and interrupted-child semantics | Installed behavior still needs its own verification |
| [Generative Agents](https://arxiv.org/html/2304.03442v2) | Reflections linked to source observations | Simulated-character research, not executive reliability evidence |
| [LongMemEval](https://arxiv.org/html/2410.10813v2) | Tests for changed information, cross-session retrieval and abstention | Does not measure a complete proactive operator |

Sources were inspected on 6 September 2026. Forum, X, Reddit, Hacker News, Skool, GitHub, first-person and research-paper evidence was covered in the companion research dossier. That search was bounded; no claim of exhaustive coverage or independent validation is made.

## Deferred runtime experiments

| Milestone | Required evidence | Current state |
| --- | --- | --- |
| Reliable daily loop | Scheduler-triggered report with actual timestamps, artifact and visible failure state | Not passed |
| Fresh-session memory | Relevant old decision and subsequent correction recovered in the Chief of Staff profile and a scheduled run | Not run |
| Verified specialist delivery | Named owner returns an artifact; each acceptance criterion is checked; required independent review completes | Latest recorded probe failed |
| Bounded overnight execution | One explicitly assigned task, finite budget, artifact and recoverable failure state | Not run |
| Useful reflection | Source observations, expectation versus outcome, a testable adjustment and evidence of changed later behavior | Not run |
| Continuity trial | Seven days of observed follow-through, correction handling and user assessment of attentiveness | Not run |

The next step is to review the researched options, learn from them and settle the initial design, then revise the personality. Runtime failures remain recorded for later work; repairing them is not a prerequisite for discussing or revising the persona. The experiments above remain unpassed or unrun as recorded. No intervention was applied during the baseline audit.

## Blog-series source protocol

Quill owns blog drafting and revision. This document is an operational evidence record, not a blog draft.

For each completed milestone, prepare a source packet containing the original intent, dated baseline, exact change, test method, observed result, failures, unresolved questions and the user's actual reaction. Preserve contrary evidence. Do not invent first-person experience or improvement claims.

The opening source packet is ready from the research and this baseline. Each issue F02-F07 can support an initial post about the observed problem, researched options and proposed experiment. Follow-up claims about improvements require actual experiment results. Quill will determine the narrative and titles.

Each future entry should record:

```text
Milestone ID and date:
Question or hypothesis:
Prior evidence and finding IDs:
Authorized change:
Verification method:
Observed result:
Failure or uncertainty:
User reaction, verbatim if provided:
Next test:
Quill draft and publication status:
```

## Public record boundaries

This public record omits secrets, private task and client contents, full transcripts, local account identifiers and absolute machine paths. Evidence locators describe the local installation; those files are not presented as publicly available. Local observations are operator-reported and have not been independently reproduced. The private research PDF remains a separate artifact.

## Change log

- 2026-09-07: recorded research selection, read-only baseline F01-F07, proposed acceptance checks and the Quill source-packet protocol. No runtime changes or publication completed as part of the audit.

- 2026-09-07: clarified the next step as research comparison, initial design and persona revision. Recorded the request for one Quill-authored post and one GSD feature stream per issue F02-F07. Feature setup is pending the actual GSD workflow; no runtime repair was authorized by this documentation step.
- 2026-09-07: created the public repository and prepared this baseline, the project README and the issue-mapped series plan for its initial publication.
