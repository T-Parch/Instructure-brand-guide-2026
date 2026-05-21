# Instructure Brand Guide AI System — Gaps & Solutions Tracker
**Living document** — update every session. Check this file at the start of any brand guide work.
**Last updated:** 2026-04-29

---

## How to read this tracker

Each gap has a **status**, a **solution path**, and an **owner or next step**. The goal is that no gap is ever just "unknown" — everything has a path forward even if the path is "waiting on Trevor."

| Status | Meaning |
|--------|---------|
| 🔴 Open | Not resolved, blocking completeness |
| 🟡 Partial | Workaround exists but gap remains |
| 🟢 Resolved | Content captured, in ai-ready files |

---

## Category 1: Content Gaps (pages/docs not yet in the system)

| # | Gap | Status | Solution | Owner / Next Step |
|---|-----|--------|----------|------------------|
| 1.1 | Parchment product messaging doc | 🔴 Open | The Parchment messaging doc was not in the downloaded folder. Likely exists in Drive — check with brand team. | Trevor to locate and download |
| 1.2 | Intelligent Insights messaging doc | 🔴 Open | Referenced on the ecosystem page but no standalone messaging doc found locally. | Trevor to request from product marketing |
| 1.3 | Impact messaging doc | 🔴 Open | Same as 1.2 — referenced in ecosystem, no messaging doc found. | Trevor to request from product marketing |
| 1.4 | LearnPlatform messaging | 🔴 Open | "Coming soon" on the live site — may not exist yet. Monitor. | Check quarterly |
| 1.5 | Canvas Catalog standalone messaging doc | 🟡 Partial | Catalog content is partially covered in the Canvas Career doc (better-together story) and the Canvas merged doc (Studio/Catalog/Career/LMS). Standalone doc may exist in Drive. | Trevor to check if a Catalog-specific doc exists |
| 1.6 | IgniteAI logo download link | 🔴 Open | Referenced in ecosystem page ("Download logo") but URL not captured by scraper. | Check brand@instructure.com or #brand-questions |
| 1.7 | Intelligent Insights logo download | 🔴 Open | Same as 1.6 | Same as 1.6 |
| 1.8 | Impact logo download | 🔴 Open | Same as 1.6 | Same as 1.6 |
| 1.9 | Higher Ed Conversation Cards (PDF) | 🟡 Partial | File downloaded locally (`Higher Ed Conversation Cards.pdf`) but not yet read into ai-ready files. | Read PDF and extract key content into ai-ready file or append to 13-product-messaging-canvas.md |
| 1.10 | K-12 Conversation Cards (PDF) | 🟡 Partial | File downloaded locally (`K12 Conversation Cards.pdf`) but not yet read into ai-ready files. | Same as 1.9 |
| 1.11 | Partner pitch deck (Master) | 🔴 Open | Referenced in Partner messaging doc: https://docs.google.com/presentation/u/0/d/1Hkn7ah8o8SvmgEPrV012IGF_hflIf2knkqAPzXDPwxQ/edit — requires auth. | Trevor to download slides and add key content |
| 1.12 | Instructure/Canvas/Mastery/K-12 Conversation Cards linked in IgniteAI and Mastery docs | 🔴 Open | Multiple Google Slides conversation card decks referenced by URL in the messaging docs. Require auth to access. | Trevor to download and share |

---

## Category 2: Visual / OCR Gaps (brand specs locked in images)

| # | Gap | Status | Solution | Owner / Next Step |
|---|-----|--------|----------|------------------|
| 2.1 | Typography specimens (LL Circular weights, sizes, usage examples) | 🟡 Partial | Text specs captured (foundry, 4 of 8 weights, min sizes). Visual specimens showing the typeface in use are image-only on the live site. | Upload screenshots from `Brand Website Core Design System - Screen Shots` folder directly into a Claude conversation; ask Claude (vision) to extract all visible text and specs |
| 2.2 | Color swatch labels and exact palette combinations | 🟡 Partial | Hex codes captured for all 5 brand systems. Swatch arrangement, named tones, and combination examples in images. | Same as 2.1 — use Claude vision on screenshots |
| 2.3 | Logo dos/don'ts visual examples | 🟡 Partial | Rules captured in text. Visual examples of correct vs. incorrect usage are image-only. | Use Claude vision on screenshots; add descriptive notes to design system ai-ready files |
| 2.4 | Composition samples (per-product layout examples) | 🟡 Partial | Text descriptions captured. Actual layout images not extracted. | Use Claude vision on screenshots |
| 2.5 | Iconography examples (4 images, no alt text on live site) | 🔴 Open | The iconography page had 4 embedded images with no alt text — zero text extracted. | Upload screenshots from the Brand Website folder; Claude vision will extract visible specs |
| 2.6 | IgniteAI visual identity (purple gradient indicators, icon placement) | 🟡 Partial | Described in product messaging doc. Actual visual examples referenced in the doc with `[image1]` `[image2]` placeholders — those images are in the Drive version of the doc. | Request image exports from brand team, or screenshot from live Canvas UI |

### How to close visual gaps with Claude vision

**Step-by-step:**
1. Open a Claude.ai conversation (not Claude Code)
2. Upload screenshot images from `brand-guide/Brand Website Core Design System - Screen Shots/`
3. Prompt: "Extract all text visible in this image, including labels, values, color names, typeface names, and any specifications shown."
4. Copy the extracted content into the relevant ai-ready file (typography section, color section, etc.)
5. Note: Claude's vision runs in the chat — this is NOT what Claude Design does (see Category 5)

---

## Category 3: Auth-Walled Content (requires Instructure credentials to access)

