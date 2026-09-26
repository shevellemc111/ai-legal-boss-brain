---
name: writing-rules-builder
description: Required. Builds writing-rules.md from three real writing samples across different registers, so AI-drafted content actually sounds like this attorney. Use after firm-brain.md exists (or alongside it). Trigger on "writing rules," "my writing samples," "voice module," "writing rules pre-work," or any request to build writing rules or capture voice/writing samples.
version: 2.1
---

# Writing Rules Builder

Firm Brain Q3 is a quick snapshot: a described tone, a couple of example lines, an edited kill list — no full sample. This skill is the deep version — it collects real writing across three different registers and hands back a voice profile the attorney confirms or corrects, instead of working from a described tone alone.

This module is **required** for every attorney at this training, the same as Firm Brain and About Me. Voice work carries real weight here: a client letter drafted in the wrong voice is a bigger problem for a law firm than for most businesses, and "sounds roughly professional" isn't the bar — "sounds like this attorney" is.

Budget 20-25 minutes.

## Before anything else — confirm the folder

Everything this training builds lives in one folder the attorney attached to this Cowork task, so their AI employees can find it later.

1. Check whether a folder is attached to this task. If none is, stop and say: "Before we start, attach the folder where you want your Firm Brain files to live (for example, a folder named My Firm Brain). Tell me when it's attached." Don't ask any interview questions until a folder is attached.
2. Confirm out loud before writing anything: "I'll save your files in [folder name]/about-me/. Sound good?" Create `about-me/` if it doesn't exist yet.
3. Save every file this skill creates in that `about-me/` folder — never the folder root, a temporary location, or anywhere else. If the attorney asks for a different location, use it, and tell them plainly that their AI employees look in `about-me/` by default.

## Before you start — pre-work check

Check whether `about-me/writing-rules.md` already exists.

- **It exists already** → tell them what you found and ask if they want to redo it, add a sample, or leave it alone.
- **It doesn't exist yet, but the attorney's Firm Brain Pre-Work Packet already has one or more of the three writing samples filled in or attached** → ask first: "I found sample(s) in your pre-work. Want me to use what's there and only ask for what's missing, or would you rather give me all three fresh?"
  - **Use the pre-work:** take the samples that are there as-is, then ask only for the missing register(s), one at a time. Say up front which registers are covered: "From your pre-work, [n] of 3 samples are in — [list which]. I just need: [list what's missing]."
  - **Answer fresh:** collect all three now, one at a time, and don't pull from the pre-work while doing it.
- **Neither exists** → collect all three now, per Step 1 below.

**Switching mid-stream, either direction:**
- Collecting fresh and they say something like "just use my pre-work" — switch right away. Keep whatever sample(s) they've already given you live (those win over the pre-work if both cover the same register), pull the rest from the pre-work, and say where that leaves things: "Between what you've given me here and your pre-work, [x] of 3 are in. I just need: [list]." Then ask only for what's still missing.
- Gap-checking the pre-work and they'd rather give the rest fresh — switch back just as readily, and stop pulling from the pre-work for anything not yet collected.

## Step 1 — Collect three samples, one per register

Ask for three writing samples, explicitly across these three registers — not three examples of the same kind of writing:

1. **Client/case correspondence** — a real email or letter sent to an actual client (redact or paraphrase anything privileged you don't want pasted into this session — the writing style is what matters, not the client's details).
2. **Marketing/content** — a real newsletter, social post, website bio, or blog piece, if the firm does any of that. If the firm truly does none, substitute a firm announcement, a bar association bio, or anything client-facing that isn't case-specific.
3. **Transcript / spoken-to-written** — a voice memo transcript, dictation to staff, or notes spoken and then typed up. This one matters because it usually reveals rhythm and word choice that polished writing hides.

Accept samples pasted directly, uploaded as files, or described and then pasted. Take what's actually offered — don't demand all three be perfect or lengthy; a short but real sample beats a long invented one.

**Already have a voice memo transcript from Firm Brain or About Me?** That covers the transcript/spoken register — don't make them record a second one. Pull it in here and just collect the client-correspondence and marketing samples fresh.

### If they don't have samples ready

Don't block. Offer, in order:

1. "Pull one up right now — a client email you already sent, an old newsletter, anything real. Paste it here (redact privileged specifics if needed — the wording style is what I'm after)." This is the fastest fix and covers most attorneys.
2. If that's still not possible for a given register, get a short live sample instead: ask them to write two or three sentences right now as if they were actually sending it (e.g., "write me a line like you're telling a client their hearing got pushed a week"). A live sample beats no sample.
3. Only skip a register entirely if both of those fail, and say plainly in the output that register wasn't covered and drafts in that register should be treated as unverified until a real sample is added later.

## Step 2 — Analyze, don't guess

Read all three samples together and look for real, repeatable patterns — not vibes. Specifically:

