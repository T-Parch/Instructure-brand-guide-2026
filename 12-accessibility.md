# 12 — Accessibility
**Source:** https://sites.google.com/instructure.com/brandguide/accessibility
**Last verified:** 2026-05-07
**Version:** v1.0.0
**Note:** Accessibility moved to the top-level nav in May 2026 (was previously nested under Visual brand guide). Significantly expanded with new sections on structure, slide/email, alt text, meaningful links, and captions.

---

## We believe in accessibility for all

Just like learners, our customers (present and future) have a wide range of needs and abilities. We do everything we can to ensure everyone can experience and interact with our site, content, and products in the ways that work best for them.

The focus for design is **color, contrast, and legibility**, plus structure, alt text, links, and captions for content.

**Resources:** WebAIM is the go-to source for accessibility best practices. For Instructure-specific questions, use @marketing-a11y or #brand-questions.

---

## Color

The Instructure palette is a horizon of blues (a good color for accessibility) with deep Instructure Navy as the foundation.

## Contrast

Contrast is non-negotiable. Use the WebAIM Contrast Checker to verify ratios using hex codes.

**WCAG 2.0 AA** requires a contrast ratio of at least **4.5:1 for normal text**. The goal is for all copy and essential information (including logos and CTAs) to meet these ratios.

Sample: Instructure Sky (`#18c2ea`) on Instructure Navy (`#0b1722`) = 8.57:1.

### Color and contrast dos
- Text on solid color backgrounds, in approved Instructure tones
- WCAG 2.2: standard text **4.5:1** minimum
- Functional UI elements (button borders, icons, form fields) **3:1** minimum against background

### Color and contrast don'ts
- Don't use Mastery, Canvas, or Parchment product colors for headline text or other essential elements
- Avoid red+green combos (color blindness)
- Don't place typography or logos over photographs or illustrations
- Don't rely on color alone to convey meaning ("click the red button" — use icons or text labels too)

---

## Legibility and type scale

Following a simple type scale helps with accessibility, hierarchy, and clarity.

Sample: headline 48pt, body copy 24pt.

**Minimum digital type size: 12pt** (per the accessibility page). Set base at 12pt and move in 4pt increments (12, 16, 20, 24, 28…).

> ⚠️ Note: The typography page lists 16pt as the minimum. The two pages refer to different contexts — confirm with brand which applies for your asset (UI vs. body copy).

---

## Structure and headings (NEW — May 2026)

A digital document needs a logical flow. Proper heading structure lets screen readers navigate efficiently and understand section relationships.

- **Logical hierarchy.** Use only one `<h1>` per page (the main title). Follow with `<h2>` for sections, `<h3>` for subsections.
- **Don't skip levels.** Never jump from `<h2>` to `<h4>`. Consistency clarifies the information.
- **Tables.** Use tables for data only, never for layout.

---

## Slide and email design (NEW — May 2026)

Presentations and emails should provide a cohesive brand experience while staying accessible.

- **The template is key.** Use the Instructure core slide template. Don't modify it — especially not the prescribed colors or type sizes set by marketing and learning strategy.
- **Email simplicity.** Keep email layouts simple. Avoid complex tables for layout. Use 12pt as your base for body copy.

---

## Alternative text (NEW — May 2026)

Alt text provides a text-based bridge for visual elements.

- **Be descriptive.** Concise, meaningful descriptions for images that convey information (e.g., "Student using a laptop with a teacher looking on")
- **Decorative images.** If purely aesthetic, mark as decorative so screen readers can skip
- **Complex graphics.** For charts or diagrams, brief summary in alt text, full description in surrounding body copy

---

## Meaningful links (NEW — May 2026)

Links should be a clear path, not a guessing game. Raw URLs are difficult for screen readers.

- **No raw URLs.** Avoid long strings like "https://sites.google.com/…"
- **Descriptive text.** Use "Learn more about the state of learning" instead of "Click here"

---

## Captions and transcripts (NEW — May 2026)

All audio and video content must be accessible.

- **Captions.** All video content requires synchronized captions for D/deaf or hard of hearing viewers
- **Transcripts.** Provide text-based transcripts for audio and video as an alternative
- **Audio descriptions.** For videos with significant visual information or no dialogue, include a detailed audio description track or text-based narrative

---

## When AI flags accessibility risk

When reviewing or generating content, flag these for fixes:
- Color used as the only signal for meaning
- Contrast ratios below 4.5:1 (text) or 3:1 (UI elements)
- Skipped heading levels
- Raw URLs in body copy
- Missing alt text mentions for image-heavy content
- Video without captions/transcripts
- Tables used for layout instead of data

## Contact
- Email: brand@instructure.com
- Slack: #brand-questions, @marketing-a11y
