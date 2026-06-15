# DYKS

**D**RY · **Y**AGNI · **K**ISS · **SOL**ID — a [Cursor rule](https://cursor.com/docs/context/rules) for keeping AI-assisted code changes focused, simple, and maintainable.

## Install

Copy the rule into your project or user rules:

```bash
# Project rule (applies to this repo only)
mkdir -p .cursor/rules
curl -o .cursor/rules/dry-yagni-kiss-solid.mdc \
  https://raw.githubusercontent.com/felipecordero/dyks/main/dry-yagni-kiss-solid.mdc

# Or user rule (applies globally)
mkdir -p ~/.cursor/rules
curl -o ~/.cursor/rules/dry-yagni-kiss-solid.mdc \
  https://raw.githubusercontent.com/felipecordero/dyks/main/dry-yagni-kiss-solid.mdc
```

Or clone this repo and copy `dry-yagni-kiss-solid.mdc` manually.

## What it does

The rule tells Cursor to apply four principles on every task — design, implementation, refactor, and review:

| Principle | One-liner |
|-----------|-----------|
| **KISS** | Prefer the simplest solution that correctly solves the problem. |
| **YAGNI** | Build only what is required now. |
| **DRY** | Reuse and consolidate; don't copy-paste. |
| **SOLID** | Single responsibility, open/closed, Liskov, interface segregation, dependency inversion. |

Before finishing any change, the agent checks: smallest correct diff, no unnecessary duplication, and clear unit boundaries.

## License

MIT — see [LICENSE](LICENSE).
