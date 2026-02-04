# Lean Prompts

A collection of prompts, skills, and agent instructions for AI-assisted Lean 4 and Mathlib development. This includes system prompts, Claude Code skills, Codex skills, slash commands, and anything else that can be used to prompt or otherwise instruct AI agents for Lean 4 programming.

Inspired by [review-prompts](https://github.com/masoncl/review-prompts) (Linux kernel / systemd) and the discussion around AI-assisted Mathlib PR review on the [Lean Zulip](https://leanprover.zulipchat.com/).

## Structure

Each subdirectory targets a different workflow:

| Directory | Purpose | Status |
|-----------|---------|--------|
| `review/` | Mathlib PR review prompts | WIP |

## Background

Inspired by Joseph Myers' suggestion in the [sloplib discussion on Zulip](https://leanprover.zulipchat.com/#narrow/channel/113488-general/topic/sloplib/with/571929508) that AI could help with the mechanical parts of Mathlib PR review — the things that aren't quite mechanical enough for linters but don't require deep mathematical judgment.

See also: [botbaki](https://github.com/kim-em/botbaki) by Kim Morrison, an AI-powered review bot for Mathlib PRs.

## Contributing

Contributions welcome. See each subdirectory's README for what's needed.

Key references for writing review prompts:
- [Mathlib style guide](https://leanprover-community.github.io/contribute/style.html)
- [Mathlib naming conventions](https://leanprover-community.github.io/contribute/naming.html)
- [Mathlib documentation conventions](https://leanprover-community.github.io/contribute/doc.html)
- [Mathlib contribution guide](https://leanprover-community.github.io/contribute/index.html)

## License

MIT
