---
name: how-i-work-builder
description: Optional. Builds how-i-work.md — standing rules for how Claude should operate day to day with this attorney, separate from what the firm does. Use anytime after firm-brain.md and about-me.md exist. Trigger on "how I work," "how i work file," "set up how Claude works with me," or any request to define working preferences or standing rules.
version: 1.1
---

# How I Work Builder

This is **optional** — unlike Firm Brain, Writing Rules, and About Me. It's worth doing if an attorney wants more control over Claude's default behavior, but nobody should feel behind for skipping it. If time is tight during the morning block, this is the one to skip first.

Budget about 10 minutes if they choose to do it.

## Before anything else — confirm the folder

Everything this training builds lives in one folder the attorney attached to this Cowork task, so their AI employees can find it later.

1. Check whether a folder is attached to this task. If none is, stop and say: "Before we start, attach the folder where you want your Firm Brain files to live (for example, a folder named My Firm Brain). Tell me when it's attached." Don't ask any interview questions until a folder is attached.
2. Confirm out loud before writing anything: "I'll save your files in [folder name]/about-me/. Sound good?" Create `about-me/` if it doesn't exist yet.
3. Save every file this skill creates in that `about-me/` folder — never the folder root, a temporary location, or anywhere else. If the attorney asks for a different location, use it, and tell them plainly that their AI employees look in `about-me/` by default.

## Before you start — pre-work check

Check whether `about-me/how-i-work.md` already exists.

- **It exists already** → tell them what you found and ask if they want to redo it or leave it alone.
- **It doesn't exist yet, but the Firm Brain Pre-Work Packet already has How I Work answered** → ask first: "I found your pre-work on How I Work. Want me to use it and only ask about what's missing, or would you rather answer these 5 questions fresh?"
  - **Use the pre-work:** map every answer onto the template, then ask only about the gaps. Say up front how much is covered: "From your pre-work, [n] of 5 are answered. Let's cover: [list]."
  - **Answer fresh:** ask all 5, one at a time, and don't pull from the pre-work while doing it.
- **Neither exists** → ask all 5, one at a time, per below.

**Switching mid-stream, either direction:** same as the other modules — "just use my pre-work" switches right away (live answers win over the pre-work, then it fills the rest and says "[x] of 5 are done, I just need you on: [list]"); wanting to finish fresh instead switches back, and the pre-work stops getting pulled from that point on.

## How to run it

One question at a time, write to file as you go.

**1. Response length**
"When you ask me something, do you usually want the short answer, or the fuller explanation with reasoning? Does that change depending on what you're asking about?"

**2. Ask-first vs. proceed**
"For routine tasks — drafting something, organizing files, pulling together info — should I just do it and show you the result, or check in with you first before starting? Does that answer change for anything higher-stakes, like something going to a client or opposing counsel?"

**3. Options vs. single pick**
"When there's more than one reasonable way to do something, do you want me to just make a call and tell you what I picked, or lay out the options and let you choose?"

**4. Default file format**
"When I create something for you, what's the default format you want — a doc, a plain message in chat, something else? Does it depend on what the deliverable is?"

**5. Delegation format (skip if solo)**
"If you have a team, how do you want me to hand off work to them — a written brief, a task in whatever tool you use, something else? If it's just you, skip this one."

**6. Accuracy check — fixed, not asked**
Tell them directly, don't ask this as an open question: "Two standing rules that are always on, no matter what you answer above, and they don't get customized away: I never cite a case, statute, rule, or other legal authority without confirming it actually exists and says what I'm claiming it says — no guessing from a familiar-sounding name. And I always flag anything that looks like a likely legal or factual error before finishing — a wrong-looking date, a citation I can't verify, a claim that doesn't hold up — rather than let it slide through."

## Output file structure

Save to `about-me/how-i-work.md`:

```markdown
# How I Work With Claude — {{NAME}}

## Response length
{{answer}}

## Ask-first vs. proceed
{{answer, noting any distinction between routine and higher-stakes tasks}}

## Options vs. single pick
{{answer}}

## Default file format
{{answer}}

## Delegation format
{{answer, or "Solo — not applicable."}}

## Non-negotiable regardless of other settings
- Claude never cites a case, statute, rule, or other legal authority without confirming it actually exists and says what's being claimed — no guessing from a familiar-sounding name.
- Claude always flags likely legal or factual errors before finishing a task — a wrong-looking date, an unverifiable citation, a claim that doesn't reconcile — rather than letting it pass silently.
```

## Hard rules for this skill

- The two non-negotiable rules in the output template are fixed — they go in unedited, every time, regardless of what else is customized.
- Don't pad this file with sections nobody answered. If "delegation format" was skipped because they're solo, say so plainly rather than leaving a blank header.

## Version notes

v1.0 — `about-me/` file location and pause/resume conventions, matching the pattern used across this kit. The two non-negotiable rules (no uncited authority, always flag likely errors) are fixed and don't get customized away.

v1.1 — Added the pre-work choice-and-switch behavior: if the Firm Brain Pre-Work Packet already has How I Work answered, ask whether to use it and only fill gaps, or answer fresh, and support switching either direction mid-session.
