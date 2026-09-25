---
name: firm-brain-builder
description: Required. Builds firm-brain.md — the operating brain your AI employees run on. Use at the start of Firm Brain pre-work, whenever firm-brain.md doesn't exist yet, or needs a refresh. ~20-25 minutes. Trigger on "firm brain," "start my firm brain," "let's do my firm brain," "firm brain pre-work," or any request to build, fill out, or create a firm brain file.
version: 2.0
---

# Firm Brain Builder

This skill builds `firm-brain.md` — the single file your three AI employees (Intake Coordinator, Email Manager, Operations Assistant) read before doing anything. It is the legal-practice equivalent of a new hire's training manual: what you practice, who you do it for, how you sound, how work actually flows through your firm, and where the hard lines are.

**This file is bigger than one event.** It should describe your real practice — every practice area, what's explicitly off the table, who your ideal client is, and what you actually deliver for them — not just the narrow slice needed to build three AI employees. You'll keep using Claude long after today, and this file is what makes every future use of it sound like your firm instead of a generic assistant.

This is a **required** module. Budget 20-25 minutes. The goal is a usable first draft — you can always refine it later, so don't let a tricky question stall you out.

## Before anything else — confirm the folder

Everything this training builds lives in one folder attached to this Cowork task, so your AI employees can find it later.

1. Check whether a folder is attached to this task. If none is, stop and say: "Before we start, attach the folder where you want your Firm Brain files to live. Tell me when it's attached." Don't ask any interview questions until a folder is attached.
2. Confirm out loud before writing anything: "I'll save your files in [folder name]/about-me/. Sound good?" Create `about-me/` if it doesn't exist yet.
3. Save every file this skill creates in that `about-me/` folder — never the folder root, a temporary location, or anywhere else.

## Before you start

Check whether `about-me/firm-brain.md` already exists. Check also whether the attorney has a completed **Firm Brain Prep Sheet** (the fillable Word doc version) — uploaded, pasted, or mentioned as already filled out. Also ask whether they'd rather talk through their answers than type them.

Then pick a path:

- **No existing file, no Prep Sheet, no voice memo → Path A (Interview).**
- **A completed (or partial) Prep Sheet, or a voice memo transcript, exists → Path B (Gap-Check).**
- **`firm-brain.md` already exists → tell them what you found and ask if they want to redo it fully, gap-check it against the current questions, or leave it alone.**

Never assume — ask in one line if it's not obvious which path applies.

### Voice memo option

Offer this up front: "If you'd rather talk through this than type, record yourself out loud answering the Firm Basics and the 9 questions — your phone's voice memo app is easiest, or your computer's dictation tool. Most transcribe automatically; if not, dictate into a Notes app. Upload or paste the resulting transcript here instead of doing the typed interview."

Treat an uploaded transcript as a Path B input, same as a Prep Sheet.

**Bonus:** since Writing Rules is required for this kit, this transcript can double as one of the three writing samples that module needs — mention this so they don't have to record a second one.

---

## Path A — Interview (default, no prep sheet)

Walk through Firm Basics, then the 9 core questions, **one at a time.** Do not front-load all 9 in one message — this is a conversation, not a form dump.

After EVERY answer, write it to `about-me/firm-brain.md` immediately using the template below, marking every not-yet-reached section `[not yet answered]` when you first create the file. Don't batch writes to the end — if the session gets interrupted, whatever's answered so far should already be saved.

If they're resuming a paused session: "Welcome back — you've finished [n] of 9 questions. Picking up at Question [x]: [topic]." Don't re-ask anything already answered.

### Step 0 — Firm Basics

Ask for these together, since they're quick facts, not reflection:

1. Your name
2. Your title/role
3. Bar admission(s) and jurisdiction(s) — this matters beyond identity: it determines which state's ethics rules your AI employees cite later
4. Firm name
5. Firm address
6. Firm size (attorneys and staff)

Write these into the **Firm Basics** section immediately.

### Step 1 — The 9 core questions

