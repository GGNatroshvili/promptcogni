# PromptCogni

**Evidence before perfection. Useful delivery with an explicit finish line.**

PromptCogni is a principal operating skill for AI-assisted development, research, products, and workflows. It helps an agent preserve the user's objective, explore unfamiliar ideas, build a small complete result, verify what matters, and close an accepted release.

## Principles

1. Establish a small, stable delivery contract.
2. Explore novelty without inventing certainty.
3. Prioritize issues by consequence: **BLOCK**, **CONTAIN**, or **DEFER**.
4. Build the smallest complete, useful increment.
5. Spend effort where it changes the result.
6. Make important failures diagnosable and containable.
7. Verify proportionally and truthfully.
8. Use an explicit convergence rule instead of endless review.
9. Check decisions against evidence rather than imagined perfection.
10. Report what exists and what was actually demonstrated.

Read the complete policy in [English](skills/pragmatic-building/references/prompt-en.md) or [Spanish](skills/pragmatic-building/references/prompt-es.md). The [skill](skills/pragmatic-building/SKILL.md) is the compact operational entrypoint.

## Install in OpenCode V2

Clone this repository. Copy `skills/pragmatic-building/` into your OpenCode user skill directory, usually `~/.config/opencode/skills/`. If that skill already exists, inspect and preserve your current version before replacing it.

Add this block to your existing global `~/.config/opencode/AGENTS.md` without replacing unrelated instructions:

```markdown
## Principal operating skill: PromptCogni

At the start of every task, load
`~/.config/opencode/skills/pragmatic-building/SKILL.md` and its
`references/prompt-en.md` before planning, executing, or loading task-specific
skills. Reuse both while present in context; reload after compaction if absent.
If skill discovery is unavailable, read those exact files directly.
Apply the relevant steps proportionally. Preserve higher-priority instructions,
project authorization, ownership, and required domain controls.
```

The global pointer makes this the principal skill across projects for that user configuration. Keep task-specific skills for specialized work. Simple questions stay simple; loading the policy does not require a planning document or a review ceremony for every answer.

Verify that OpenCode discovers `pragmatic-building` and can load the full policy. Installing a skill is not proof that every future agent follows it; assess compliance from actual delivery evidence. Other users, hosts, and harnesses need their own verified installation.

OpenCode V2's `instructions` configuration array currently accepts values without loading their contents. Use the active `AGENTS.md` entrypoint. See the official [instructions](https://opencode.ai/v2/docs/instructions/) and [skills](https://opencode.ai/v2/docs/skills/) documentation.

## Use with another agent

Point the harness's actual persistent instruction entrypoint to `skills/pragmatic-building/SKILL.md` and the complete policy. Require loading at task start and reuse while in context. Confirm that the harness reads the files rather than merely storing their paths.

This guidance preserves domain-specific review requirements, permissions, and essential invariants. A working implementation is separate from business effectiveness; experiments and simulations must be labeled accurately.

## Example

For a web form, a useful increment is: submit real input, persist it, and display the saved record. Verify that path and relevant failure handling. A noncritical spacing issue can be deferred with a revisit trigger. Silent data loss blocks the affected release. Once the agreed criteria pass, deliver; optional improvements belong in the next scope.

## Updates and rollback

Review changed policy text, replace the installed skill with the reviewed version, and verify loading again. To uninstall, remove only your PromptCogni instruction block and installed `pragmatic-building` directory. Preserve unrelated configuration and project evidence.

## Publication scope

This repository contains the reusable skill, bilingual policy, and installation guidance. It does not include private project configuration, operational receipts, session history, credentials, or personal machine paths.

## License status

No open-source license grant has been declared for this material. Public availability alone does not establish a redistribution license. The skill's `LicenseRef-Owner-Provided` metadata records this status.
