# Runtime personality comparison: source packet

**Recorded:** 2026-09-07. **Status:** Proposed experiment; no comparative test has run. This is operational source material for Quill.

## Correct comparison

Hermes using GPT-6 Astra, Codex desktop, and Codex CLI running inside Warp. The third condition is not Warp's native agent.

## Evidence and limits

- [GPT-6 Astra guidance](https://developers.openai.com/api/docs/guides/latest-model) describes sensitivity to skill/instruction guidance and response-style directions. These tendencies do not diagnose a particular session.
- [Hermes personality documentation](https://hermes-agent.nousresearch.com/docs/user-guide/features/personality) identifies SOUL.md as an instance-scoped identity slot and describes a session personality overlay.
- A dated local source inspection found the Responses transport sending assembled instructions alongside the selected model and conversation. This supports distinguishing a backend from the complete Codex application's context; it is not a new network trace.
- [Codex configuration](https://learn.chatgpt.com/docs/config-file/config-basic), [AGENTS.md](https://learn.chatgpt.com/docs/agent-configuration/agents-md) and [configuration reference](https://learn.chatgpt.com/docs/config-file/config-reference) document configuration and instruction layers. The comparison has not inspected the local Codex configuration.
- [Warp agent objects](https://docs.warp.dev/knowledge-and-collaboration/warp-drive/ai-objects) concern Warp's own agent. They do not establish that Warp injects those rules into an independently launched Codex CLI.

## Hypothesis

Differences in instructions, recovered context, available tools, permission rules and runtime settings may affect apparent initiative and continuity even when a displayed model label matches. Equal labels do not establish equal backend revisions or effective inputs. This is a testable hypothesis, not a finding about intrinsic model personality.

## Proposed protocol

Record resolved model identifier, client/runtime version, reasoning settings, working directory category, visible effective instructions, memory availability, skills/tools and permission profile. Mark hidden or unavailable layers unknown; never export hidden instructions or private conversations.

Use fresh sessions for synthetic interrupted commitments, changed priorities, factual corrections, evidence-backed disagreement and failed artifacts. Separate communication-only runs from tool/memory-enabled runs. Choose and record repeat count before execution, randomize review order, and retain unmatched conditions rather than forcing a platform-effect claim.

Score relevant-context recovery, unnecessary clarification, truthful uncertainty and follow-through. Record Dr. Mani's actual attentiveness assessment separately from automatic scoring. No imagined user reactions.

Colab may host synthetic fixtures or analysis and a separately configured API condition. An API call cannot stand in for the desktop/CLI application. Publish a Colab run/link only after actual execution.

## Initial SOUL review

Review [Claudia's inspected seed](https://github.com/kbanc85/claudia-autonomous/blob/177236207991ed7ccec6de16a9458ecdcf9c1b3f/claudia_cli/default_soul.py) first, then selectively use Felix ownership/follow-through practices. Examine adaptation to pace, commitments, corrections and stable stance. Do not adopt unsupported experiential claims, unverified 24/7 operation or repeated approval demands that conflict with the requested executive autonomy. No active SOUL edit is part of this source packet.