- **Sentence rhythm** — average sentence length, whether they favor short direct sentences or longer ones, how formal the punctuation is.
- **Vocabulary** — words and phrases that show up more than once, anything distinctly "them," legal shorthand they use naturally versus terms they always spell out for clients.
- **Structure** — paragraph length, whether they use headers or numbered points in client letters, how they open and close correspondence (salutation style, sign-off).
- **Recurring phrases** — a signature way of softening bad news, a way they reassure a client, a consistent sign-off.
- **How it shifts by register** — what changes between client correspondence, marketing, and the transcript/spoken sample. Most attorneys are noticeably more formal in client correspondence and looser in marketing or spoken material. Name the specific differences, don't just say "more casual."

## Step 3 — Present findings for confirmation, not as a final answer

Show your analysis back to them in plain language, organized as:

- **Overall voice** — 3-5 sentences describing how they write across contexts, using specifics from their actual samples, not generic adjectives.
- **By register:**
  - Client/case correspondence: {{specific observations}}
  - Marketing/content: {{specific observations}}
  - Transcript/spoken: {{specific observations}}
- **Recurring phrases/vocabulary found**
- **Anything surprising or worth flagging** (e.g., "your client letters and your newsletter read like two different people — is that intentional?")

Ask directly: "Does this sound like you? Anything wrong, missing, or that you'd word differently?" Iterate on their corrections before finalizing. Never treat your first-pass analysis as done without this check — the whole point of this module is accuracy over a guess.

## Step 4 — Reconcile with the Firm Brain Q3 kill list

If `about-me/firm-brain.md` already has a Q3 Anti-AI Kill List, pull it in as-is — don't rebuild it from scratch. Note explicitly in the output: "This file goes deeper than the Firm Brain Q3 snapshot. The kill list from Q3 still applies — see firm-brain.md — this file adds the register-specific voice detail Q3 doesn't cover."

If `firm-brain.md` doesn't exist yet or Q3 hasn't been done, use the same Starter Anti-AI Kill List from firm-brain-builder and let them edit it here instead, then note it should also get copied into firm-brain.md's Q3 when that module runs.

## Output file structure

Save to `about-me/writing-rules.md`:

```markdown
# Writing Rules — {{ATTORNEY_OR_FIRM_NAME}}

## Overall voice
{{3-5 sentence summary, specific to this attorney}}

## By register

### Client/case correspondence
{{observations + 1 illustrative line pulled from their own sample, redacted of client specifics}}

### Marketing/content
{{observations + 1 illustrative line pulled from their own sample}}

### Transcript / spoken
{{observations + 1 illustrative line pulled from their own sample}}

## Vocabulary & recurring phrases
- **Words/phrases they reach for:** {{list}}
- **Words/phrases they'd never use:** {{list, if known}}
- **Legal shorthand used naturally vs. always spelled out for clients:** {{notes}}

## Structural habits
- Paragraph length: {{}}
- Salutation/sign-off style: {{}}
- Headers or numbered points in client letters: {{yes/no, how}}

## Anti-AI Kill List
(Pulled from firm-brain.md Q3 if it exists — otherwise built here and flagged for copy-back.)
{{list}}

## Legal filings and formal court documents
Always stay in the firm's formal legal-writing register, regardless of what these registers cover. Marketing tone and casual/spoken rhythm never apply to a filing, a motion, or formal court correspondence — that's the register working correctly, not a violation of "sounding like this attorney."

## When breaking the rules is OK
- When they're deliberately being direct or informal with a client who prefers that — match that tone.
- When a legal term of art is the correct, precise word — use it plainly, don't dress it up or dumb it down past accuracy.
- When it's a real firm announcement, not hype — a direct, plain headline is fine.

**Golden rule:** if this attorney's actual voice conflicts with the kill list on a specific phrase, their voice wins. The kill list is a floor, not a ceiling.

## Coverage note
{{Which of the 3 registers had a real sample vs. a live/substitute sample vs. was skipped — be honest here so future drafts in an unverified register get extra review.}}
```

## Hard rules for this skill

- Never fabricate a writing sample or fill in a register with invented text. If a register wasn't covered, say so in the Coverage note — don't paper over the gap.
- Always show the analysis back for confirmation before saving as final. Skipping this step is exactly the kind of thing that leads to a voice profile that doesn't actually sound like the attorney.
- Don't overwrite an existing Q3 kill list in firm-brain.md from here — read it in, don't replace it, unless the attorney explicitly asks to redo it.
- Never let a client-correspondence sample's content override privilege or confidentiality — if a pasted sample contains sensitive client detail, use it for style only and don't repeat the specifics back in the output file.
- Legal filings and formal court documents always stay in the firm's formal register — never apply the marketing or transcript/spoken register there, no matter what those samples show.

## Version notes

v2.0 — Required module built on a 3-sample pattern (client-facing, marketing/content, transcript/spoken). Legal-correspondence register is one of the three required samples; Firm Brain Q3's kill list stays the source of truth and gets pulled in here, not rebuilt. Includes the "legal filings always stay formal" rule and a privilege/confidentiality guard on client-correspondence samples.

v2.1 — Added the pre-work choice-and-switch behavior: if the Firm Brain Pre-Work Packet already has the three writing samples, ask whether to use them and only fill gaps, or answer fresh, and support switching either direction mid-session.
