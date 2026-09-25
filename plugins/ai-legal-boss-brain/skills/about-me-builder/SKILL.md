---
name: about-me-builder
description: Required. Builds about-me.md — who this attorney is as a person and a practitioner, separate from how the firm runs. ~15 minutes. Trigger on "about me," "my about-me file," "about me pre-work," or any request to build or fill out an about-me file.
version: 1.0
---

# About-Me Builder

`firm-brain.md` is about the firm — practice areas, clients, fees, process. This file is about the **attorney running it**: how they think, what they're juggling, how they learn, and what's made AI actually useful for them before. Claude reads this alongside `firm-brain.md`, but it's a separate file and a separate section of the interview — don't merge them.

Required. Budget about 15 minutes.

## Before anything else — confirm the folder

Everything this training builds lives in one folder the attorney attached to this Cowork task, so their AI employees can find it later.

1. Check whether a folder is attached to this task. If none is, stop and say: "Before we start, attach the folder where you want your Firm Brain files to live (for example, a folder named My Firm Brain). Tell me when it's attached." Don't ask any interview questions until a folder is attached.
2. Confirm out loud before writing anything: "I'll save your files in [folder name]/about-me/. Sound good?" Create `about-me/` if it doesn't exist yet.
3. Save every file this skill creates in that `about-me/` folder — never the folder root, a temporary location, or anywhere else. If the attorney asks for a different location, use it, and tell them plainly that their AI employees look in `about-me/` by default.

## How to run it

One question at a time, same as the Firm Brain interview. Write each answer to `about-me.md` as you go, don't batch it to the end. If someone already has an `about-me.md` from another tool or a prior session, read it first and gap-check the thin spots instead of starting over — same logic as the Firm Brain Prep Sheet path.

**Voice memo option:** offer this up front, same as Firm Brain — "If you'd rather talk through this than type it, record yourself out loud answering these 9 questions — your phone's voice memo app is the easiest way — get a text transcript, and upload or paste it here instead." Treat an uploaded transcript the same way as an existing `about-me.md`: read the whole thing first, map what you can onto the 9 sections below (a spoken transcript won't follow the question order — use judgment on where each part belongs), then ask one at a time about anything thin, missing, or unclear from context. Don't re-ask what's already solid.

Ask, in order:

**1. Who you are**
"Your name, your title (partner, solo practitioner, associate, of counsel), your firm name, and where you're based?"

**2. What you do, dinner-party version**
"If someone at a dinner party asked what you do, what's the one or two sentences you'd actually say — no jargon, no law-firm-brochure polish?"

**3. Current roles and responsibilities**
"Beyond practicing law day to day, what else are you running or responsible for right now — managing the firm, business development, bar or community involvement, teaching or speaking? If something's on the back burner, say so and why."

**4. Who you work with**
"Who are your typical clients, in a sentence? And who else is involved in the firm day to day — associates, paralegals, an office manager, co-counsel you work with regularly, or is it just you?"

**5. Tools**
"What do you open every day for the practice — case management software, email, a specific document system? What do you use weekly or monthly but not daily? Anything you're supposed to use but actually avoid?"

**6. Personal context — optional**
"This one's optional, skip it if you'd rather not: is there anything personal worth knowing — family, what's driving you right now, how you got into this practice area — that would help Claude understand your context, not just your caseload? Totally fine to skip or keep this brief."

Do not push if they skip this. Don't ask a follow-up probing for more. One offer, then move on.

**7. How you learn best**
"When you're figuring out something new — a tool, a process, a way of doing something — what actually works for you? Reading it out, watching someone do it, trying it yourself and breaking it, a quick explanation before you dive in?"

**8. What's worked in past AI sessions**
"Think of a time working with Claude or another AI tool went well. What made it work — 2-3 specific things you want to see repeated?"

**9. Anything else**
"Anything else you want Claude to know about you that didn't fit anywhere above?"

## Output file structure

Save to `about-me/about-me.md`:

```markdown
# About Me — {{NAME}}

## Who I am
- **Name:** {{name}}
- **Title:** {{title}}
- **Firm:** {{firm_name}}
- **Location:** {{location}}

## What I do (plain version)
{{dinner-party description}}

## Current roles & responsibilities
- **Practice:** {{status}}
- **Other responsibilities:** {{list}}
- **On the back burner:** {{if any}} — {{why}}

## Who I work with
- **Typical clients:** {{description}}
- **Team:** {{who, or "just me"}}

## Tools
- **Daily:** {{list}}
- **Weekly/monthly:** {{list}}
- **Avoid, even though "supposed to" use:** {{if any}}

## Personal context (optional)
{{whatever was shared, or "Not shared — that's fine."}}

## How I learn best
{{answer}}

## What's made past AI sessions successful
{{answer}}

## Anything else
{{answer, or "Nothing further."}}
```

## Hard rules for this skill

- Never make personal context mandatory. If skipped, write "Not shared — that's fine." and move on — don't leave a placeholder that reads like an unfinished task.
- Keep this file about the attorney, not the firm's mechanics — if an answer drifts into practice areas, fees, or client process, that belongs in `firm-brain.md`; note it there instead and keep this file lean.
- Don't guess at tone or add color commentary — this file is a factual reference, not a writing sample (that's what writing-rules.md is for).
