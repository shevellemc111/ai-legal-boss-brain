# Intake Matter Types (shared reference for ai-intake-coordinator)

The Intake Coordinator asks **"What type of matter is this?"** before anything else, then runs ONLY the track for that matter type. A criminal caller never gets PI questions, a PI caller never gets criminal questions, and a family caller gets neither.

Each track below is a **starter**. During setup the attorney keeps, cuts, rewords, or adds to the track for each practice area they actually take, and the final version lives in their own `about-me/intake-coordinator.md`. The attorney's rulebook always wins over this file.

Built-in tracks: **Criminal**, **Personal Injury**, **Family**. Any other practice area (estates, immigration, employment, real estate, etc.) uses the **Other / custom track**, built from scratch with the attorney during setup.

---

## Jurisdiction comes first in every track

Attendees practice in different states (this kit is built for **New Jersey, Pennsylvania, Maryland, and Massachusetts**). The tracks below are written state-neutral, with each state's own terms in the table. Rules:

- **Read the attorney's bar admission(s) from Firm Brain.** Use only the terms, courts, and agencies for those states. Never default to New Jersey.
- **Ask which state the matter is in** (common question 2). If the attorney is admitted in more than one state, that answer picks which state's terms apply.
- **Matter is in a state where the attorney isn't admitted** → stop and flag it to the attorney (possible not-a-fit, pro hac vice, or referral). Don't run the track further without the attorney's go-ahead.
- **Deadlines and filing requirements are flags, never advice.** The AI names the issue ("public entity involved: notice deadline may apply") and the attorney calculates and confirms it. No deadline or day count is ever stated to a prospect.
- **Every state-specific term below is a starting point to confirm with the attorney at setup.** It has not been verified against current statutes or rules, and laws change. At setup, show the attorney their state's row and ask them to correct it; their rulebook version wins.

| Topic | New Jersey | Pennsylvania | Maryland | Massachusetts |
|---|---|---|---|---|
| Criminal trial courts | Municipal Court; Superior Court (Law Division, Criminal Part) | Magisterial District Court; Court of Common Pleas | District Court; Circuit Court | District Court / Boston Municipal Court; Superior Court |
| Auto tort option to ask about (PI) | "Limitation on lawsuit" / verbal threshold vs. no limitation | "Limited tort" vs. "full tort" | No tort-threshold election (PIP state) — ask about PIP and coverage | No-fault PIP; ask about medical expenses and injury type (tort threshold may apply) |
| Public-entity claim notice (PI) | NJ Tort Claims Act notice | Notice to government unit (Political Subdivision / Sovereign Immunity Acts) | Local Government Tort Claims Act / Maryland Tort Claims Act notice | Presentment under the Massachusetts Tort Claims Act (G.L. c. 258) |
| Med mal pre-suit/early requirement (PI) | Affidavit of Merit | Certificate of Merit | Certificate of Qualified Expert (Health Care Malpractice Claims) | Medical malpractice tribunal |
| Domestic violence order (Family/Criminal) | TRO / FRO | PFA (Protection From Abuse) | Protective order (interim / temporary / final); peace order | Abuse prevention order (c. 209A) / harassment prevention order (c. 258E) |
| Child-welfare agency (Family) | DCPP | Children & Youth Services (CYS) | Local Department of Social Services | Department of Children and Families (DCF) |
| Family court | Superior Court, Chancery Division, Family Part | Court of Common Pleas (Family Division) | Circuit Court (family division) | Probate and Family Court |
| Contingent fee agreement (PI) | Written agreement; court rule limits (R. 1:21-7) | Written agreement (Rule 1.5(c)) | Written agreement (Rule 19-301.5(c)) | Written agreement (Rule 1.5(c)) |

---

## Common questions (every matter type, asked after the conflict check)

