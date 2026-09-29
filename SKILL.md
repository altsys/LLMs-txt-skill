---
name: llms-txt
description: Generate or improve a curated llms.txt file for a website.
---

# LLMs.txt Generator

Generate a simple, useful, curated `llms.txt` file for a website.

The goal is **maximum useful coverage with minimum links**, not an exhaustive index of every page.

## Workflow

### 1. Inspect the website

Start with the website's homepage.

Look for:

- An existing `/llms.txt`
- The main navigation
- A sitemap, if available
- Important sections of the site
- Documentation, guides, projects, products, or other core content

Understand what the website is about before selecting links.

### 2. Identify the most useful pages

Prioritize pages that help an LLM understand the website or discover deeper content.

Prefer:

- Important hub or index pages
- Documentation entry points
- Product or project pages
- Important guides or reference material
- About pages when they provide useful context
- Pages prominently linked from the site's primary navigation

A page being heavily linked is a useful signal, but not proof that it belongs in `llms.txt`.

Prefer pages that provide unique information or lead to substantial additional information.

### 3. Keep the link set small

Aim for **up to 20 high-value links**. Many sites will need fewer.

Never add a link simply to meet a minimum.

Each URL should normally appear only once in the file, even if it could fit under multiple sections.

Exceed 20 only when the site's size or structure clearly requires it.

Avoid:

- Duplicate or near-duplicate pages
- Repeating the same URL in multiple sections
- Pagination
- Tag and category archives unless genuinely useful
- Search result pages
- Tracking URLs
- Thin or low-value pages

When a single hub page gives access to many related pages, prefer the hub rather than listing every child page.

### 4. Prefer LLM-friendly resources

When verified versions are available, prefer clean Markdown or other text-oriented resources that are easier for an LLM to consume.

Do not invent Markdown URLs or alternate versions that you have not verified.

### 5. Generate the file

Follow the `llms.txt` format.

Start with an H1 containing the website or project name.

Follow it with a short blockquote explaining what the site is about.

Add useful context when necessary.

Organize selected resources into clear H2 sections.

Each resource should use this format:

`[Page title](URL): Short description of why this resource is useful.`

Keep descriptions factual and concise.

## Existing llms.txt

If the website already has an `llms.txt`, review it before replacing it.

Preserve useful existing content.

Prefer small improvements over rewriting a good file unnecessarily.

## Final check

Before returning the file, verify that:

- The links are valid
- The most important parts of the site are represented
- Hub pages are preferred where appropriate
- Each URL normally appears only once
- Low-value URLs have been excluded
- No links were added merely to reach a target count
- The file is concise
- The result helps an LLM understand and navigate the site without trying to reproduce the entire sitemap