**Q1 — Legal Services, Practice Areas & Limits**
"What legal services do you provide, and what's explicitly off the table?"
- Name every practice area you actually work in — not just the busiest one.
- Within each, what specific services do you provide?
- What matter types or practice areas do you explicitly not take, and why?
- Anything you used to take but no longer do, or are winding down?

**Q2 — Ideal Client & Legal Solution**
"Who's your ideal client, and what's the legal solution you actually deliver?"
- Describe your ideal client concretely — their situation, not adjectives.
- What's the specific legal problem, fear, or situation that actually brings someone to you?
- What's genuinely different for them once the matter is resolved?
- Who's NOT a good fit — a case type, jurisdiction, or client expectation mismatch?
- Separately: is there a client *behavior* pattern that's a bad fit regardless of case value — excessive contact, distrust of your judgment, high-conflict dynamics?

**Q3 — Voice & Communication Style**
"How do you actually sound when you talk to clients?"
- Formal and buttoned-up, plain-spoken and warm, or somewhere in between?
- Any phrases, disclaimers, or sign-offs you always include?
- What would sound obviously wrong coming from you if an AI wrote it in your voice?

Then say: "Let's sanity-check your voice against a starter list of things that make writing sound AI-generated. Read through it and tell me what to cut, what to keep, and anything to add." Paste the Starter Anti-AI Kill List below. Let them edit it live — don't ask them to write one from scratch. Write their edited version into the file.

> **Note:** This captures a quick tone description, not a full writing sample — Writing Rules (required in this kit) is where the real samples live, three of them, across client-facing, social/marketing, and transcript/spoken registers. Don't ask for a full sample here. If they've already built writing-rules.md, pull the tone from there instead of re-asking, and go straight to the Kill List check.

**Q4 — Client Intake & Case Journey**
"Walk through the full client journey, from first contact through case resolution."
- How does a prospective client first reach you?
- What happens between first contact and a signed retainer — consult, documents, deposit paid?
- What else disqualifies someone at intake — conflicts, capacity, jurisdiction?
- Does the process look different by practice area? Describe each briefly if so.
- What happens during active representation, in broad strokes?
- How does a matter actually end — is there a closing conversation?
- If you ever need to end representation before resolution, what's the process?

**Q5 — Client Communications & Review Rules**
"What are the client emails you send most often, and what should never go out without you seeing it first?"
- Name the 3-5 client communications you send most.
- Is there boilerplate or a disclaimer you include in most of these?
- What must never be sent without your personal review?

**Q6 — Team & Tools**
"Who's on your team, and who owns what?"
- Name each team member, their role, and what they actually own. Solo is a valid answer.
- Who handles intake calls today, and what do they ask?
- Who drafts documents, and which types are theirs versus yours?
- Any VAs or contractors, and what are they responsible for?
- How does the team communicate?
- What software do you use for case management, calendaring, e-signature, or billing?

**Q7 — AI Boundaries & Escalation Rules**
"What are the hard boundaries for AI in your practice?"
- What should AI never do on its own?
- Any confidentiality or ethics rules in your jurisdiction you're already tracking around AI use?
- When something's uncertain, who should it get flagged to, and how?
- Is there a current caseload capacity limit worth flagging?

**Q8 — Fee Structure**
"What's your fee structure?"
- Flat fee, hourly, or contingency — does it change by practice area?
- Typical retainer or deposit amount, and how it's collected.
- Are there stages billed separately — a trial, a bail hearing, an appeal?
- Anything unusual — payment plans, sliding scale, case-type minimums?

**Q9 — Event-Day Goals**
"If your three AI employees worked perfectly, what would actually change about your week?"
- What's the single task eating the most time right now that you'd want gone first?
- What would you personally stop doing if intake, email, and ops ran themselves?

### Step 2 — Wrap up

Show the finished `firm-brain.md` and ask: "Here's your Firm Brain. Anything you'd change, add, or that feels off before we move on?" Make any edits requested.

Then tell them directly: "One standing rule is built into your Firm Brain: whenever this folder is attached, anything I create for a client or matter gets saved in `outputs/<client-or-matter-name>/`, named `YYYY-MM-DD-short-description` with the right extension. If I can't tell which matter something belongs to, I'll ask before saving."

