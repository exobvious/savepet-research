# PetMergency Activated Charcoal First Aid Kit (SavePet): EB raw research step one, Reddit Answers problem bank

- **Run:** onboarding / 01-raw-research-reddit-answers-bank, 2026-11-02 (UTC), cloud research agent
- **Product folder:** `01_petmergency_activated_charcoal_first_aid/` in `exobvious/savepet-research`
- **Status: BLOCKED (partly unblocked since the Vylaras run).** No Reddit Answers questions were run. Nothing was bought on Apify ($0.00). No verbatim raw files were written to `raw/avatar_bank_2026-11-02/`, and no avatar templates were written to `avatar/`. This report is the only file this run wrote.
- **What changed since the 2026-10-20 Vylaras run:** the buyer's problems now exist. `PRODUCT_DECISION.md` lists six of them, so `[problem]` is no longer empty.
- **What still blocks the stage:**
  1. The prompt registry still says `ADD_ID` for both raw-research rows.
  2. `EB_ANGLE_CONTEXT_TEMPLATE.md` does not exist in either repo.
  3. The course bank has 26 questions, not 27.
  4. The course's own tailoring step has to rewrite the bank for this category before anything runs, and nobody has signed off that wording.

  The playbook says: "A stage whose prompt column still says `ADD_ID` is reported as missing; the bot never reconstructs a prompt from memory or substitutes a similar one." AGENTS.md rule 2 says the same. I followed that rule.

---

## 1. What was read (in order)

| # | Source | Result |
|---|---|---|
| 1 | `gateway_status` | scaler, vantage, apify and supermemory were OK. **clickup: false** (not configured, and not needed because this run creates no tasks). GitHub OK. Apify today: $1.49 spent, no daily stop. |
| 2 | `get_playbook` → `00_rules_and_process/UNIFIED_PLAYBOOK.md` (sha 02e8ca8) | **Every registry row still says `ADD_ID`**, including "Raw research lesson" and "Problem question bank". The Container column is empty. |
| 3 | `PRODUCT_DECISION.md` (sha 3f08d1e) | Core category: "Pet first aid / at-home pet poisoning response (activated charcoal)". **Six buyer problems** (listed in §3). Competitors: "none given yet". Locked rules: page claims and "Made in USA" / "third-party tested" are seller claims. The avatar-profile quotes are illustrative, and its numbers are hypotheses. The brand spelling is unconfirmed. Keep SavePet separate from Vylaras. |
| 4 | `product_truth.md` (sha a2a4a93) | 1 tube at $39.95 (shown as down from $80). Named on the page: coconut shell activated charcoal and kaolin clay. Full ingredient list, mL per tube, supplier, origin and bundle prices are **NOT CONFIRMED**. The page's dose guidance contradicts itself. |
| 5 | `get_playbook raw-research` → `RAW_RESEARCH_METHOD.md` (sha f11ed6d) | Steps: write the coverage table first, then run every bank question for an uncovered problem, follow the cited threads, and use other channels only for thin families. Per-problem files go in `<folder>/avatar/`. |
| 6 | `NEVER_REPEAT_MISTAKES.md`, `AGENTS.md` | Never-repeat is empty. AGENTS rule 2: "A stage with no ID yet is reported as missing, not improvised." |
| 7 | `00_rules_and_process/telegram_log/2026-11-02.md` | The owner chose a separate repo (B) and then said "go + research". At 16:38 the assistant said Reddit collection was "running now". **Related findings:** no Reddit Answers Apify run exists (§5), and no raw files are in the SavePet folder. |
| 8 | Repo searches for `EB_ANGLE_CONTEXT_TEMPLATE` (main repo and savepet repo) and "Reddit Answers Question Bank" (main) | **0 hits** each time. |
| 9 | `list_project_files` on the SavePet product folder | Only `PRODUCT_DECISION.md`, `product_truth.md`, READMEs, `course_v2/COVERAGE_V2.md` and `listening/SOURCES.md`. `avatar/README.md` expects `<problem>_EB_TEMPLATE.md` files, and none exist. `raw/README.md` says "Raw pulls, saved verbatim with links. Never edited." **There is no category context document yet.** |
| 10 | Main repo root listing | `SavePet PetMergency Avatar Profile.pdf` and `.txt` are still loose at the main repo root. They have not been copied into the SavePet repo, as the Telegram log said. I did not read the profile again, because the decision file already carries its six problems and its locked caveats. |
| 11 | Supermemory `list_spaces` → `research_bot` (37 docs, 51 memories), then `search_memory` | **No course prompt or question bank is stored there.** One hit: doc `SuShCWyV62J9nNnEceT4jR` (the Vylaras 2026-10-20 run), which records "Course lesson's question bank contains 26 questions, not 27" and "Named avatar template file for the step does not exist." Memory `rt13wF2CCVkUvpbA7krzhy` says the "research for SavePet should use the main repo exobvious/research". That is **stale**: the owner later chose a separate repo (Telegram 16:15–16:38). |
| 12 | Main repo `01_ai_translator_earbuds/bot_reports/onboarding/2026-10-20/01-raw-research-reddit-answers-bank.md` | The same stage was blocked for Vylaras, and that report gives Apify actor options for a Reddit Answers lane. |
| 13 | Scaler `get_doc(51)`: "Learn E-Commerce Builders (3): Raw Research and Category Context for Copywriting" (skool_url null) | I read it in full again. It still holds the **26-question** bank and the tailoring prompt. Details in §4. |
| 14 | `list_apify_runs` (last 6 h) | 23 runs. All are untagged, all used actor `XtaWFhbtfxyzqrFmd` (identified on 2026-10-20 as `curious_coder/facebook-ads-library-scraper`), and all SUCCEEDED. Reported totals: $0.96 (`total_usd`) vs $1.03 (`by_job.untagged`). **No Reddit Answers run, nothing tagged to SavePet, nothing to reuse.** I did not open these datasets because they are not Reddit data. |

