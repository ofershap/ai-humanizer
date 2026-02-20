---
name: audit
description: Scan project files for AI-detectable patterns in prose, comments, commits, and docs
---

Scan the current project for AI fingerprints that detectors and experienced developers would flag.

Check these file types: README.md, CHANGELOG.md, docs/, \*.md, code comments, package.json
descriptions, PR templates.

For each file, look for:

1. **Em dashes** (—) used as separators
2. **Flagged vocabulary**: delve, tapestry, leverage, utilize, facilitate, streamline, paramount,
   pivotal, meticulous, holistic, robust, comprehensive, multifaceted, harness, foster, bolster,
   seamless, cutting-edge, game-changing, revolutionary, groundbreaking, nuanced, intricate,
   elevate, empower, unleash
3. **AI opening/closing cliches**: "In today's...", "It's worth noting...", "In summary...", "Happy
   coding!"
4. **Narrating code comments**: comments that describe what the next line does instead of why
5. **Over-formatting**: bold-label bullets, uniform list lengths, excessive markdown
6. **Low burstiness**: 4+ consecutive sentences of similar length
7. **AI git metadata**: Co-authored-by trailers for AI tools in recent commits

For each finding:

1. Show the file and line
2. Quote the problematic text
3. Suggest a human-sounding replacement
4. Rate: high (em dashes, flagged words, git trailers) / medium (cliches, over-formatting) / low
   (burstiness, minor style)

After the scan, show a summary count by category.

Use the ai-humanizer skill for the full reference of patterns to check.
