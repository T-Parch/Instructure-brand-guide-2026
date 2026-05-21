# Gemini Gem setup — Instructure Brand Guide Assistant

**Bundle location:** `02-ai-ready/gemini-bundle/`
**Last built:** 2026-05-07
**Pairs with:** Claude Project files at the parent level (`02-ai-ready/00-system-prompt.md` through `17-...`)

---

## What's in the bundle

The `gemini-bundle/` folder contains 11 files:

- **1 instructions file** (`00-gemini-instructions.md`) — paste contents into the Gem's Instructions field. Do NOT upload as a knowledge file.
- **10 knowledge files** (`01-` through `10-`) — upload all 10 to the Gem's knowledge area.

Gemini Gems cap knowledge at 10 files. That's why this bundle exists separately from the Claude bundle (which uses 15 granular files).

---

## How to set up the Gem (one-time)

1. In the Gemini Gem builder, create a new Gem named **"Instructure Brand Guide Assistant."**
2. Open `gemini-bundle/00-gemini-instructions.md`. Copy everything below the first divider line and paste it into the Gem's **Instructions** field.
3. Copy the Description block from the same file into the Gem's **Description** field.
4. In the **Knowledge** section of the Gem builder, upload the 10 knowledge files: `01-brand-foundation.md` through `10-product-messaging-partner-program.md`. Drag-and-drop the whole set.
5. Save the Gem.

That's it. The Gem is now equivalent to the Claude Project in behavior, with content adapted for Gemini's retrieval model.

---

## What's consolidated and why

Gemini caps at 10 knowledge files. The Claude bundle has 15. Two consolidations make the math work without losing content:

| Gemini file | Sources merged from Claude bundle |
|---|---|
| `06-visual-and-accessibility.md` | `06-visual-brand-overview.md` + `07-logos-and-colors.md` + `11-brand-elements.md` + `12-accessibility.md` |
| `07-product-messaging-canvas-suite.md` | `13-product-messaging-canvas.md` + `14-product-messaging-canvas-career.md` |

Each consolidated file has a quick-navigation header so Gemini retrieval can route queries to the right section.

The remaining 8 files map 1:1 (some renumbered):

| Gemini file | Claude source |
|---|---|
| `01-brand-foundation.md` | `01-brand-foundation.md` |
| `02-voice-and-tone.md` | `02-voice-and-tone.md` |
| `03-style-guide.md` | `03-style-guide.md` |
| `04-legal-and-quick-tips.md` | `04-legal-and-quick-tips.md` |
| `05-glossary.md` | `05-glossary.md` |
| `08-product-messaging-mastery.md` | `15-product-messaging-mastery.md` |
| `09-product-messaging-igniteai.md` | `16-product-messaging-igniteai.md` |
| `10-product-messaging-partner-program.md` | `17-product-messaging-partner-program.md` |

---

## Maintenance

When the live brand guide changes:

1. Update the source files at the **parent level** of `02-ai-ready/` first. That's the canonical edit point.
2. Re-build the Gemini bundle so it stays in sync. Either run the build script (TBD — see note below) or manually:
   - Copy 1, 2, 3, 4, 5, 15, 16, 17 → bundle equivalents.
   - Re-concatenate 6+7+11+12 → `gemini-bundle/06-visual-and-accessibility.md`.
   - Re-concatenate 13+14 → `gemini-bundle/07-product-messaging-canvas-suite.md`.
3. Re-upload the changed knowledge files in the Gem builder. If you changed the instructions file, paste the new contents into the Gem's Instructions field.
4. Bump the version date in both `00-system-prompt.md` (Claude) and `gemini-bundle/00-gemini-instructions.md` (Gemini).

> **Note:** A build script can be added later to automate the re-build step. For now, the structure is simple enough to maintain by hand.

---

## What NOT to upload to the Gem

Same rule as Claude. These working docs stay local:

- `00-deployment-recommendation.md`
- `GAPS-AND-SOLUTIONS.md`

They live at the parent level of `02-ai-ready/` for your own reference. Don't include them in either assistant's knowledge.

---

## Why this structure

- **Drag-and-drop simplicity.** The Gem folder is self-contained. Open it, drag the 10 knowledge files into the Gem builder, paste the instructions content. Done.
- **No platform confusion.** Each AI platform has its own folder. You never have to remember "which files go to Gemini and which to Claude."
- **Single canonical source.** Edits start at the parent level (`02-ai-ready/`). The Gemini bundle is a rebuilt artifact. That keeps Claude as the source of truth and Gemini as a derivative — easier to maintain than two parallel canonical sets.

---

## Contacts

- Owner: Trevor Misina (Marketing AI)
- Brand escalations: brand@instructure.com · #brand-questions