## 2. Blockers

1. **The prompt registry is not filled.** "Raw research lesson" and "Problem question bank" both say `ADD_ID`. The lesson does exist (Scaler doc 51), and the playbook lets the owner write `scaler: <lesson name>` in the registry. Nobody has done that, so I report the stage as missing rather than picking the prompt myself.
2. **`EB_ANGLE_CONTEXT_TEMPLATE.md` does not exist** in `exobvious/research` or `exobvious/savepet-research`. The per-problem avatar template (`avatar/<problem>_EB_TEMPLATE.md`) has no file to copy from. Scaler doc 51 gives only the template's section names, not its full text.
3. **There are 26 questions, not 27.** "Run every question, skip none" can't be checked until the owner settles which bank is the real one.
4. **The bank can't run unedited on these six problems.** The course says to tailor the templated questions to the category with a short Claude prompt *before* running them. These problems are written in the first person, and one of them is itself a question, so straight substitution produces broken questions:
   - *"What have people tried to fix Should I make him throw up with peroxide? that didn't work?"*
   - *"What's something people don't understand about having The vet is closed at night?"*

   The tailored wording becomes the actual prompt. If I wrote it myself, that would be the reconstruction the playbook forbids, so it needs the owner's sign-off (or her uploaded tailored copy).

None of these was a tool failure. Every source answered. The stage stopped because inputs were missing.

## 3. The six problems (from `PRODUCT_DECISION.md`, verbatim) and their status

| # | Problem (verbatim) | Bank questions run | Raw file | Avatar template |
|---|---|---|---|---|
| P1 | My dog ate something toxic and I have nothing at home to help | 0 / 26 | not created | not created |
| P2 | Should I make him throw up with peroxide? | 0 / 26 | not created | not created |
| P3 | The vet is closed at night | 0 / 26 | not created | not created |
| P4 | A $2,000 emergency vet bill | 0 / 26 | not created | not created |
| P5 | Poison control charges a fee and puts me on hold | 0 / 26 | not created | not created |
| P6 | I'm scared I'd give the wrong amount in a panic | 0 / 26 | not created | not created |

A full run would be **6 × 26 = 156 Reddit Answers questions**, or 162 if the bank really has 27.

Note: these problems came from the owner's avatar profile, which the decision file itself calls "a written summary" with illustrative quotes. They are good **search inputs**. They are not yet **evidence**. Each needs two independent customer reports before it enters the angle bank (AGENTS.md rule 4).

## 4. What the course lesson says (Scaler doc 51), for the owner to register

I report this so the owner can decide. **I did not run it.**

