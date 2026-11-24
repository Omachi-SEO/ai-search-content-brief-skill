# AI Search Content Brief Generator

A Claude plugin package containing a research-led skill for creating writer-ready content briefs for traditional organic search and AI search experiences, including Google AI Overviews, Google AI Mode, ChatGPT and Perplexity.

The skill combines live SEO research, competitor analysis, AI Search visibility data and editorial strategy. It is designed to produce a defensible brief grounded in current data, rather than a generic outline generated from model knowledge.

## What the skill does

Given a topic or primary keyword, brand and domain, buyer journey stage, and target region, the skill follows a six-step workflow:

1. **Intake:** Collects the topic, brand/domain, buyer journey stage and target region.
2. **Live research:** Uses SE Ranking MCP to retrieve SERP results, related and long-tail keywords, question keywords, domain information, AI Search Leaderboard data and AI search prompts citing the brand and competitors.
3. **Strategic analysis:** Assesses search intent, buyer journey emotion, AI Share of Voice (AISoV), SERP gaps and AI citation structure.
4. **Brief generation:** Produces a recommended title, meta description, keywords, intent, journey stage, word-count range, content format and detailed writer-ready outline.
5. **Verification:** Checks the brief against a quality checklist covering intent, brand positioning, keyword use, citation opportunities, evidence, internal links and buyer-journey alignment.
6. **Delivery:** Saves the brief as a Markdown file, includes source URLs and summarises the key research findings.

## What the brief includes

- Recommended H1 title and meta description
- Primary and secondary keywords
- Search intent and buyer journey stage
- Recommended word count and content format
- AI Share of Voice status and strategic goal
- Section-by-section outline with writing instructions
- Keyword placement and structural recommendations
- HIGH / MEDIUM / LOW AI citation-potential flags
- Internal-link cues and storytelling considerations where relevant
- FAQ recommendations based on commercially relevant question data
- A verification checklist and writer notes
- A Sources section containing key URLs referenced

## Requirements and dependencies

- **Claude environment with support for the plugin/skill package format.**
- **SE Ranking MCP:** Must be connected and authenticated. The skill requires live SE Ranking data and must not substitute guessed or remembered data when the connection is unavailable.
- **SE Ranking account access:** The connected account must have access to the relevant keyword, SERP and AI Search data.
- **Workspace/file tools:** The workflow references workspace tools for processing large SERP result files and presenting the completed Markdown brief. Availability depends on the Claude environment in which the plugin is run.

The package does not include an SE Ranking account, API key, OAuth token or other credentials. Each user must configure and authenticate their own connection.

## Installation

This repository contains a Claude plugin package. Install it using the plugin installation/import workflow supported by your Claude environment.

The package structure is:

```text
.claude-plugin/
  plugin.json
skills/
  ai-search-content-brief/
    SKILL.md
```

After installing the package:

1. Configure and authenticate the SE Ranking MCP connection in your Claude environment.
2. Confirm that the required SE Ranking data tools are available.
3. Enable the plugin/skill.
4. Request a research-backed content brief and provide the topic, brand/domain, buyer journey stage and target region.

The full workflow depends on the SE Ranking MCP connection. Without it, the skill should not proceed by guessing research data.

## Download Skill

Release link - https://github.com/Omachi-SEO/ai-search-content-brief-skill/releases/tag/v1.0.0 

## When to use it

Use the skill when you need a detailed, research-backed content brief for an article targeting a specific search query and buyer journey stage.

It is intentionally heavyweight. It is not designed for quick blog ideas, casual brainstorming or lightweight outlines.

## Demo

Watch the skill demonstration (https://photos.app.goo.gl/cKPMv3Rx2NfPaFvr9))

## Project notes

I built this skill to connect traditional SEO research with AI Search visibility analysis in a repeatable content-brief workflow. It reduces the manual effort involved in collecting and organising research while keeping strategic decisions, fact-checking and editorial judgement human-led.
 
