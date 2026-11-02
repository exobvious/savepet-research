# PetMergency Activated Charcoal First Aid Kit (SavePet): onboarding step four, the Category Context Template

- **Run:** onboarding / 04-category-context, 2026-11-02 (UTC), cloud research agent
- **Product folder:** `01_petmergency_activated_charcoal_first_aid/` in `exobvious/savepet-research`
- **Target file:** `01_petmergency_activated_charcoal_first_aid/EB_CATEGORY_CONTEXT_<category>_v2.md`
- **Status: BLOCKED. The template prompt was not run.**
  - `EB_CATEGORY_CONTEXT_<category>_v2.md` was **not created**.
  - Nothing was synthesised: no Category Overview and no Potential Angles and Hooks.
  - Apify spend: **$0.00**. Nothing was bought.
  - This report is the only file written.
- **Two reasons, and either one alone stops the stage:**
  1. **The prompt isn't registered.** The playbook's "Category context template" row still says `ADD_ID`, and its Container column is empty. The playbook says: "A stage whose prompt column still says `ADD_ID` is reported as missing; the bot never reconstructs a prompt from memory or substitutes a similar one." AGENTS.md rule 2 says the same.
  2. **The raw research isn't complete, so it can't be run "on the complete research".** The playbook's research order (step 3) says: "Only when the raw research is in, run the category context template prompt once." The lesson says: "Once raw research is complete, leave the other sections blank … upload it to Claude with the provided prompt." What is actually in place:
     - **Reddit**, the course's primary source, has **0 of 156** bank questions run.
     - **Quora answers** are MISSING.
     - **P3 and P5 are thin.**

     Because the playbook allows only one run of this stage ("run … once"), using that run on partial research would spend it on the wrong input.

---

## 1. What was read (in order)

| # | Source | Result |
|---|---|---|
| 1 | `gateway_status` | scaler, vantage, apify and supermemory OK. **clickup: false** (not configured; no tasks are created by policy). GitHub OK. Apify spend today before this run: $2.23, no daily stop. |
| 2 | `get_playbook` → `00_rules_and_process/UNIFIED_PLAYBOOK.md` (sha 02e8ca8) | Registry row "Category context \| Category context template" = **`ADD_ID`**, Container empty. Every other row is also `ADD_ID`. **The playbook names no Supermemory space** for course prompts or for evidence. |
| 3 | `PRODUCT_DECISION.md` (sha 3f08d1e) | Core category (verbatim): "Pet first aid / at-home pet poisoning response (activated charcoal)". Six buyer problems P1–P6. Competitors: "none given yet". Locked rules: page claims, "Made in USA" and "third-party tested" are seller claims. The avatar-profile quotes are illustrative and its numbers are hypotheses. Keep SavePet separate from Vylaras. |
| 4 | `product_truth.md` (sha a2a4a93) | 1 tube at $39.95. Coconut shell activated charcoal plus kaolin clay (named on the page). The full label, mL per tube, supplier, origin and bundle prices are NOT CONFIRMED. The page's dose guidance contradicts itself. |
| 5 | Step 1 report `01-raw-research-reddit-answers-bank.md` (sha ec5bca1) | BLOCKED. 0 of 156 Reddit Answers questions run, $0. No raw files, no avatar templates, no category document. |
| 6 | Step 2 report `02-raw-research-thin-families-on-the-other-channels.md` (sha 78576b8) | PARTIAL. Amazon, YouTube and TikTok were kept, about 75 customer quotes. Facebook was bought but not read. Quora had no answers. The quote bank lives in that report's §4. **P3 and P5 thin.** |
| 7 | Step 3 report `03-avatar-clean-up.md` (sha 9e931f7) | BLOCKED as a stage. That run read the 30 paid Facebook posts (25 distinct owners). Their quotes are in its §4. P3 and P5 are still thin. |
| 8 | `RAW_RESEARCH_METHOD.md` (sha f11ed6d) | One category document per product, `EB_CATEGORY_CONTEXT_<category>_v2.md`, "written by the category context step". New material is appended as dated `## Added` sections. |
| 9 | `00_rules_and_process/telegram_log/2026-11-02.md` (sha a79096f) | At 17:24 the owner approved: "yes reword it for my offer then run the search". The rewording, Reddit and profile-copy steps were **never queued** because the queue was busy. They should run once the queue is free (the owner is to send "queue reddit"). **No message registers a category context prompt.** The owner hasn't said to run this stage on partial research. |
| 10 | Product folder listing (savepet repo) | 11 files. **No `EB_CATEGORY_CONTEXT_*`.** Nothing in `raw/` or `avatar/` except READMEs. `00_rules_and_process/` in the savepet repo is empty, so the main-repo playbook governs. |
| 11 | Supermemory `list_spaces` | Only `research_bot` (48 docs, 113 memories). No `courses` space. |
| 12 | Supermemory `search_memory` "category context template prompt" (default namespace) | 0 results. |
| 13 | Supermemory `search_memory` "SavePet category context template registered prompt ID" (`research_bot`) | 10 hits, all status notes. The top hit is `1GJFECMHBdk2aVq4TT6EEi`, "Category context template was blocked because no registered prompt and research unfinished." (doc `6JvLuSrzs3q9FfjHYsAGNw`), most likely the Vylaras run. **No prompt document.** |
| 14 | Scaler `search_docs` (3 queries on the template) → `get_doc(51)` "Learn E-Commerce Builders (3): Raw Research and Category Context for Copywriting" (skool_url null) | **I read the lesson in full** (§2). The template prompt text is printed inside the lesson. It is not registered, so I did not run it. |
| 15 | `list_apify_runs` (10 h) | Still **no Reddit run**. SavePet `raw-research`: 13 runs, $0.70. **Untagged: 26 runs, $1.08**, almost all from Facebook Ads Library actor `XtaWFhbtfxyzqrFmd`, the newest at 18:28 UTC. Nothing to reuse for this stage. |

