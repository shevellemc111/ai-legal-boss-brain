---
name: about-me-builder
description: Required. Builds about-me.md — who this attorney is as a person and a practitioner, separate from how the firm runs. ~15 minutes. Trigger on "about me," "my about-me file," "about me pre-work," or any request to build or fill out an about-me file.
version: 1.1
---

# About-Me Builder

`firm-brain.md` is about the firm — practice areas, clients, fees, process. This file is about the **attorney running it**: how they think, what they're juggling, how they learn, and what's made AI actually useful for them before. Claude reads this alongside `firm-brain.md`, but it's a separate file and a separate section of the interview — don't merge them.

Required. Budget about 15 minutes.

## Before anything else — confirm the folder

Everything this training builds lives in one folder the attorney attached to this Cowork task, so their AI employees can find it later.

1. Check whether a folder is attached to this task. If none is, stop and say: "Before we start, attach the folder where you want your Firm Brain files to live (for example, a folder named My Firm Brain). Tell me when it's attached." Don't ask any interview questions until a folder is attached.
2. Confirm out loud before writing anything: "I'll save your files in [folder name]/about-me/. Sound good?" Create `about-me/` if it doesn't exist yet.
3. Save every file this skill creates in that `about-me/` folder — never the folder root, a temporary location, or anywhere else. If the attorney asks for a different location, use it, and tell them plainly that their AI employees look in `about-me/` by default.

## Before you start — pre-work check

Check whether `about-me/about-me.md` already exists.

- **It exists already** → read it first and gap-check the thin spots instead of starting over.
- **It doesn't exist yet, but the Firm Brain Pre-Work Packet already has About Me answered — typed or a voice-memo transcript** → ask first: "I found your pre-work on About Me. Want me to use it and only ask about what's missing, or would you rather answer these 9 questions fresh?"
  - **Use the pre-work:** read the whole thing first, map what you can onto the 9 sections below (a spoken transcript won't follow the question order — use judgment on where each part belongs), then ask only about anything thin, missing, or unclear. Say up front how much is covered: "From your pre-work, [n] of 9 are answered. Let's cover: [list]."
  - **Answer fresh:** ask all 9, one at a time, and don't pull from the pre-work while doing it.
- **Neither exists** → ask all 9, one at a time.

**Switching mid-stream, either direction:**
- Answering fresh and they say something like "just use my pre-work" — switch right away. Keep whatever they've already answered live (it wins over the pre-work on anything both cover), fill the rest in from the pre-work, and say where that leaves things: "Between what you've answered here and your pre-work, [x] of 9 are done. I just need you on: [list]." Then ask only the remaining gaps.
- Gap-checking the pre-work and they'd rather answer the rest fresh — switch back just as readily, and stop pulling from the pre-work for anything not yet asked.

## How to run it

One question at a time, same as the Firm Brain interview. Write each answer to `about-me.md` as you go, don't batch it to the end.

**Voice memo option:** offer this up front, same as Firm Brain — "If you'd rather talk through this than type it, record yourself out loud answering these 9 questions — your phone's voice memo app is the easiest way — get a text transcript, and upload or paste it here instead." Treat an uploaded transcript the same as a Pre-Work Packet for the choice above.

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
