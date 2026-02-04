# Lean Prompts

AI-assisted prompts for Lean 4 and Mathlib development. Designed for use with [Claude Code](https://claude.com/claude-code) and other AI tools.

Inspired by [review-prompts](https://github.com/masoncl/review-prompts) (Linux kernel / systemd) and the discussion around AI-assisted Mathlib PR review on the [Lean Zulip](https://leanprover.zulipchat.com/).

## Structure

Each subdirectory targets a different workflow:

| Directory | Purpose | Status |
|-----------|---------|--------|
| `review/` | Mathlib PR review prompts | WIP |

## Background

From [Joseph Myers on Zulip](https://leanprover.zulipchat.com/):

> There should be lots of ways for AI to accelerate stating things other than building a sloplib. For example, AI could probably help with many of the more mechanical parts of PR review for mathlib (that aren't mechanical enough to turn into linters) and so reduce the amount of time maintainers need to spend on those when doing reviews for mathlib. People have written extremely detailed instructions to AIs on Linux kernel patch review, why shouldn't we have similarly detailed instructions on reviewing mathlib changes and a service that does such reviews on PRs (automatically, or when requested)?

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