## 2. What the lesson says this stage is (Scaler doc 51), for the owner

I read the lesson as the playbook requires. I quote it here so the owner can decide on registration. **I did not run any of it.**

- **When to run it:** "Once raw research is complete, leave the other sections blank, download the doc as a PDF, and upload it to Claude with the provided prompt." Also: "By the end of this stage, the category context file should be stacked."
- **The lesson's steps:**
  1. Remove the blue text.
  2. Download the PDF.
  3. Upload it to Claude.
  4. Use the template prompt.
  5. Paste Claude's sections back in.
- **Template sections:**
  - Category Overview: Category Name, Core Problem / Symptom, Emotional Core, Audience Snapshot
  - Raw Research
  - Potential Angles and Hooks
- **The prompt's rules (quoted from the lesson):**
  - "Base everything ONLY on the themes and patterns inside my Avatar Deep Dive research."
  - "Do NOT invent hooks."
  - "Do NOT introduce new symptoms, claims, or solutions."
  - "Do NOT use information from outside the uploaded file."
- **The prompt has a fill-in:** "Keep everything specific to this angle (INSERT ANGLE HERE)."

**Why I didn't treat the lesson text as the registered prompt.** The playbook makes the owner the one who points a stage at its prompt, either with a Supermemory ID or by writing `scaler: <lesson>` in the registry. The row is still `ADD_ID`. On top of that, the printed prompt doesn't match this stage on three points, and each needs an owner decision, not a bot guess:
1. It is written for an "**EB Angle Context Template**" with an "**Avatar Deep Dive**" section. This stage is the **Category** Context Template, and its research section is called "Raw Research".
2. It says to keep everything "specific to this angle (INSERT ANGLE HERE)". This stage runs on the **broad core category**, before any angle is chosen. Whatever goes in that blank changes the output.
3. The lesson's section is called "Potential Angles and Hooks". The prompt's task is called "Potential Hooks & Leads".

Filling those gaps myself would mean rewriting the prompt, which is the reconstruction the playbook forbids.

## 3. Readiness check against "run once on the complete research"

