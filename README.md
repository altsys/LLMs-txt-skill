# LLMs.txt Skill

A portable agent skill for generating concise, curated `llms.txt` files for websites.

The goal is **maximum useful coverage with minimum links**. It does not turn a sitemap into another sitemap-shaped file.

## What it does

Given a website, the skill:

- Inspects the homepage, navigation, sitemap, and existing `llms.txt` when available
- Finds high-value hub pages, documentation, projects, guides, and core content
- Prefers pages that provide broad coverage or unique context
- Uses up to 20 high-value links, and often fewer
- Avoids duplicate URLs, thin pages, pagination, tracking URLs, and exhaustive indexing
- Produces a concise `llms.txt`

## Example

Ask your agent:

> Generate an llms.txt for https://hawando.com using the llms-txt skill.

The skill was tested against Hawando.com. Rather than listing every article and project, it selected a small set of pages that cover the site's main areas.

See [examples/hawando.com-llms.txt](examples/hawando.com-llms.txt) for the generated result.

## Install in Codex

This repository is also a Codex marketplace, so you can add it directly:

```bash
codex plugin marketplace add altsys/LLMs-txt-skill
```

Then browse the marketplace and install the `llms-txt` plugin. The marketplace catalog lives at `.agents/plugins/marketplace.json`.

After installation, ask Codex:

```text
Generate an llms.txt for https://example.com using the llms-txt skill.
```

## Portable plugin structure

```text
plugin.json
skills/
  llms-txt/
    SKILL.md
.agents/
  plugins/
    marketplace.json
examples/
  hawando.com-llms.txt
```

The portable plugin manifest is `plugin.json`, and the reusable workflow lives in `skills/llms-txt/SKILL.md`.

## Philosophy

A useful `llms.txt` should help an LLM understand and navigate a website without reproducing the entire sitemap.

**Maximum useful coverage with minimum links.**

## License

MIT
