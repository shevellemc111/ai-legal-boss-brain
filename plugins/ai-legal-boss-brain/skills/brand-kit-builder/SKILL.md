---
name: brand-kit-builder
description: Required. Builds brand-kit.md and stores the firm's actual letterhead file, so every AI employee that drafts correspondence or agreements uses the real brand colors, fonts, letterhead, and bar-required disclosures instead of guessing. ~10-15 minutes. Trigger on "brand kit," "my brand," "letterhead," "brand colors," or any request to build or fill out a brand file.
version: 1.1
---

# Brand Kit Builder

`firm-brain.md` is the firm's mechanics. `writing-rules.md` is the voice. `about-me.md` is the attorney. This file is the **visual identity and required disclosures** — colors, fonts, logo, letterhead, bar number, attorney-advertising language — so anything an AI employee drafts (a letter, an agreement, a document) actually looks like it came from this firm and carries what the bar requires it to carry.

Required for this training, alongside Firm Brain, Writing Rules, and About Me — a drafted letter or engagement letter that's missing a bar-required disclosure or the attorney's registration number is a real problem, not a style miss.

Budget about 10-15 minutes.

## Before anything else — confirm the folder

Everything this training builds lives in one folder the attorney attached to this Cowork task, so their AI employees can find it later.

1. Check whether a folder is attached to this task. If none is, stop and say: "Before we start, attach the folder where you want your Firm Brain files to live (for example, a folder named My Firm Brain). Tell me when it's attached." Don't ask any interview questions until a folder is attached.
2. Confirm out loud before writing anything: "I'll save your files in [folder name]/about-me/. Sound good?" Create `about-me/` if it doesn't exist yet.
3. Save every file this skill creates in that `about-me/` folder, including any letterhead and logo files uploaded — never the folder root, a temporary location, or anywhere else. If the attorney asks for a different location, use it, and tell them plainly that their AI employees look in `about-me/` by default.

## Before you start — pre-work check

Check whether `about-me/brand-kit.md` already exists.

- **It exists already** → tell them what you found and ask if they want to redo it, update a piece, or leave it alone.
- **It doesn't exist yet, but the Firm Brain Pre-Work Packet already has Brand Kit answered** → ask first: "I found your pre-work on Brand Kit. Want me to use it and only ask about what's missing, or would you rather answer these 11 questions fresh?"
  - **Use the pre-work:** map every answer onto the template, flag anything thin or missing (no hex color given, no bar number, etc.), then ask only about the gaps, one at a time. Say up front how much is covered: "From your pre-work, [n] of 11 are answered. Let's cover: [list]." If a letterhead or logo file was mentioned in the pre-work but not actually attached, ask them to upload it now — a described file doesn't substitute for the real one (see Hard rules).
  - **Answer fresh:** ask all 11, in order, and don't pull from the pre-work while doing it.
- **Neither exists** → ask all 11, in order, per below.

**Switching mid-stream, either direction:**
- Answering fresh and they say something like "just use my pre-work" — switch right away. Keep whatever they've already answered live (it wins over the pre-work on anything both cover), fill the rest in from the pre-work, and say where that leaves things: "Between what you've answered here and your pre-work, [x] of 11 are done. I just need you on: [list]." Then ask only the remaining gaps.
- Gap-checking the pre-work and they'd rather answer the rest fresh — switch back just as readily, and stop pulling from the pre-work for anything not yet asked.

## How to run it

One question at a time. Save to `about-me/brand-kit.md` as you go. If a letterhead file gets uploaded, save the actual file too (see Output below) — the .md file describes the brand, it doesn't replace the real letterhead document.

Ask, in order:

**1. Letterhead — do you already have one?**
"Do you have an existing letterhead template — a Word doc, PDF, or export you already use for correspondence and filings? If so, upload it now. If not, that's fine — say so and we'll build the header from your brand basics instead."

If uploaded: confirm the file type and save it (see Output). You can pull colors, fonts, and header layout straight from the document itself rather than re-asking questions 3-6 — only ask those if something's genuinely missing (e.g., it has a logo but no clear hex colors).

If not uploaded, continue through the rest in order.

**2. Firm name for the header**
"What's the exact firm name as it should appear on formal documents — the one on your letterhead, your bar registration, or your LLC/PC filing? Is that the same as what you go by day to day, or different?"

**3. Logo**
"Do you have a logo file (PNG, JPG, or SVG)? Upload it if so. If not, no problem — we'll use your firm name in text instead."

**4. Brand colors**
"What are your firm's colors? Hex codes if you know them (like #6E1423) are ideal, but 'navy and gold' works fine too — I'll match the closest hex values."