| Requirement | State today | Source |
|---|---|---|
| Reddit Answers: every bank question per problem, threads and comments followed, subreddits searched | **0 of 156 run.** Rewording approved at 17:24 but not queued. | Reports 01, 02, 03; Telegram 17:24–17:25; `list_apify_runs` |
| Amazon reviews | Done, 2 pages (helpful and critical), 25 kept | Report 02 §4, §6 |
| YouTube comments | Done, 4 videos, 26 kept (transcripts **not** pulled; the lesson asks for both) | Report 02 |
| TikTok comments | Done, 5 videos, 24 kept | Report 02 |
| Facebook groups | 30 posts read, 25 distinct owners. Comments on the big threads (595, 257, 167, 99) **not bought** | Report 03 §4 |
| Quora | **Answers MISSING.** 1 story, 2 titles. | Report 02 §3 |
| Competitor ad comments (AdSpy in the lesson) | **Not done.** AdSpy isn't one of the gateway's tools. Vetanica's Facebook ad is known only through one owner's post. | Report 03 §4.6 |
| Category document exists to run the prompt on | **No.** Quotes are spread over report 02 §4 and report 03 §4. | Folder listing |
| Per-problem coverage | P1, P2, P4, P6 covered (3+ people). **P3 thin** (4 indirect, and nobody says "the vet was closed"). **P5 thin** (1 report, $65). | Report 03 §6 |

**Verdict:** not complete. The course's main source hasn't run at all, and two of the six buyer problems are thin.

There is also a specific risk if the prompt ran now. It reads only the uploaded file. With no Reddit voice, the Emotional Core and Audience Snapshot would come almost entirely from Amazon reviewers who already bought charcoal and from TikTok commenters on affiliate videos. Those audiences lean toward buyers and toward vet-staff objections. The "vet closed at night" and "poison control fee and hold" problems, two of the owner's six, would barely show up, and the output would not reflect the full category.

## 4. Things the eventual run will need to handle (from the existing evidence, not synthesis)

These come from reports 02 and 03, with sources there. They are not template output, and I only list them so the eventual run doesn't lose them.

- **Negative evidence must sit in Raw Research next to the seller's claims.** Examples:
  - "as a vet assistant never give this without consulting a vet first! charcoal can cause dangerous electrolyte imbalances!" (TikTok, 2,533 likes)
  - "NOT SAFE FOR CATS" (575 likes), which contradicts the seller's cat claim
  - "My vet said please don't use that she could aspirate the charcoal…" (Amazon RXIWHMIQJDOQL)
  - "my vet didn't like the fact that I bought it" (Facebook, Dupont)

  The prompt's "Do NOT introduce new … claims" rule doesn't stop it from leaving out negative lines. Whoever runs it should check that these survive into the Emotional Core and the hooks section.
