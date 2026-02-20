# AI Humanizer

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Skills](https://img.shields.io/badge/skills.sh-ai--humanizer-blue)](https://skills.sh/ofershap/ai-humanizer/ai-humanizer)

Make AI-generated content undetectable. Prevents the patterns AI detectors and experienced developers flag - em dashes, buzzwords, over-formatting, narrating comments, git co-author trailers, and uniform sentence structure.

> AI detectors look for statistical patterns, not meaning. This plugin prevents those patterns at the source. The agent writes human-sounding content from the start instead of you fixing it after.

## Install

### Cursor / Claude Code / Windsurf

```bash
npx skills add ofershap/ai-humanizer/ai-humanizer
```

Or copy `skills/` into your `.cursor/skills/` or `.claude/skills/` directory.

## What's Included

| Type | Name | Description |
|------|------|-------------|
| Skill | `ai-humanizer` | 10 rules covering vocabulary, formatting, structure, comments, commits, and git metadata |
| Rule | `best-practices` | Always-on behavioral rule that catches AI patterns before they're written |
| Command | `/audit` | Scan your project for AI fingerprints in READMEs, docs, comments, and git history |

## What It Catches

| AI pattern | Why it gets flagged | What the plugin enforces |
|------------|--------------------|-----------------------|
| Em dashes (---) everywhere | AI uses them 5-10x more than humans | Hyphens with spaces, periods, or restructured sentences |
| "delve", "leverage", "robust" | 50-700x more frequent in AI text | Plain words: "use", "important", "careful" |
| "In today's...", "Happy coding!" | Opening/closing cliches | Direct, varied openings |
| 12-18 word sentences consistently | Uniform length is a strong signal | Mixed short and long sentences |
| `// Import the module` | Narrating comments are an instant tell | Only non-obvious intent in comments |
| `Co-authored-by: Cursor` | Permanently marks your git history | No AI attribution in commits |
| Bold labels on every bullet | Over-formatting signals AI | Sparse, varied formatting |

## Related Plugins

- [think-first](https://github.com/ofershap/think-first) - Plan-first workflow (pairs well with humanized output)

## Author

[![Made by ofershap](https://gitshow.dev/api/card/ofershap)](https://gitshow.dev/ofershap)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/ofershap)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-181717?style=flat&logo=github&logoColor=white)](https://github.com/ofershap)

## License

MIT
