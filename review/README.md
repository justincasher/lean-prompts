# Review Prompts

AI-assisted prompts for reviewing Mathlib pull requests. Modeled after the [kernel review prompts](https://github.com/masoncl/review-prompts/tree/main/kernel).

## Directory Structure

```
review/
  review-core.md        # Main review protocol (entry point)
  skills/               # Claude Code skill files
  slash-commands/        # Claude Code slash commands (/lreview, etc.)
  patterns/             # Common patterns and anti-patterns
  scripts/              # Setup and utility scripts
  examples/             # Example reviews
```

## What's Needed

The goal is a set of prompts that help AI perform the mechanical parts of Mathlib PR review — the things that aren't quite mechanical enough for linters but don't require deep mathematical judgment. For example:

- **Naming conventions**: Do lemma/definition names follow [Mathlib conventions](https://leanprover-community.github.io/contribute/naming.html)?
- **Style compliance**: Line length, indentation, `by` placement, binder spacing per the [style guide](https://leanprover-community.github.io/contribute/style.html)?
- **Documentation**: Are module docstrings and declaration docs present and well-formed per [doc conventions](https://leanprover-community.github.io/contribute/doc.html)?
- **API completeness**: Are `simp` lemmas, `ext` lemmas, and coercion lemmas provided for new definitions?
- **Tactic hygiene**: Overuse of `decide`, unnecessary `set_option maxHeartbeats`, non-terminal `simp` usage?
- **Definition design**: Appropriate transparency, universe polymorphism, typeclass vs explicit arguments?
- **Deprecation protocol**: Correct use of `@[deprecated]` with dates and messages?

## How to Contribute

1. Pick an area from the list above (or propose a new one)
2. Write a prompt file (`.md`) with detailed, actionable instructions
3. Open a PR

Look at the [kernel review-core.md](https://github.com/masoncl/review-prompts/blob/main/kernel/review-core.md) for the level of detail to aim for.
