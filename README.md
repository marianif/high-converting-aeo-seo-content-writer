# High-Converting AEO & SEO Content Writer

An [Agent Skills](https://agentskills.io/specification)–compatible skill that writes and rewrites **product-led marketing content**: blog posts, guides, explainers, comparisons (`X vs Y`, `alternatives`, `best`) and page copy. Everything leads with the answer so AI answer engines can quote it, and steers a reader who is mid-decision toward the product.

It is deliberately **not** a neutral journalist and **not** a note-taker. Every piece has one job: move a reader choosing between options toward the product.

**The constraint that makes it work:** the verdict always favors the product — and every favorable claim is true, sourced and dated. A caught exaggeration destroys the trust that closes a decision-stage reader, so fabricated numbers, benchmarks, quotes, coverage and user counts are banned outright.

> **Also known as:** SEO content writer · AEO content writer · GEO content writing · answer-first blog writing · long-form article writer · comparison page / alternatives page / "X vs Y" writer · best-of page · product-led content · growth marketing copy · conversion copywriting · Claude Code / OpenCode / Codex / Cursor Agent Skill.

## What it does

| Phase | Outcome |
| --- | --- |
| Step 0 — Learn the project | Product source of truth, maturity (concept / prototype / shipped), CMS and content pipeline |
| Brief | Keyword, angle, audience, the reader's decision, what the piece must prove |
| Write | Answer-first sections, question-shaped H2s, honest comparison tables, one CTA |
| Verify | Every competitor number dated and sourced; no unshipped feature in the present tense |
| Ship | Written to the authoritative content location, not a regenerated build output |

It is **product-agnostic**: it learns the project first and never carries facts, names or paths over from another product. If the project keeps a notes vault, style guide or editorial system, that wins over any default in the skill.

## Install

```sh
npx skills add marianif/high-converting-aeo-seo-content-writer
```

The [skills CLI](https://github.com/vercel-labs/skills) detects your installed agents, clones the repo and links the skill into each one. Useful flags:

```sh
# Install globally for Claude Code and OpenCode, non-interactive
npx skills add marianif/high-converting-aeo-seo-content-writer -g -a claude-code -a opencode -y

# Inspect before installing
npx skills add marianif/high-converting-aeo-seo-content-writer --list
```

It works with Claude Code plugin marketplaces, Codex, Cursor, Gemini CLI, GitHub Copilot, Windsurf and [75+ other agents](https://github.com/vercel-labs/skills#supported-agents).

<details>
<summary>Manual install (no Node)</summary>

Clone the repo into the skills directory of your harness, keeping the folder named `high-converting-aeo-seo-content-writer`:

```sh
git clone https://github.com/marianif/high-converting-aeo-seo-content-writer.git <skills-dir>/high-converting-aeo-seo-content-writer
```

| Harness | Typical skills directory |
| --- | --- |
| Claude Code | `~/.claude/skills/high-converting-aeo-seo-content-writer/` |
| OpenCode | `.opencode/skills/high-converting-aeo-seo-content-writer/` (project) or `~/.config/opencode/skills/high-converting-aeo-seo-content-writer/` |
| Codex / Cursor / other Agent Skills runtimes | that runtime's documented skills directory |

</details>

## Complements research skills

This skill writes; it does not research. It expects the research to have already happened:

- **Keyword research / clustering** — what to target.
- **Competitor analysis / competitive landscape** — who and what they rank for.
- **AI visibility audit** — what answer engines already say, and where the product is missing.

It pairs naturally with the [OpenSEO](https://github.com/every-app/open-seo) research skills (MIT), which is what its "Related skills" section refers to. Research first, then write from it.

## Suggested initial requests

- "Use the content writer skill. Write the 'alternatives' page for [product], leading with the answer and keeping every competitor claim sourced and dated."
- "Rewrite this existing post so each H2 answers its question in the first two sentences."
- "Draft a comparison table for [product] vs [competitor] — product column first, and include where the other tool wins."
- "Review this draft against the pre-publish checklist and tell me what would get it dropped by an answer engine."

## Package contents

- `SKILL.md` — the complete skill: role, constraints, Step 0 project discovery, writing rules, comparison-page format, checklists and guardrails.

## Guardrails it enforces

- No invented product facts, numbers or competitor limitations — leave it out or write `unknown`.
- No honest comparison turned into a sales page with a comparison skin.
- No unshipped feature described in the present tense.
- No comparison published before the product has a comparable shipping state.
- No hand-editing build output and calling it done.

## Search terms

If you arrived here searching for any of these, this is the skill:

`content writing skill` · `seo content writer` · `aeo content writer` · `geo content` · `answer engine optimization` · `generative engine optimization` · `ai citations` · `answer-first writing` · `blog post writer` · `long-form article skill` · `comparison page writer` · `alternatives page` · `vs page` · `best-of page` · `landing page copy` · `product-led content` · `growth marketing` · `conversion copywriting` · `claude code skill` · `claude skills` · `opencode skill` · `codex skill` · `cursor skill` · `agent skills`

## License

Licensed under the [MIT License](LICENSE).