| # | Gap | Status | Solution | Owner / Next Step |
|---|-----|--------|----------|------------------|
| 3.1 | Product messaging framework Google Docs (live versions) | 🟡 Partial | Local MD copies downloaded for Canvas, Mastery, IgniteAI, Canvas Career, Partner Program. Parchment, Intelligent Insights, Impact, LearnPlatform not downloaded. | Trevor to download remaining docs |
| 3.2 | Canvas Apps experience (listing management) | 🔴 Open | Referenced as a key partner program feature. Cannot access without auth. | Descriptive capture only — covered in messaging doc |
| 3.3 | LearnPlatform partner product library | 🔴 Open | Same as 3.2 | Same as 3.2 |
| 3.4 | Live Google Slides conversation card decks | 🔴 Open | Multiple decks referenced in messaging docs by URL. All require Instructure auth. | Trevor to download and export as PDF or MD |

---

## Category 4: Stale Content Risk

| # | Gap | Status | Solution | Owner / Next Step |
|---|-----|--------|----------|------------------|
| 4.1 | Brand guide live site last scraped 2026-04-28 | 🟢 Resolved (for now) | Full scrape completed. Raw files in `raw-scrape/` are the audit trail. | Re-scrape if live guide shows changes; check `03-source-map-and-gem-inclusion-rules.md` for versioning protocol |
| 4.2 | Product messaging docs are dated (Canvas Studio: Dec 2025, Mastery: Oct 2025, IgniteAI: Dec 2025, Canvas Career: Feb 2026) | 🟡 Partial | All docs captured at their stated version. Product messaging teams may have newer versions. | Check with messaging doc owners quarterly; Shelby Schaefer (Canvas/Career), Amy Haskell (Mastery), Deepa Prasad (IgniteAI), Sarah Cornelius (Partner) |
| 4.3 | IgniteAI Agent for Canvas flagged as "Coming soon" in messaging doc | 🟡 Partial | Noted as coming soon in 16-product-messaging-igniteai.md. May be live now — check. | Verify current product state; update messaging file when Agent is GA |

---

## Category 5: Deployment Gaps (system not yet live for the marketing team)

| # | Gap | Status | Solution | Owner / Next Step |
|---|-----|--------|----------|------------------|
| 5.1 | Claude.ai Project not yet created | 🔴 Open | All ai-ready files exist locally. Need to create the Claude.ai Project and upload files. | Trevor to create Project at claude.ai, upload files 00–17 from ai-ready/ |
| 5.2 | Marketing team not yet onboarded | 🔴 Open | Depends on 5.1 | Once Project created: share invite link with marketing team |
| 5.3 | No usage guidance doc for marketing team | 🔴 Open | The `00-system-prompt.md` and `00-deployment-recommendation.md` explain setup but there's no user-facing "how to use this tool" guide for the marketing team members themselves. | Create a simple 1-pager: how to start a chat, sample prompts for content creation vs. review mode |
| 5.4 | No feedback loop from marketing team | 🔴 Open | When the team uses the assistant, they'll find missing info or wrong answers. No mechanism to capture and route that back to improve the files. | Designate a Slack channel or shared doc for brand guide feedback; Trevor reviews monthly |

---

## Category 6: Claude Design — Role Clarification

| # | Question | Answer |
|---|---------|--------|
| 6.1 | Do the screenshot images need to be in the MD files? | No. Screenshots are a source for extracting text via Claude vision (see Category 2). They don't embed in MD files — Claude reads images in chat, not in Project knowledge files. |
| 6.2 | What does Claude Design do vs. what we need? | **Claude Design** (Anthropic Labs, April 2026) creates NEW visual assets — prototypes, slides, marketing collateral, one-pagers — using brand context you provide. It's for creation, not extraction. It accepts PPTX/DOCX/image uploads and reads brand tokens from codebases. **Best use case for Instructure:** Once the brand guide Project is live, marketers could use Claude Design to generate on-brand slides, social assets, or one-pagers — with the brand guide files as the context it reads. |
| 6.3 | Should we get Claude Design involved now? | Not yet for OCR. Use Claude vision (plain chat) to extract text from screenshots — that closes gap 2.x. **Then** evaluate Claude Design for asset creation once the brand guide Project is stable. Claude Design is the right next step *after* the knowledge base is complete. |
| 6.4 | What Claude Design needs from us to be useful | It would need: brand hex codes, LL Circular/Poppins font info, logo files (Drive links we already have), and the composition rules. All of that is now in the ai-ready files. So the path is: close content gaps → deploy Project → evaluate Claude Design for creation. |

---

## Summary: Priority Order to Close Gaps

| Priority | Action | Effort | Impact |
|----------|--------|--------|--------|
| 1 | **Create Claude.ai Project and upload ai-ready files** (gap 5.1) | Low | Unlocks the whole system for the team |
| 2 | **Close visual gaps with Claude vision on screenshots** (gaps 2.1–2.6) | Medium | Fills the most important visual spec holes |
| 3 | **Download and read the two Conversation Card PDFs** (gaps 1.9, 1.10) | Low | Adds persona/ICP depth to messaging files |
| 4 | **Download Parchment messaging doc** (gap 1.1) | Low | Completes the product family |
| 5 | **Request missing logo download links** (gaps 1.6–1.8) | Low | Completes external-links.md |
| 6 | **Create marketing team user guide** (gap 5.3) | Low | Reduces friction for first-time users |
| 7 | **Request Intelligent Insights and Impact messaging docs** (gaps 1.2, 1.3) | Medium | Expands platform enhancement coverage |
| 8 | **Set up feedback loop** (gap 5.4) | Low | Makes the system self-improving |
| 9 | **Evaluate Claude Design for asset creation** (gap 6.3) | Medium | Next phase of the rollout |