1. Is the caller the prospective client, or calling on behalf of someone? (If on behalf: caller's name and relationship. Intake questions are about the client.)
2. Which state, and which county, is this matter in? (Picks the state terms above; flag if the attorney isn't admitted there.)
3. Full legal name of the client
4. Address, phone (and alternate), email
5. Date of birth
6. How did you hear about us? (referral source)
7. Will someone other than the client be paying? If yes: the financial obligor's full name, phone, and email. Never share case details with a third-party payer unless the client has agreed (Rules 1.8(f) and 1.6 in each state's rules of professional conduct; attorney verifies current rule text).

Sensitive identifiers (SSN, etc.) are collected only if the attorney's rulebook says to, and are never repeated in emails, summaries, Slack, or task tools. Write "SSN on file."

---

## Track: Criminal

**Conflict-check names (collect before any other intake question):** the client; all co-defendants; every complaining witness or alleged victim; any other named party (business, store, property owner).

**Intake questions:**
1. What are the charges? (from the complaint/summons if they have it)
2. Which court (the state's lower court or trial court, per the table), if known
3. Date of arrest or incident
4. Upcoming court dates: date, time, and what the appearance is for
5. Is the client in custody right now? If yes, where?
6. Bail / release conditions, or is a detention hearing scheduled?
7. Any prior record or pending cases? (attorney may cut)
8. Has the client spoken to police or anyone else about the case? (logistics only; no advice)

**Emergency flags (flag immediately, ahead of everything):**
- Client is in custody
- Court date within 1-2 days, or a missed court date / bench warrant
- Detention hearing scheduled
- Any safety concern

---

## Track: Personal Injury

**Conflict-check names (collect before any other intake question):** the client; every at-fault or potentially responsible party (driver, vehicle owner, employer of the driver); any business or property owner; for med mal, every doctor, hospital, or practice involved; all insurance companies on both sides.

**Intake questions:**
1. What type of case: motor vehicle, slip/trip and fall, medical malpractice, dog bite, other?
2. Date and location of the accident or incident
3. What happened, in the client's own words, and who they believe is at fault
4. Injuries, treatment so far, and the doctors, hospitals, or providers
5. Client's own auto/health insurance company. For auto: ask the state's tort-option question from the table (NJ limitation on lawsuit; PA limited vs. full tort; MD and MA: PIP coverage). Client may not know; note "unknown."
6. Other party's insurance; was a commercial vehicle, rideshare, or uninsured/underinsured driver involved?
7. Was a government entity or public property involved (city vehicle, public sidewalk, public school, transit)?
8. Police or incident report number
9. Witnesses, photos, or video
10. Time missed from work / lost wages
11. Has the client already spoken with any insurance company, signed anything, or hired another attorney on this?

**Emergency flags (flag immediately):**
- The statute of limitations may be close or may have passed (attorney calculates; the AI never states a deadline as advice)
- A government entity or public property is involved: public-entity claims carry a short statutory notice deadline in every one of these states (see table; attorney verifies the current requirement)
- Medical malpractice: special early filing requirements apply (see table; attorney verifies)
- Evidence at risk: vehicle about to be repaired or salvaged, surveillance video that may be overwritten
- The client already gave a recorded statement or is being pressured to settle

**Fee note:** PI is usually contingency. Contingent fee agreements must be in writing in all four states, and NJ adds court-rule limits (see table; attorney verifies). The AI fills the attorney's own contingency template only; it never writes fee percentages or terms from scratch.

---

## Track: Family

**Conflict-check names (collect before any other intake question):** the client; the opposing party (spouse, ex-spouse, co-parent, other parent); the opposing party's attorney, if known; all children involved; any other party to the case (grandparents, new partner, DCPP/child-welfare caseworker if named).

**Intake questions:**
1. What type of family matter: divorce, custody / parenting time, child support, alimony, domestic violence protective order (use the state's term from the table: NJ TRO/FRO, PA PFA, MD protective order, MA 209A), post-judgment modification or enforcement, adoption, other?
2. Which court (per the table), if a case is already filed
3. Is there already a case or existing order? (docket number, judgment of divorce, custody or support order)
4. Upcoming court dates: date, time, and what it is for
5. Children: names and ages, and who they live with now
6. Marriage date and separation date (divorce matters)
7. Is the opposing party represented? By whom?
8. Any safety concerns, protective orders, or child-welfare agency involvement?
9. General picture of finances in dispute (home, retirement, business, support) at a high level only (attorney may cut)

**Emergency flags (flag immediately):**
- Any safety concern for the client or a child; active domestic violence
- A threat to take a child out of state or out of the country, or a child withheld
- Hearing or return date within 1-2 days (including a temporary protective order's final-hearing date)
- Child-welfare agency investigation or removal (agency name per the table)

---

## Track: Other / custom

For any practice area not above, the attorney builds the track during setup:
- **Conflict-check names:** who are the adverse parties and related entities in this kind of matter?
- **Intake questions:** what do you always need to know before you'll take this kind of case?
- **Emergency flags:** what makes this kind of matter urgent (deadlines, safety, custody, a hearing)?

---

## Routing rules

- **The matter type decides the track.** Never mix tracks. If a matter honestly spans two (e.g., a domestic violence protective order with criminal charges), follow the attorney's mapping in their rulebook (a criminal defense firm may run protective-order matters through the criminal track; a family firm runs them through the family track). If no mapping exists, ask the attorney which track to use before continuing.
- **Matter type the firm doesn't take** (per Firm Brain Q1 / rulebook): stop, don't run a track, and flag it to the attorney as a not-a-fit inquiry. Never tell the prospect the firm can't help without the attorney's approval.
- **Caller isn't sure what type it is:** ask one plain follow-up ("Is this about criminal charges, an injury, or a family situation like divorce or custody?"). If still unclear, flag it to the attorney.
