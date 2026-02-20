# AI Humanizer

Make AI-generated content undetectable. Rules that prevent the patterns AI detectors and experienced developers flag - em dashes, buzzwords, over-formatting, narrating comments, git co-author trailers, and uniform sentence structure.

## Install

### Cursor IDE

```
/add-plugin ai-humanizer
```

### Claude Code

```
/plugin install ai-humanizer
```

### Skills only (any agent)

```bash
npx skills add ofershap/ai-humanizer/ai-humanizer
```

Or copy `skills/` into your `.cursor/skills/` or `.claude/skills/` directory.

## What's Included

### Skills

- **ai-humanizer** - 10 rules covering vocabulary, formatting, structure, comments, commits, and git metadata. Full word blacklist and pattern reference.

### Rules

- **best-practices** - Always-on rules that catch AI patterns before they're written

### Commands

- `/audit` - Scan your project for AI fingerprints in READMEs, docs, comments, and git history

## Why This Plugin?

AI detectors look for statistical patterns, not meaning. These are the patterns that get flagged:

1. **Em dashes everywhere** - AI uses em dashes (—) 5-10x more than humans. Detectors weight this heavily.
2. **Buzzword density** - Words like "delve", "leverage", "robust", "comprehensive" appear 50-700x more in AI text.
3. **Uniform sentence length** - AI writes sentences of 12-18 words consistently. Humans vary wildly.
4. **Narrating comments** - `// Import the module` above an import statement is an instant tell.
5. **Git co-author trailers** - `Co-authored-by: Cursor <cursoragent@cursor.com>` permanently marks your commits.
6. **Over-formatting** - Bold labels on every bullet, perfect parallel structure, tricolons in every list.

This plugin prevents all of these by changing agent behavior at the rule level. The agent writes human-sounding content from the start instead of fixing it after.

## License

MIT