- **How the bank is used:** go to reddit.com/answers, "Run all of the questions through Reddit Answers. Do not skip any." Then click into the linked posts, read the comments, search the relevant subreddits directly, and paste the exact quotes under RAW RESEARCH.
- **Tailoring step (part of the course):** "adjust these questions so it is relevant to our category". The lesson shows a Claude prompt written for the hair-removal example. For SavePet it would need the owner's pet-poisoning version.
- **Bank: 26 questions in 7 families:**

  | Family | Count |
  |---|---|
  | Emotional Experience | 4 |
  | Failed Attempts & Frustration | 5 |
  | Beliefs & Self-Image | 5 |
  | Transformation & Hope | 4 |
  | Language, Voice & Expression | 3 |
  | Trust & Proof | 3 |
  | Catalyst Moments (Buying Psychology) | 2 |
  | **Total** | **26** |

- **Bank wording written for skincare that the tailoring step would have to adapt** (I flagged these and did not rewrite them):
  - "What ingredients or methods made [problem] worse?"
  - "Who do they trust most -- peers, dermatologists, influencers, or brands?" For this category the obvious stand-ins are vets and poison hotlines, but that is the owner's call.
  - "How has [problem] changed how people see themselves or their confidence?"
  - "What words do they use to describe themselves because of [problem]?"
  - The "fix [problem]" phrasing in general. An emergency is a one-off event, not a chronic condition.
- **Template sections (per the lesson):** Category Overview (Category Name, Core Problem / Symptom, Emotional Core, Audience Snapshot), Raw Research, Potential Angles and Hooks. The lesson duplicates one template **per core category**. Its closing Claude prompt calls the file the "EB Angle Context Template", with an "Avatar Deep Dive" section.

## 5. Coverage table (RAW_RESEARCH_METHOD step 1: read first)

No category context document exists, and no per-problem files exist. The table is the same for all six problems (P1–P6):

| Family | Status | Quotes (different people) |
|---|---|---|
| Emotional experience | thin | 0 |
| Failed attempts and frustration | thin | 0 |
| Beliefs and self-image | thin | 0 |
| Transformation and hope | thin | 0 |
| Language, voice and expression | thin | 0 |
| Trust and proof | thin | 0 |
| Catalyst moments / buying psychology | thin | 0 |

**End-of-run table: unchanged.** No searches were run. No family may be marked "MISSING after saturation", because none has been searched yet.

## 6. Pull log

| Actor | runId | datasetId | Bought | Kept | Cost |
|---|---|---|---|---|---|
| none | none | none | 0 | 0 | **$0.00** |

The only calls were free reads: Scaler `get_doc(51)`, Supermemory `list_spaces`, `search_memory` and `get_document`, and `list_apify_runs`.

**Reddit Answers lane for the next run.** These Apify Store listings were recorded by the 2026-10-20 report. I did not re-check them today, and none has been tested:

| Actor | Why | Listed price (2026-10-20) |
|---|---|---|
| `nice_dev/reddit-answers-scraper` | Batches many questions and returns the cited posts and top comments. That matches "follow the threads behind each answer". New, with 3 users. | $0.00699/answer + $0.00799 source text + $0.00149 comments per post |
| `openclawai/reddit-scraper` | AI answers plus post and comment fetches in one actor. 233 users. | $0.01/answer, $0.002/post or comment |
| `clearpath/reddit-answers-api` | One question per run. 58 users. | $0.035/answer |
| `lexis-solutions/reddit-answers-scraper` | `questions[]` batch. 40 users. | $0.025/result + $0.005 start |

Rough cost, a hypothesis built from those listings: about $0.40 per problem on `nice_dev` with source text, so about **$2.40 for all six problems**, before following comment threads. It is about $5.50 on `clearpath`. Reddit Answers output is only a starting point: the quotes kept must come from the cited threads and comments, with permalinks saved.

## 7. Unavailable or failed sources

- **ClickUp:** not configured (`clickup: false`). No tasks are created by policy.
- **Course prompts in Supermemory:** none stored. The space `research_bot` holds chat logs and run summaries only.
- **`EB_ANGLE_CONTEXT_TEMPLATE.md`:** absent from both repos.
- **Vantage:** not used on purpose. It covers ad structure only, never customer problems. On 2026-11-02 the Telegram assistant also reported that Vantage had nothing on SavePet or pet first aid.
- No source call failed.

## 8. Contradictions found