---

## Path B — Gap-Check (prep sheet, existing file, or voice memo transcript)

1. Read the whole thing first.
2. Map every answer onto the template below, section by section. For a spoken transcript, read it all before mapping — it won't follow question order.
3. Flag anything thin or missing: a vague answer, a skipped question, a contradiction between sections.
4. Ask ONLY about the thin/missing items, one at a time. Don't re-ask what's already solid.
5. Write every clarified answer into `about-me/firm-brain.md` as you go.
6. When done, say plainly which sections you gap-checked and which you left as-is.

If the input is too thin or rambling to gap-check with confidence, say so honestly and offer to run Path A instead.

---

## Output file: about-me/firm-brain.md

```markdown
# Firm Brain — {{FIRM_NAME}}

## Firm Basics
- **Name:** {{name}}
- **Title/Role:** {{role}}
- **Bar Admission(s) & Jurisdiction(s):** {{bar admissions}}
- **Firm Name:** {{firm_name}}
- **Firm Address:** {{address}}
- **Firm Size:** {{size}}

## 1. Legal Services, Practice Areas & Limits
{{answer}}

## 2. Ideal Client & Legal Solution
{{answer}}

## 3. Voice & Communication Style
{{answer}}

### Anti-AI Kill List
{{their edited list}}
Golden rule: if this attorney's real voice and this list conflict on a specific phrase, their voice wins.

## 4. Client Intake & Case Journey
{{answer}}

## 5. Client Communications & Review Rules
{{answer}}

## 6. Team & Tools
{{answer}}

## 7. AI Boundaries & Escalation Rules
{{answer}}

## 8. Fee Structure
{{answer}}

## 9. Event-Day Goals
{{answer}}

## Standing File Rule
Whenever this folder is attached to a Cowork task, save every new deliverable in `outputs/<client-or-matter-name>/`, named `YYYY-MM-DD-short-description` with the right extension — never the folder root and never `about-me/`. If it isn't clear which matter a file belongs to, ask before saving. Firm Brain files stay in `about-me/`.
```

## Starter Anti-AI Kill List (paste this for Q3)

```
BANNED OPENERS: "Great question!", "Certainly!", "I'd be happy to help with that.",
"Please be advised that...", "In today's fast-paced legal environment..."

BANNED FILLER: "It's worth noting that...", "At the end of the day...", "That said..."

BANNED CORPORATE-SPEAK: "leverage" (as a verb), "circle back", "touch base",
"move the needle", "robust", "holistic", "game-changer"

BANNED STRUCTURAL TELLS: opening a sentence with an em-dash, closing with "I hope this
helps! Let me know if you have any questions." without a real question

BANNED TONE TELLS: flattering the reader in the first sentence, over-qualifying
("This is just my opinion, but..."), writing bland enough it could be from any attorney
```

Golden rule, always: if the attorney's actual voice conflicts with this list on a specific phrase, their voice wins.

## Set up the rest of the folder

Create two subfolders alongside `about-me/` if they don't already exist:

`templates/README.md`: "Drop your firm's actual documents here when you have them — retainer agreements, engagement letters, standard motions, letterhead, intake forms. Not required today. Add these whenever you have them."

`branding/README.md`: "Drop brand guidelines here later — logo files, color hex codes, fonts, tagline. Optional. Add anytime."

Show the folder structure so far, then say: "Firm Brain is done — the required piece. Writing Rules, About Me, and Brand Kit are also required today; How I Work is optional if there's time."

## Hard rules for this skill

- Never invent an answer on the attorney's behalf. If something's unclear, ask — don't guess and write it down as fact.
- Never skip straight to Path B logic without confirming a prep sheet or transcript actually exists.
- Always write to file after each answer, not at the end.
- Always flag, out loud, any answer that seems to contradict an earlier one in the same file.
- The Standing File Rule section in the output template is fixed — it goes in unedited, every time.

## Version notes

v2.0 — Folder-check gate, `about-me/` file location, Standing File Rule, voice-memo option, and pause/resume language, matching the pattern used across this kit. Writing Rules is required in this kit, so Q3's note points to it as required.