- **The profile's numbers are not research.** The avatar profile's $95 hotline fee, $2,000 bill, 451,000 calls, 38%, 81% and 82% must **not** be put in the category document as raw research. Only the real figures are raw research: $65 poison control, $600 visit, $1,000 deposit, one "2 grand". The profile is a written summary (locked in `PRODUCT_DECISION.md`).
- **Seller and affiliate content (`competitor_claim`) stays labelled,** so the prompt doesn't read it as customer voice. Examples: "EpiPen"-style lines from affiliates, "#1 Vet Recommended", and the Kelly Bone affiliate post.
- **Customer quotes are about other brands.** No quote mentions SavePet or PetMergency. Every product-specific line is about PawMergency, PetVet Medic, NOW, a powder, or Vetanica.
- **Possible filename slug** (suggestion, owner's call): `EB_CATEGORY_CONTEXT_pet_poisoning_first_aid_v2.md`. It is taken from the core category in `PRODUCT_DECISION.md`.

## 5. Contradictions and open questions

1. **Stage queued ahead of its inputs.** This is the second time in a row: the clean-up (step 3) was queued before the avatar stage existed, and now the category context (step 4) is queued before Reddit has run. The Telegram queue (16:38) put "Background on pet first aid and poisoning" fourth, which looks like this stage. The playbook puts it after raw research is in.
2. **Names don't agree.** The playbook has "Category context template". The lesson body has "EB CATEGORY CONTEXT TEMPLATE". The lesson's prompt has "EB Angle Context Template" with "Avatar Deep Dive". `RAW_RESEARCH_METHOD.md` has `EB_CATEGORY_CONTEXT_<category>_v2.md`. Step 1 asked for `EB_ANGLE_CONTEXT_TEMPLATE.md`, which still exists in neither repo.
3. **Who runs it.** The lesson has the human upload a PDF to Claude and paste the output back. The playbook gives the run to the bot. Either works once a registered prompt and a finished document exist, but the owner should say which.
4. **"Run once" vs "evergreen".** The playbook says to run the template once. The lesson says the file is "continuously updated" and you "refresh the context" later. My reading: the synthesis runs once, and Raw Research keeps growing through `## Added` sections. That needs confirming.
5. **Untagged Apify spend keeps growing.** It is now 26 runs and $1.08 in 10 h, mostly Facebook Ads Library pulls with nothing tagged to them. Reports 01–03 already flagged this, and the runs are still happening.
6. **Stale memory.** Supermemory `rt13wF2CCVkUvpbA7krzhy` still says SavePet research goes to the main repo. That is wrong: the owner chose `exobvious/savepet-research`. I didn't edit memories.

## 6. Ideas for the owner (not tasks; nothing was assigned or scheduled)

1. **Register the stage's prompt.** Two options:
   - Write `scaler: Learn E-Commerce Builders (3): Raw Research and Category Context for Copywriting — CLAUDE PROMPT FROM THE TEMPLATE` in the Category context row.
   - Or upload your own copy, adjusted for a *category* rather than an angle, as a Supermemory document and paste its ID.

   Either way, settle three things: what goes in "(INSERT ANGLE HERE)" for a category run, whether "Avatar Deep Dive" means "Raw Research" here, and "Angles and Hooks" vs "Hooks & Leads".
2. **Finish the raw research first, in course order.** Send "queue reddit" so the approved rewording runs, then the Reddit run (cap $6), then the profile copy. Point Reddit hardest at P3 ("vet closed", "no emergency vet near me") and P5 ("poison control fee", "ASPCA poison control charge", "pet poison helpline hold").
3. **Then build the category document from the existing quote banks.** Paste report 02 §4 and report 03 §4 (both verbatim, sourced) into `EB_CATEGORY_CONTEXT_<slug>_v2.md` as dated `## Added 2026-11-02` sections, plus the Reddit output. Leave Category Overview and Angles/Hooks blank, as the lesson says. **Only then** queue this stage, once.
4. **Optional gaps before the run:**
   - YouTube transcripts for the 4 chosen videos, which the lesson asks for alongside comments
   - comments on the four big Facebook threads
   - a Quora answer source that works

   None of these is priced yet. AdSpy-style competitor ad comments aren't reachable through the gateway. Vantage gives ad structure only, never customer proof.
5. **Proposed `NEVER_REPEAT_MISTAKES.md` line** (queue order has now gone wrong twice):
   > "Don't queue a synthesis stage (category context, clean-up, deep research) until the stage it reads from has written its files and the stage's registry row has an ID."
6. **Add PawMergency, PetVet Medic, Vetanica and NOW to Competitors** in `PRODUCT_DECISION.md` if you agree (reports 02 and 03).

## 7. Unavailable or failed sources

- **Category context template prompt:** MISSING from the registry (`ADD_ID`). No Supermemory prompt document. The lesson text exists in Scaler doc 51 but is unregistered (§2).
- **Supermemory course space:** none. The playbook names no space. The only space is `research_bot`, which holds chat logs and step notices.
- **Reddit:** not run (0 of 156).
- **Quora answers:** MISSING.
- **AdSpy:** not available through the gateway.
- **ClickUp:** not configured and not used. No tasks were created.
- **Vantage:** not used. It gives ad structure only and is never category evidence.
- **Tool failures this run:** none. Every call answered. The stage stopped on missing inputs.

## 8. Outputs of this run

- `01_petmergency_activated_charcoal_first_aid/EB_CATEGORY_CONTEXT_<category>_v2.md`: **not created.** There is no registered prompt and the raw research is incomplete. A file with a Claude-style Category Overview written without the registered prompt would be a reconstruction, and a file with blank sections would wrongly look like the stage had run.
- `course_v2/COVERAGE_V2.md`: unchanged. The category context block stays unticked.
- Apify: **$0.00**. Only free reads were used (Scaler `search_docs` and `get_doc`, Supermemory `list_spaces` and `search_memory` ×2, `list_apify_runs`, GitHub reads).
- This report is the only file written.