1. **27 vs 26:** the stage instruction says 27 questions, but Scaler doc 51 has 26. The 2026-10-20 run found the same thing, and it is still unresolved.
2. **One file, four names:** `EB_ANGLE_CONTEXT_TEMPLATE.md` (the stage), "EB CATEGORY CONTEXT TEMPLATE" (the lesson body), "EB Angle Context Template" (the lesson's Claude prompt) and `EB_CATEGORY_CONTEXT_<category>_v2.md` (`RAW_RESEARCH_METHOD.md`).
3. **Per problem vs per category:** the stage wants an avatar template per problem in `avatar/`. The lesson makes one template per core category. `RAW_RESEARCH_METHOD.md` does both: one category document plus per-problem files.
4. **"Running now" vs nothing run:** at 16:38 Telegram told the owner that Reddit collection was "running now". In the last 6 hours there is no Reddit Answers Apify run and no file under `raw/`. The only runs are untagged Facebook Ad Library pulls. The owner may believe Reddit research is underway when it is not.
5. **Stale memory:** Supermemory memory `rt13wF2CCVkUvpbA7krzhy` ("research for SavePet should use the main repo exobvious/research") conflicts with the owner's later choice of `exobvious/savepet-research`. It should be forgotten or corrected so that future runs don't write to the wrong repo.
6. **Problems written as statements, bank written for chronic conditions:** see blocker 4 and §4.
7. **Apify cost totals disagree:** `list_apify_runs` reports `total_usd` $0.96 but `by_job.untagged` $1.03 for the same 6-hour window.

## 9. Ideas for the owner (not tasks; nothing was assigned or scheduled)

- **Register the two raw-research prompts in the playbook.** Either:
  - "Raw research lesson" → `scaler: Learn E-Commerce Builders (3): Raw Research and Category Context for Copywriting` (doc_id 51), and
  - "Problem question bank" → that lesson's "Reddit Answers Question Bank" section, or a Supermemory document ID for your own copy (for example a 27-question version).
- **Settle 26 vs 27.** If your copy has a 27th question, upload it to Supermemory and register its ID.
- **Supply or approve the tailored, pet-poisoning version of the bank** (the course's Claude tailoring step). Decide in particular:
  - who replaces "dermatologists" (vets? poison hotlines?), and
  - how the "fix [problem]" questions read for a one-off emergency.

  Upload the result as a Supermemory document and register its ID. Then the next run can do all 156 questions word for word with no improvising.
- **Pick one template filename and commit the template file** (its full text isn't in the lesson). Decide whether avatar files are per problem (`avatar/<slug>_EB_TEMPLATE.md`) as this stage says, per category as the lesson says, or both as the repo method says.
  - Possible slugs, a suggestion only: `toxic_ingestion_nothing_at_home`, `peroxide_vomit_question`, `vet_closed_at_night`, `emergency_vet_bill`, `poison_control_fee_hold`, `wrong_dose_panic`.
- **Approve one Reddit Answers actor** (§6). Ask that runs be tagged `job: raw-research` so SavePet spend shows separately. All 23 runs in the last 6 hours were untagged.
- **Tell the owner on Telegram that no Reddit research has run yet** (contradiction 4).
- **Copy the avatar profile into the SavePet repo** (`SavePet PetMergency Avatar Profile.pdf/.txt` from the main repo root). Correct the stale Supermemory memory about the main repo.
- **Search seeds already given by the owner** (from the decision and Telegram log; not run):
  - Subreddits: AskVet, dogs, DogAdvice, puppy101, cats, CatAdvice, Pets.
  - Terms: dog ate chocolate / grapes / rat poison / ibuprofen, cat ate lily, activated charcoal for dogs, peroxide to make a dog vomit, emergency vet bill.

  The lesson says to search these subreddits directly after Reddit Answers.
- **Watch for negative evidence once research runs.** The category likely includes owners and vets warning against home-induced vomiting or giving charcoal at home. That is a hypothesis, not checked. If it shows up, it should be logged verbatim as negative evidence next to the seller's claims.

## 10. Outputs of this run

- `01_petmergency_activated_charcoal_first_aid/raw/avatar_bank_2026-11-02/`: **not created.** There is no verbatim Reddit Answers output, and empty or placeholder raw files would misrepresent the research.
- `01_petmergency_activated_charcoal_first_aid/avatar/<problem>_EB_TEMPLATE.md` × 6: **not created.** The template file doesn't exist and the bank wasn't run.
- `course_v2/COVERAGE_V2.md` block 1 (Raw research): stays **unticked**.
- Apify spend for this run: **$0.00**.
- This report is the only file written.