**5. Fonts**
"Do you have specific fonts you use for headings and body text? If you're not sure, say so — I'll use a clean, professional default."

**6. Header info for documents**
"What should appear in the header of a formal document — firm name, address, phone, email, website? Give me exactly what you want shown, in the order you want it."

**7. Signature block — bar-required items**
"When a document is signed on your behalf, what should the signature block show — your name, title, bar registration/attorney ID number, and the states you're admitted in? Give me it exactly as it should appear. This one matters: most jurisdictions require your bar number and admission state(s) on formal correspondence and filings."

**8. Required attorney-advertising disclosures**
"Does your jurisdiction require specific language on marketing or client communications — something like 'Attorney Advertising,' a 'prior results do not guarantee a similar outcome' disclaimer, or a specific disclosure your bar association requires? If you're not sure of the exact wording, tell me your bar admission state(s) here and I'll flag this for you to verify against your own bar's current advertising rules before it goes on anything — I won't guess at exact required wording."

**9. Preferred file format**
"When a document is finished, do you want it delivered as a Word doc, a PDF, or both? Any naming convention you already use?"

**10. Tagline — optional**
"Do you use a tagline on marketing materials? Skip if not — and if you have one, this is not the place for anything a bar would treat as a guarantee of outcome; flag that concern if the tagline reads that way."

**11. Anything else brand-specific**
"Anything else — a specific way your firm name must always be written, colors or styles to avoid, an old logo version that should never be used? Skip if nothing comes to mind."

## Output

**1. Save the actual letterhead/logo files, if provided**, in `about-me/` alongside `brand-kit.md` (not just described in the text) — these are what actually get used when drafting, the .md file is the index.

**2. Save `about-me/brand-kit.md`:**

```markdown
# Brand Kit — {{FIRM_NAME}}

## Letterhead
{{"On file: [filename] — use this as the base for all drafted documents." OR "No letterhead on file — build headers from the brand basics below."}}

## Firm name for formal documents
{{exact name}}

## Logo
{{"On file: [filename]" OR "No logo on file — use firm name in text."}}

## Brand colors
- **Primary:** {{name/description}} — {{hex if known}}
- **Secondary:** {{name/description}} — {{hex if known}}

## Fonts
- **Headings:** {{font or "not specified — use a clean professional default"}}
- **Body:** {{font or "not specified — use a clean professional default"}}

## Document header
{{exactly what they specified, in their order}}

## Signature block (bar-required items)
{{exactly as specified — name, title, bar registration/attorney ID number, admission state(s)}}

## Attorney-advertising disclosures
{{whatever they gave, flagged for their own verification if the exact wording wasn't confirmed — "Attorney admitted in: {{state(s)}}. Exact required advertising disclosure language not confirmed here — verify current wording against {{state}} bar advertising rules before use." if applicable, or "None specified — verify with your own jurisdiction's advertising rules before relying on this file's silence as 'nothing required.'"}}

## File format & naming
- **Preferred format:** {{Word / PDF / both}}
- **Naming convention:** {{if given, or "Not specified — use YYYY-MM-DD-description as default"}}

## Tagline
{{tagline, or "None"}}

## Other brand rules
{{list, or "None specified"}}
```

## How other AI employees use this

Any skill that drafts a document under this firm's name — Intake Coordinator drafting an agreement, Email Manager drafting correspondence — checks for `brand-kit.md` and the letterhead file first:

1. **Letterhead on file** → draft on it directly.
2. **No letterhead, but colors/fonts/header specified** → build a clean header from those specifics.
3. **`brand-kit.md` doesn't exist at all** → fall back to firm name and address from `firm-brain.md`. Never invent colors, a logo, a letterhead, a bar number, or a required disclosure that wasn't provided.

Signature-block bar numbers and admission states, and any attorney-advertising disclosure this file gives, are not optional flourishes — include them on every document brand-kit.md says they belong on, the same way a hard rule gets followed, not treated as a style preference to skip under time pressure.

## Hard rules for this skill

- Never invent a hex color, a font, a bar number, a signature block, or a required disclosure that wasn't given. "Not specified" is a valid, honest answer — guessing at what looks "professional enough" or "probably required" is not.
- Never guess at the exact wording of a bar advertising disclosure. If the attorney doesn't have it on hand, record their admission state(s) and flag it for their own verification — don't fabricate disclosure language and present it as compliant.
- Never redraw or recreate a logo from a description — only use an actual uploaded logo file. A described logo with no file gets "no logo on file," not an invented one.
- If a letterhead file is uploaded, save the real file — don't just transcribe what it looks like into markdown. Other skills need the actual document to draft on.
