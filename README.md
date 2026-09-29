# LLMs.txt Skill

A simple skill for generating curated `llms.txt` files for websites.

The goal is not to dump every URL from a site. The skill tries to identify the smallest set of useful pages that gives an LLM a good understanding of the website.

## What it does

Given a website, the skill:

- Inspects the homepage and main navigation
- Checks for an existing `llms.txt`
- Looks for important hub pages, documentation, projects, guides, and other core content
- Prioritizes high-value pages over exhaustive indexing
- Usually limits the result to around 10 to 20 links
- Produces a clean `llms.txt` file

## Example

Ask your agent:

> Generate an llms.txt file for https://hawando.com using this skill.

For a personal site like Hawando, the skill should prefer a small number of pages that explain the site and provide access to deeper content instead of listing every blog post.

For example, it may prioritize:

- Homepage
- About
- Projects
- Writing or blog index
- Tutorials
- Important tools or projects

The exact links should be chosen by inspecting the current website.

## Usage

Add `SKILL.md` to an agent or coding environment that supports skills, then ask it to generate or improve an `llms.txt` file for a website.

Example:

```text
Generate an llms.txt for https://hawando.com