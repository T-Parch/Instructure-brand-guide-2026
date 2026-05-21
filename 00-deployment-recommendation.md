# Deployment Recommendation — Instructure Brand Guide Assistant
**Prepared for:** Trevor Misina / Instructure Marketing Team
**Last updated:** 2026-04-29

---

## The goal
Give the marketing team a Claude-powered Brand Guide Assistant that can:
1. Answer brand questions in real-time (voice, style, logo rules, color, product messaging, etc.)
2. Review drafted content for brand compliance and suggest corrections
3. Generate on-brand first drafts or variations
4. Serve as a living reference for product positioning and messaging frameworks

---

## Recommended approach: Claude.ai Projects (strongest fit)

### Why Projects?
Claude.ai Projects let you upload files as persistent context that live across all conversations in that project. Every team member who joins the project gets the same brand knowledge baked in from the start — no prompting required, no copy-pasting files.

### Setup
1. Create a Project in Claude.ai called **"Instructure Brand Guide Assistant"**
2. Upload these files from `ai-ready/` as project knowledge (in order):
   - `00-system-prompt.md` (defines the assistant's role)
   - `01-brand-foundation.md`
   - `02-voice-and-tone.md`
   - `03-style-guide.md`
   - `04-legal-and-quick-tips.md`
   - `05-glossary.md`
   - `06-visual-brand-overview.md`
   - `07-design-system-instructure.md`
   - `08-design-system-canvas.md`
   - `09-design-system-mastery.md`
   - `10-design-system-parchment.md`
   - `11-brand-elements.md`
   - `12-accessibility.md`
   - `13-product-messaging-canvas.md`
   - `14-product-messaging-canvas-career.md`
   - `15-product-messaging-mastery.md`
   - `16-product-messaging-igniteai.md`
   - `17-product-messaging-partner-program.md`
3. Set the Project Instructions (custom system prompt) to the text in `00-system-prompt.md`
4. Invite the marketing team to the project

### Usage patterns
- **"Review this email draft for brand compliance"** → Claude flags issues with specific rule citations and offers corrections
- **"Write a social post about Canvas Career for a Higher Ed audience"** → Claude applies voice/tone/style and pulls from the Canvas Career messaging framework
- **"What's the hex code for Mastery green?"** → instant answer from the knowledge files
- **"What's our elevator pitch for IgniteAI for a K-12 admin?"** → Claude pulls the IgniteAI messaging file and tailors to the audience
- **"Can I use the panda in this campaign?"** → Claude explains the policy and directs to brand team
- **"Draft a value prop paragraph for Mastery targeting State DoEs"** → Claude uses the Mastery messaging doc's State DoE narrative

---

## Alternative: Claude.ai Org-Wide Skill (future-state)

If Instructure has Claude.ai for Work with organization-level features, you can publish this as an **org-wide skill** that any team member can invoke with `/brand-guide`. This is more scalable but requires admin access to configure.

For now, a Project is the fastest path to value.

---

## Alternative: Claude Code + CLAUDE.md (for technical teams)

If anyone on the team uses Claude Code (the CLI), this bundle can serve as the codebase's `CLAUDE.md`. Place the system prompt content in `CLAUDE.md` at the root and the numbered files as context. This is already what the existing `Claude Design Bundle` folder approximates.

---

## Claude Design — The Next Phase (Not Now)

**What Claude Design is:** Anthropic Labs product (launched April 2026, available to Pro/Max/Team/Enterprise) that generates visual assets — slides, one-pagers, prototypes, social assets, marketing collateral — from text prompts, image uploads, and document context. It reads brand tokens from files and codebases to produce on-brand outputs. Exports to Canva, PDF, PPTX, and HTML.

**What Claude Design is NOT:** It is not an OCR tool and it does not extract content from existing images. Do not use it to close the visual/screenshot gaps (Category 2 in GAPS-AND-SOLUTIONS.md). Use plain Claude chat with image uploads for that.

**Why it matters for Instructure marketing:**
Once the brand guide Project is live and content gaps are closed, Claude Design becomes a powerful next layer:
- Marketers could generate on-brand slide decks, social graphics, or one-pagers with the brand guide as context
- Claude Design would read the hex codes, font names, logo rules, and composition guidance from the ai-ready files
- Output goes directly to Canva or PPTX — marketers aren't starting from blank templates

**Recommended sequence:**
1. ✅ Build the knowledge base (done — raw-scrape and ai-ready folders)
2. ✅ Close content gaps (in progress — see GAPS-AND-SOLUTIONS.md)
3. 🔲 Deploy Claude.ai Project for the team (priority 1 in gap tracker)
4. 🔲 Close visual/OCR gaps (priority 2)
5. 🔲 Evaluate Claude Design for asset creation (priority 9 — the next phase)

---

## What this bundle does NOT replace

- The live brand guide at https://sites.google.com/instructure.com/brandguide/home — always the authoritative source
- Human creative judgment on edge cases (especially panda, legal review)
- The Instructure brand team for escalations (brand@instructure.com / #brand-questions)

---

## Maintenance

| When | Action |
|------|--------|
| Live guide changes (major) | Re-scrape affected pages, update ai-ready files, bump version to v2026.2.0 |
| Minor updates (spelling, rule tweaks) | Edit affected ai-ready file, bump patch version, update "Last verified" date |
| New product added to ecosystem | Add to 01-brand-foundation.md + create new design system file |

The `raw-scrape/` folder is the audit trail — compare it to the live site to know what changed.

---

## File structure summary

```
brand-guide/
├── Brand Website Product Messaging Docs/   ← Source messaging docs (local copies)
│   ├── Canvas - All Product Messaging [MERGED].md
│   ├── Canvas Career _ Product Messaging Doc [FINAL].md
│   ├── IgniteAI Product Messaging Doc [FINAL].md
│   ├── Instructure Integration Tiers_Partner Segment _ Product Messaging Doc.md
│   ├── Mastery _ Product Messaging Doc [FINAL].md
│   ├── Higher Ed Conversation Cards.pdf    ← ⚠️ Not yet extracted
│   └── K12 Conversation Cards.pdf          ← ⚠️ Not yet extracted
│
├── raw-scrape/           ← One file per live page. Source of truth for scrape accuracy.
│   ├── home.md
│   ├── ecosystem.md
│   ├── brand-foundation.md
│   ├── voice-and-tone.md
│   ├── style-guide.md
│   ├── legal-stuff.md
│   ├── glossary.md
│   ├── quick-tips.md
│   ├── visual-brand-guide.md
│   ├── core-design-system-instructure.md
│   ├── core-design-system-canvas.md
│   ├── core-design-system-mastery.md
│   ├── core-design-system-parchment.md
│   ├── brand-elements-typography.md
│   ├── brand-elements-photography.md
│   ├── brand-elements-videography.md
│   ├── brand-elements-illustration.md
│   ├── brand-elements-iconography.md
│   ├── brand-elements-panda.md
│   ├── accessibility.md
│   └── external-links.md   ← All external URLs + local file cross-reference
│
└── ai-ready/             ← Upload these to Claude.ai Project
    ├── GAPS-AND-SOLUTIONS.md             ← ⭐ Living gap tracker — check every session
    ├── 00-deployment-recommendation.md   ← This file
    ├── 00-system-prompt.md               ← Project instructions (paste into Project Instructions field)
    ├── 01-brand-foundation.md
    ├── 02-voice-and-tone.md
    ├── 03-style-guide.md
    ├── 04-legal-and-quick-tips.md
    ├── 05-glossary.md
    ├── 06-visual-brand-overview.md
    ├── 07-design-system-instructure.md
    ├── 08-design-system-canvas.md
    ├── 09-design-system-mastery.md
    ├── 10-design-system-parchment.md
    ├── 11-brand-elements.md
    ├── 12-accessibility.md
    ├── 13-product-messaging-canvas.md     ← Canvas LMS, Studio, Catalog
    ├── 14-product-messaging-canvas-career.md
    ├── 15-product-messaging-mastery.md
    ├── 16-product-messaging-igniteai.md
    └── 17-product-messaging-partner-program.md
```
