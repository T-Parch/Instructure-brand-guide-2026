# Instructure brand guide 2026 — AI-ready bundle.

This repo contains the AI-ready version of the 2026 Instructure Brand Guide. It's the knowledge base that powers the Instructure Brand Guide Assistant, a Claude-based tool the marketing team uses to draft, review, and refine on-brand content.

The files in here are written as structured Markdown so a large language model can read them as persistent context. They mirror the live brand guide at sites.google.com/instructure.com/brandguide/home but are formatted for machine consumption, not browsing.

## What's in this repo.

The files are numbered to indicate priority order when loaded as context.

- `00-system-prompt.md` — the role, guardrails, strictness scale, and brand QA checklist that defines how the assistant behaves.
- `00-deployment-recommendation.md` — how to deploy the bundle in Claude.ai Projects, Claude Code, or as an org-wide skill.
- `01-brand-foundation.md` — mission, positioning, audience, and brand pillars.
- `02-voice-and-tone.md` — how Instructure sounds in writing.
- `03-style-guide.md` — capitalization, punctuation, formatting, and word choice rules.
- `04-legal-and-quick-tips.md` — claims, naming, the top quick-tip list, and review escalation paths.
- `05-glossary.md` — approved terms and what to avoid.
- `06-visual-brand-overview.md` — high-level visual identity summary.
- `07-logos-and-colors.md` — the consolidated logos, colors, and co-branding reference for Canvas, Mastery, Parchment, and Instructure.
- `11-brand-elements.md` — typography, photography, videography, illustration, iconography, and panda usage.
- `12-accessibility.md` — accessibility standards for content, slide design, email, alt text, captions, and meaningful link text.
- `13-product-messaging-canvas.md` — Canvas messaging framework, positioning, and audience narratives.
- `14-product-messaging-canvas-career.md` — Canvas Career messaging framework.
- `15-product-messaging-mastery.md` — Mastery messaging framework.
- `16-product-messaging-igniteai.md` — IgniteAI messaging framework.
- `17-product-messaging-partner-program.md` — Partner Program messaging framework.
- `18-case-study-template.md` — the standard structure for customer case studies.
- `GAPS-AND-SOLUTIONS.md` — known gaps between the live brand guide and this bundle, plus the plan to close them.
- `gemini-bundle/` and `README-gemini-bundle.md` — a Gemini-formatted version of the same content for teams using Google's Gemini.

Files 08, 09, and 10 (the per-product design system files) were retired in May 2026 when the brand consolidated to a single logos and colors page. That content now lives in `07-logos-and-colors.md`.

## How to use this bundle.

The fastest path is Claude.ai Projects. Create a project, upload every numbered file as project knowledge, paste the contents of `00-system-prompt.md` into the project instructions, and invite the team. Anyone in the project can then ask the assistant to draft copy, review a draft, or answer a brand question with full context.

For the full deployment walkthrough, including Claude Code and org-wide skill options, see `00-deployment-recommendation.md`.

## Source of truth.

The live brand guide at sites.google.com/instructure.com/brandguide/home is always the canonical source. If something in here conflicts with the live guide, the live guide wins. This bundle is refreshed on a regular cadence — see `REFRESH-WORKFLOW.md` in the parent `brand-guide/` directory for how updates flow from the live site into these files.

## Maintainer.

Trevor Misina, Instructure Marketing. For brand questions outside the scope of this bundle, email brand@instructure.com or post in #brand-questions on Slack.
