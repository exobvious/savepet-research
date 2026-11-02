# PetMergency Activated Charcoal First Aid Kit (SavePet): onboarding step three, the Zakaria avatar clean-up (merge, then cluster)

- **Run:** onboarding / 03-avatar-clean-up, 2026-11-02 (UTC), cloud research agent
- **Product folder:** `01_petmergency_activated_charcoal_first_aid/` in `exobvious/savepet-research`
- **Target output folder:** `01_petmergency_activated_charcoal_first_aid/avatar/cleanup/`
- **Status: BLOCKED. The stage was not run.**
  - Nothing was merged and nothing was clustered.
  - No file was written to `avatar/cleanup/`.
  - $0.00 was spent on Apify.
  - This report is the only file written.
- **Why it is blocked.** There are two separate reasons, and either one alone stops the stage.
  1. **No prompt is registered, and none can be found.** The playbook's Clean-up row, "Avatar clean-up prompts (merge, then cluster)", still says `ADD_ID`, and its Container column is empty. Nothing called "Zakaria" exists in:
     - the Scaler course library
     - Supermemory
     - either repo

     The playbook rule is: "A stage whose prompt column still says `ADD_ID` is reported as missing; the bot never reconstructs a prompt from memory or substitutes a similar one." AGENTS.md rule 2 says the same.
  2. **There is nothing to clean up yet.** Merge-then-cluster works on the output of the Avatar stage (sub-avatars and the deep dive). That stage has not run:
     - `avatar/` holds only `README.md`
     - no `<problem>_EB_TEMPLATE.md` exists
     - no sub-avatar list exists
     - there is no category context document
     - Reddit (the course's first and main channel) has still not run

     Even with the prompt, a merge/cluster pass on raw quotes would mean inventing the avatar layer the prompt expects.
- **What this run did instead, at $0:**
  - Read the Facebook dataset `uQBfIcoXY0boLKb5r`. It was paid for in step two but never read. This was a free read, no re-buy.
  - Listed everything pulled so far, so a future clean-up has a known base (§4–§5).
  - Updated the per-problem coverage (§6).

  None of this is clean-up output.

---

## 1. What was read (in order)

| # | Source | Result |
|---|---|---|
| 1 | `gateway_status` | scaler, vantage, apify and supermemory OK. **clickup: false** (not configured; no tasks are created by policy). GitHub OK. Apify today $2.18 before this run, no daily stop. |
| 2 | `get_playbook`: `UNIFIED_PLAYBOOK.md` (sha 02e8ca8) | **Clean-up row = `ADD_ID`, Container empty.** The Avatar row "Avatar research prompts (sub-avatars, deep dive)" is also `ADD_ID`, as is every other row. **The playbook names no Supermemory space** for prompts or for evidence. |
| 3 | `PRODUCT_DECISION.md` (sha 3f08d1e) | Six buyer problems (P1–P6). Competitors: "none given yet". Locked rules: page claims, "Made in USA" and "third-party tested" are seller claims. The avatar-profile quotes are illustrative and its numbers are hypotheses. Keep SavePet apart from Vylaras. |
| 4 | `product_truth.md` (sha a2a4a93) | 1 tube, $39.95. Coconut shell activated charcoal plus kaolin clay (page). Label, mL, supplier, origin and bundles **NOT CONFIRMED**. The page's dose guidance contradicts itself. |
| 5 | Step 1 report `01-raw-research-reddit-answers-bank.md` (sha ec5bca1) | BLOCKED. 0 of 156 Reddit Answers questions run, $0 spent. No raw files, no avatar templates. |
| 6 | Step 2 report `02-raw-research-thin-families-on-the-other-channels.md` (sha 78576b8) | PARTIAL. Amazon, YouTube and TikTok were read and kept. **Facebook was bought (30 posts) but not read.** Quora had no answer text. Reddit has still not run. The quote bank lives inside that report (§4), not in a category document. |
| 7 | `FULL_COURSE_TREATMENT.md` (sha 9133008) | Block 8, "Avatar research: sub-avatars, selection matrix, deep dive", is `ADD_ID`. **The 24-block table has no clean-up block**, so the clean-up exists only as a playbook registry row. |
| 8 | `AGENTS.md` (sha 60cd2dd), `NEVER_REPEAT_MISTAKES.md` (sha 42777e1, empty) | Rule 2: a stage with no ID is reported missing. Rule 3: keep evidence classes separate. Rule 4: two independent reports per angle. Rule 7: no ClickUp. |
| 9 | `telegram_log/2026-11-02.md` | The owner approved the pet-poisoning rewording and the Reddit run at 17:24 ("yes reword it for my offer then run the search"). Those steps are **not queued yet** because the queue was busy. Telegram called this step **"Cleaning up the buyer profile"** (16:38, 16:50). See contradiction §8.2. No clean-up prompt was given in chat. |
| 10 | Product folder listing | `avatar/README.md`: "Reddit Answers bank per problem (`<problem>_EB_TEMPLATE.md`) and `cleanup/`". **Neither exists.** `raw/` holds only its README. |
| 11 | Main repo `01_ai_translator_earbuds/.../2026-10-20/03-avatar-clean-up.md` (sha b537f0f) | The **same stage was blocked for Vylaras** on 2026-10-20 for the same two reasons. This is the second occurrence (see §9, idea 8). |

## 2. Where I looked for the clean-up prompt (none found)

| Source | Call | Result |
|---|---|---|
| Playbook registry | `get_playbook` | Clean-up = `ADD_ID` |
| Supermemory | `list_spaces` | One space only: `research_bot` (47 docs, 106 memories). There is no `courses` space. |
| Supermemory | `list_documents` (research_bot, all 47) | Telegram copies and step notices only. **No course prompt document.** |
| Supermemory | `search_memory` "Zakaria avatar clean-up prompt merge then cluster" | 10 hits, all status notes. For example, `ERjZf5SpESjmZg7KUXTaeu` "Merge or cluster prompt not registered for avatar clean-up." and `3qrCQMA8E98DfGbiLNexHJ` "Nothing called Zakaria exists in the course library." (both from doc `GMV5wU6YSg4jymvY1yqMZx`, the Vylaras clean-up notice). **No prompt.** |
| Scaler docs | `search_docs` ("avatar clean-up merge then cluster prompt", "Zakaria avatar cleanup merge duplicate avatars cluster", "clean up avatar research sub-avatars merge cluster") | No clean-up, merge or cluster lesson. The closest hit is doc 53, "Learn E-Commerce Builders (5): Angle & Avatar Expansion" (skool_url null). It is not a clean-up prompt. |
| Scaler docs | `list_docs` (full outline, 40+ docs) | **No doc by or titled Zakaria.** No clean-up or cluster lesson in any module. |
| Scaler community | `search_community` (keywords: avatar clean-up, merge avatars, cluster avatars, Zakaria, sub-avatars) | "Zakaria" appears only as a **separate instructor**: "they just doing what zakaria teaching in his copywriting about story telling" and "zakaria just went deeper into the hooks survival, fear, pain points, curiosity etc." (Polo, 2026-09-15, builders-chat). Also an unanswered question (Polo, 2026-07-02): "camm only gave a prompt to make avatars from researching the problem now after that stage … make a complete persona doc for it". **No clean-up prompt was shared.** |
| Repos | `search_project_files` "Zakaria" in `exobvious/research` and `exobvious/savepet-research` | **0 hits** in each. |

**Conclusion.** This is a hypothesis about where the prompt lives, not a finding. The Zakaria merge and cluster prompts most likely come from a separate course the owner has access to, outside the Scaler library the gateway can read. They can only be used after the owner uploads them and registers their IDs (§9). I did not write my own merge or cluster method.

## 3. Avatar inputs a clean-up would need, and their status

| Input | Expected location | Status |
|---|---|---|
| Per-problem avatar templates (P1–P6) | `avatar/<problem>_EB_TEMPLATE.md` | **MISSING.** The Reddit bank (step 1) never ran. |
| Category context document | `EB_CATEGORY_CONTEXT_<category>_v2.md` | **MISSING.** Step 2's quote bank sits inside its report. The filename has not been chosen. |
| Avatar stage output (sub-avatars, selection matrix, deep dive) | `avatar/` / `course_v2/` (block 8) | **MISSING.** Prompt is `ADD_ID` and the stage has not run. |
| Owner's avatar research profile | `exobvious/research` root: `SavePet PetMergency Avatar Profile.pdf` / `.txt` | It exists, but it is **a written summary, not course avatar output**. `PRODUCT_DECISION.md` locks its quotes as illustrative and its numbers as hypotheses. It has not been copied into the SavePet repo, and the copy-and-compare step is still unqueued (Telegram 16:40, 17:25). I did not merge it with anything. |

## 4. Facebook dataset read this run (step two's unread purchase)

- **Dataset:** `uQBfIcoXY0boLKb5r`, from run `mciIc7HradgHcKWf8` (actor `lofomachines/facebook-groups-posts-search-scraper`, job `raw-research`, $0.15, bought in step two).
- **Read:** all 30 of 30 items, with `get-dataset-items` at no charge.
- **Searches it came from:** "dog ate chocolate emergency vet" and "activated charcoal dog poison" (country: us).
- **What was pulled:** post text only. **No comments were bought.**
- **Composition:**
  - 26 owner posts. Two of them carry identical text under two different names, so I count them as **25 distinct owners** (§8.4).
  - 1 groomer (pro).
  - 1 vet-education page (pro).
  - 1 affiliate recommendation post (`competitor_claim`).
  - 1 anonymous "looking for" post.
- **Scraper quirk:** for several posts the `group_name` field holds the post title instead of the group name. The `group_url` values are correct.

These are verbatim, typos included. They are raw evidence for the category document. **They are not clean-up output.**

### 4.1 Emotional experience / catalyst (the moment)
- "Is there anything I should do right now? **It's 1138 at night.** Has anyone had anything like this happen and what did you do and what did you notice? 😳😳😳". Stephanie Swann, French Bulldog Owners, https://www.facebook.com/groups/7138117442873230/posts/26281064311485256/, 2026-02-02, **283 reactions, 595 comments**. customer_report **(P1, P3)**
- "My dog swallowed my mothers naproxen pill we induced vomiting and gave activated charcoal. Do i need to take her to emerge still ? **I'm freaking out help**". Karen Lunning, https://www.facebook.com/groups/asktheveterinarian/posts/1520850722800456/, 2026-03-17. customer_report **(P2, plus charcoal used at home)**
- "Hello vets, I'm wondering if I have an immediate emergency. My 9.5 pound … Chihuahua/Pug mix consumed a small piece of my 53% dark chocolate covered rice crispy". Deanna Christopher, Pet Vet Corner, https://www.facebook.com/groups/petvetcorner/posts/1736493917374636/, 2026-06-11, **257 comments**. customer_report
- "Help! Just caught my 50lb Blue healer with a Hershey's chocolate bar… Should I call my vet or take her to emergency vet?" Jessica Lynn, https://www.facebook.com/groups/petvetcorner/posts/1602998844057478/, 2026-01-07. customer_report
- "My dog ate a piece of chocolate that was on the floor now she has diarrhea. I don't know what to do how do I treat this? please help". Michelle Coppersmith, Chihuahua Parents, https://www.facebook.com/groups/chihuahuaparents/posts/25798389799841369/, 2026-01-24, 99 comments. customer_report
- "My lab puppy has ingested a bunch of chocolate and I need some advice on what to do please". Cody Allen, https://www.facebook.com/groups/petvetcorner/posts/1637188857305143/, 2026-02-16. customer_report
- "he is acting fined but when i google it is sayin take him to vet right now … should i take him to emergency vet right now." Denise Everhart, https://www.facebook.com/groups/lynchburgrecommendations/posts/1964171084555916/, 2026-11-01, 82 comments. customer_report
- "Lf activated charcoal for dogs asap". Anonymous, https://www.facebook.com/groups/326828460987298/posts/3044464939223623/, 2026-10-27. customer_report **(P1: nothing at home, looking to get it right now)**

### 4.2 Nothing at home / cost (P1, P4)
- "my dogs got on counter and ate chocolate unfortunately **I dont have funds for vet til next week** is there anything I can do at home to counter the chocolate so wife and I dont lose our fur babies?" Christopher Johnson, The Lee's Summit Community, https://www.facebook.com/groups/theleessummitcommunity/posts/28439017415799009/, 2026-10-23, 90 comments. customer_report **(P1, P4)**
- "What can I give a dog that seemed to have picked up poison?" Cassandra Rowe, https://www.facebook.com/groups/2185259998371204/posts/4797300193833825/, 2026-10-07, **167 comments**. customer_report **(P1)**
- "**I can not find activated charcoal in the stores anywhere.** Has anyone ever used human activated charcoal for substitute?" Alison Townsley Runk, https://www.facebook.com/groups/petvetcorner/posts/1684184149272280/, 2026-04-12, 55 comments. customer_report **(P1: can't buy it in time)**
- "Rooster managed to counter surf his way into a bag of chocolate chips and ended up with chocolate poisoning. Thankfully he's on the mend after a **$600 vet visit** 😩🐾🍫". "Must Love Dogs", Dogalogue, https://www.facebook.com/groups/dogalogue/posts/1869962833683603/, 2026-03-09. customer_report (a page-style name) **(P4)**
- "I have a problem with my dogs being poisoned by toads/frogs.... **the medical bills are just insane!!** How can I treat them at home … I have 5 beautiful shepards". Community Animal Rescue – Belize City, https://www.facebook.com/groups/communityanimalrescue/posts/2823914071316110/, 2026-06-10. customer_report **(P4; outside the US)**
- "We took her to the ER where they gave her fluids and took an X-ray to make sure her stomach didn't flip. They sent us home with anti nausea and pain meds". Kelly Diavola, https://www.facebook.com/groups/2723594934465209/posts/3663396577151702/, 2026-10-29. customer_report (what the ER actually did; no cost stated)

### 4.3 Peroxide / inducing vomiting (P2)
- "got a hold of a chocolate chip cookie … not sure if he ate the other half. **Should I induce vomiting?**" Loudoun Valley, Ask the Veterinarian, https://www.facebook.com/groups/asktheveterinarian/posts/1584055409813320/, 2026-06-01. customer_report
- Karen Lunning (§4.1): "we induced vomiting and gave activated charcoal". customer_report

### 4.4 Dosing and timing in a panic (P6)
- "I have the Now charcoal. **How much do I give a 60 pound pit and a 37 pound Pittie mix.**" Amy Glaeser, Saving Pets One Pet @ A Time, https://www.facebook.com/groups/DuncanStrong/posts/2078592759537933/, 2026-04-29. customer_report (multi-dog household, human-brand charcoal)
- "I don't want to be a nervous Nelly but **when do you know when to administer the charcoal?**" Then the post's own update: "****Update, I will have it on hand if the time comes that the vet says so.****" Lynette Diel Mangels, Aussie Friends, https://www.facebook.com/groups/837889829591939/posts/27967074699580085/, 2026-09-03. customer_report **(P6 is about *when*, not only *how much*)**
- "Have charcoal capsules, should I give her some? She's 3 years old and weighs around 55/60lbs". Then the update: "she's fine. No issues no puking no pooping." Toula Helen, https://www.facebook.com/groups/asktheveterinarian/posts/1571570144395180/, 2026-05-17. customer_report
- "My dog ate approx 2 tablespoons of dry cocoa she is 70 lbs do we need to go to the vet?" Laurie Szumla, Holistic & Natural Pet Care, https://www.facebook.com/groups/holisticandnaturalpets/posts/4522115424718660/, 2026-11-01. customer_report

### 4.5 Bought "just in case" (pre-emptive buyers)
- "I have activated charcoal and I know it's suppose to be used if he eats poison but is that it? **Just bought it to have on hand just in case.**" Linseed Do, https://www.facebook.com/groups/holisticandnaturalpets/posts/4520364248227111/, 2026-10-30. customer_report
- "decided to get some emergency charcoal for the just in case. I have an 11 month old girlie that finds everything to chew on … I c@nt control what she may find on a walk". Lynette Diel Mangels (above). customer_report
- "I bought activated charcoal as precaution for poisoning situations. **But my vet didn't like the fact that I bought it.** What do you guys think?" Donna Dupont, Love ❤️ Of Yorkies, https://www.facebook.com/groups/514612959043998/posts/2623712288134044/, 2026-09-08. customer_report **(trust: vet disapproval)**

### 4.6 Trust, proof and negative evidence
- "I live in Florida where we have cane toads. It's been my worst nightmare since moving here … **I'm seeing some stuff advertised now by Vetanica.** It's an activated charcoal syringe … **Before I take the bait - does anyone know if it's legitimate?** … this seems like a newer ad I'm seeing and I want to do my HW first." Nicole Graziano, Holistic Pet Care, https://www.facebook.com/groups/holisticdomesticpetcare/posts/2016643172330081/, 2026-09-11, 45 reactions, 35 comments, 6 shares. customer_report.
  - Ad skepticism toward a direct competitor's Facebook ads.
  - A **second Florida-toad report** after Amazon R2B4Q34V2L7YAV in step two.
- "Keep chocolate out of your pet's reach—and if ingestion occurs, contact a veterinarian promptly." VetCareHub, Veterinary Jobs Worldwide, https://www.facebook.com/groups/vetjobsworldwide/posts/1090011996996990/, 2026-10-22. pro_opinion (education post)
- "Everyone should have activated charcoal on hand for an emergency. it works great for pets and humans." The same post links NOW Activated Charcoal, a "60ml EZ Dose Bottle" gel and a powder through `amzn.to` affiliate links. It then says "**Do not administer activated charcoal unless instructed.**" and "human products may contain sweeteners like xylitol". Kelly Bone, Saving Pets One Pet @ A Time, https://www.facebook.com/groups/DuncanStrong/posts/2037119440351932/, 2026-03-10. **competitor_claim** (affiliate). The post contradicts itself.
- "the vet have to use activated charcoal to induce vomiting. What is good to help with the **black staining** from the charcoal?" Ashley Lehua Swartz (writing about a client's white Maltese, so a pro or groomer), https://www.facebook.com/groups/1542021025906490/posts/27993132663701966/, 2026-09-14.
  - Mechanism misconception: charcoal is assumed to make the dog vomit.
  - New objection: staining of white coats.
- "would it be ok to do the activated charcoal gel for a **one time detox** to clear out their system? I read on there that it can help with gut issues." Lisa Potter, https://www.facebook.com/groups/DuncanStrong/posts/2004915606905649/, 2026-01-29. customer_report. **Off-label "detox" use.** This is a claims and compliance risk, watch-only.
- "we have to syringe charcoal down them … we'll have to get up at four in the morning … as we've have to do it every four and six hours". Paree Jarvis, Maine Coons UK, https://www.facebook.com/groups/mainecoonsuk/posts/1474471548195569/, 2026-11-01. customer_report. Vet-directed, **multi-dose** charcoal after raisins, in a cocker spaniel puppy. **UK, not US.**

### 4.7 What Facebook did not give
- **No poison control fees and no hold-time complaints (P5: 0).** No poster says they called poison control. They ask the group instead, with 595, 257 and 167 comments on the biggest threads. That is an observation about behaviour, labelled `hypothesis`: crowdsourcing in the moment may stand in for the hotline.
- **No literal "the vet is closed" language (P3).** Night is implied ("1138 at night"), not stated as closure.
- **Cats:** no owner post about a cat poisoning in this pull. The Maine Coons UK post is about a dog.

## 5. Inventory: everything pulled so far for SavePet

These are counts only. **No merging or clustering was done.**

| Channel | Source run / dataset | Bought | Read | Kept (distinct people) | Where it lives |
|---|---|---|---|---|---|
| Reddit Answers + subreddits | none | 0 | 0 | 0 | **Not run** (approved 17:24, not queued) |
| Amazon listings | bmIlKTBEAo5ZMXdAH / iYklexFOx41Uh6Rx7 | 10 | 10 | listing data only | Report 02 §5 |
| Amazon reviews (helpful) | zpV1HpHWN7f2FdBap / Da2ivMrrTuvpdIR5n | 36 | 36 | 22 | Report 02 §4 |
| Amazon reviews (critical) | CYkmzt09mXXREEpLR / cxM8wT7E2E0nPOP8e | 8 | 8 | 3 | Report 02 §4 |
| YouTube search | pKploE4hWEaZ2vVFX / eZYd73zYQIuOpndsg | 15 videos | 15 | 4 chosen | Report 02 §3 |
| YouTube comments | 51s7iPvR1eeqkygIW / DNJAqKFgeHTwWtV0p | 80 | 80 | 26 | Report 02 §4 |
| TikTok search | YSwu7LfFtNqKXRObj / VBkj0hMIJsDIP0xXE | 20 | 20 | captions = competitor_claim | Report 02 §4–5 |
| TikTok comments | UdBUPRzpCDjWcFiWv / yOhyIAyBMiC8IQ0oz | 100 | 100 | 24 | Report 02 §4 |
| Quora | L9SinbOHUq1tdpAeZ, vuPNVMPy26UBt6Qoy | 8 | 8 | 1 story + 2 titles | Report 02 §4.8 |
| **Facebook groups** | mciIc7HradgHcKWf8 / **uQBfIcoXY0boLKb5r** | 30 | **30 (this run)** | 25 owners + 1 anonymous owner + 2 pro + 1 affiliate | **This report §4** |
| Failed or empty pulls | I4oWg…, tg9BR…, 8IceD…, nJfZZ…, wndUe… | n/a | n/a | 0 | Report 02 §6 |

- **Customer voice base today:** about 75 kept customer quotes from Amazon, YouTube and TikTok (report 02), plus 26 Facebook owner posts (this run).
- **All of it is category-level.** None mention SavePet or PetMergency.
- **Product mentions:** the only product-specific customer voice is about PawMergency (B0FXBQSFJP), PetVet Medic (B0FNY9J7ZT), powder (B0CN6JLXLS), NOW (human charcoal) and Vetanica (Facebook ad).
- **Apify spend:**
  - SavePet `raw-research` total, per `list_apify_runs` (8 h): **$0.70 across 13 runs**.
  - This run: **$0.00**. Only free dataset reads and the free run listing were used.

## 6. Coverage by buyer problem (report 02's table, updated with Facebook)

Counts are distinct people with kept quotes. "Covered" means three or more people. It is **not** the AGENTS rule-4 angle bar.

| Problem (verbatim from `PRODUCT_DECISION.md`) | After report 02 | After this run | Note |
|---|---|---|---|
| P1 "My dog ate something toxic and I have nothing at home to help" | covered | covered (+5) | Johnson, Rowe, Swann, Runk ("can not find activated charcoal in the stores"), "Lf … asap" |
| P2 "Should I make him throw up with peroxide?" | covered | covered (+2) | Loudoun Valley, Lunning |
| P3 "The vet is closed at night" | thin (3 indirect) | **thin (4 indirect)** | Adds Swann "1138 at night". **Nobody has yet said the vet was closed.** Needs Reddit. |
| P4 "A $2,000 emergency vet bill" | covered | covered (+3) | **Real figures so far: $600, a $1,000 deposit, and "2 grand" (one TikTok comment).** Also "dont have funds for vet til next week" and "medical bills are just insane". The profile's $2,000 has **one** report. |
| P5 "Poison control charges a fee and puts me on hold" | thin (1: $65) | **thin (unchanged)** | Facebook added 0. The profile's $95 is still unsupported. Needs its own search, Reddit first. |
| P6 "I'm scared I'd give the wrong amount in a panic" | covered | covered (+4) | Glaeser, Mangels, Helen, Szumla. **New nuance: owners are unsure *when* or *whether* to give it, not only how much.** |

## 7. Recurring situations seen in the raw quotes (signal list, not avatars)

> These are `hypothesis` labels for the owner and for the future avatar stage. They are **not** sub-avatars. They have no emotional-driver, behaviour or belief layer, and they were **not merged or clustered**. That is the job of the unregistered Avatar and Clean-up prompts.

| Situation | People seen (sources) |
|---|---|
| Puppy or "eats everything" dog | ≥6 (Amazon "My puppy eats everything!", "inhale chocolate"; Facebook Mangels "finds everything to chew on", Allen "lab puppy"; YouTube "3 puppies") |
| Toad region (Florida, Belize) | 4 (Amazon R2B4Q34V2L7YAV, R3ULWZZTQKMD4U; Facebook Graziano, Belize post) |
| Can't afford the vet right now | ≥4 (YouTube "don't have money to take them", Facebook Johnson, Belize post, Amazon "saves me from extra vet costs") |
| Bought "just in case" before any incident | ≥6 (Facebook Linseed Do, Mangels, Dupont; Amazon "Hope I never have to use it" ×3) |
| Owner-caused exposure (guilt) | ≥4 (left grapes, husband's Warfarin, mother's naproxen, "looked away for two seconds") |
| Multi-pet household | ≥4 (5 shepherds, two pits, "all babies in your home", three puppies) |
| Holistic / natural-care group member | 4 Facebook posts from holistic groups (Szumla, Earp, Linseed Do, Graziano) |

## 8. Contradictions and open questions

1. **The stage is named but its prompt is absent.** The run instruction names a "Zakaria avatar clean-up stage (merge, then cluster)". The registry says `ADD_ID`, and the only "Zakaria" in reach is a separate instructor mentioned in the Scaler Discord. This is the **second time** in a row the stage has been queued without its prompt (Vylaras 2026-10-20 was the first).
2. **"Buyer profile clean-up" vs the "Zakaria merge/cluster".** On Telegram (16:38, 16:50) the assistant described this queued step as "Cleaning up the buyer profile". The owner may therefore expect her avatar profile to be tidied and checked. That is a different job. The copy-and-compare step the assistant promised at 16:40 and 17:25 is what does that, and it is still not queued. **Nothing was done to her profile in this run.**
3. **Order.** The clean-up was queued as step 3, straight after a partial raw research and before any of these had run: Reddit, category context, deep research, and the avatar stage (block 8). The playbook's research order and the course (doc 53: "BROAD >> VALIDATE >> GO DEEP") put avatar breakdown after those, and merge/cluster after the avatars exist.
4. **Duplicate Facebook post.** The same text, word for word ("I just got home from an event and I found this Hershey's bar on the floor … It's 1138 at night …"), appears under Stephanie Swann (French Bulldog Owners, 2026-02-02, 595 comments) and under "Frenchie Moments." in an unrelated "Bariatric Tips Tricks & Recipes 2025" group five days later (https://www.facebook.com/groups/265073846009062/posts/941900958326344/). It is likely a repost or engagement copy, so it is counted as **one** person.
5. **"Have it on hand" vs "only when the vet says".**
   - Several just-in-case buyers end up deferring to the vet: Mangels' update, and Dupont's "my vet didn't like the fact that I bought it".
   - The affiliate post says both "Everyone should have activated charcoal on hand" and "Do not administer activated charcoal unless instructed."
   - Together with report 02's vet-staff warnings (2,533-like TikTok comment), the evidence keeps supporting **"charcoal plus the call to your vet"** framing, not "instead of the vet".
6. **Mechanism confusion recurs.** The groomer post ("the vet have to use activated charcoal to induce vomiting") is now the third report of charcoal being linked with vomiting. The others are Amazon R22OQU9696DWL7 (the buyer expected vomiting) and report 02's credit reviews. Charcoal binds toxins and does not cause vomiting. Copy that explains this is both a risk and an education opportunity. **The mechanism itself is not verified for this product's label.**
7. **Untagged Apify runs keep running.**
   - `list_apify_runs` (8 h) shows **24 untagged Facebook Ads Library runs** (actor `XtaWFhbtfxyzqrFmd`), the newest at 18:28 UTC (`5Az1EeLofPUNffBTG`, $0.046). That is after both earlier reports flagged them.
   - Step two's two `apify/web-fetch` runs (`I4oWgcaRGs0ePJJ2P`, `wndUeDqw6EcmKVFKP`) also show as `untagged`, although that step says it ran under job `raw-research`.
8. **Stale memory.** Supermemory memory `rt13wF2CCVkUvpbA7krzhy` ("research for SavePet should use the main repo exobvious/research") still conflicts with the owner's choice of `exobvious/savepet-research`. I did not edit memories.
9. **Non-US posts are in a US-filtered search:** Belize, Singapore and UK posts. They are kept, and the country is labelled on each.

## 9. Ideas for the owner (not tasks; nothing was assigned or scheduled)

Ordered by what unblocks the most:

1. **Upload the Zakaria clean-up prompts.** Upload each prompt (merge, cluster) and its lesson as its own Supermemory document. A `courses` space works, or `research_bot`. Then paste the IDs into the playbook's **Clean-up** row and name the container. Do the same for the **Avatar research prompts** row (block 8), whose output the clean-up consumes. Until both exist, re-queuing this step will block again.
2. **Say what this step should mean.** Is it the course's merge-then-cluster of sub-avatars, or "tidy my avatar profile"? If it is the second, the copy-and-compare step (Telegram 16:40) is the right step, and it can run now with no course prompt.
3. **Queue in course order once the queue is free:**
   1. the pet-poisoning rewording of the 26 questions
   2. the Reddit run (both approved 17:24)
   3. the copy-and-compare of the profile
   4. the category context document, with report 02 §4 plus this report §4 pasted in
   5. deep research
   6. the avatar stage
   7. **only then** this clean-up, into `avatar/cleanup/`
4. **Point Reddit at P3 and P5 hardest.** Search "vet closed", "no emergency vet near me", "poison control fee", "ASPCA poison control charge", "pet poison helpline hold". The $95 fee and the $2,000 bill stay hypotheses until Reddit backs them: the only real figures so far are $65, $600, a $1,000 deposit and one "2 grand".
5. **Optional, after Reddit: pull comments on the four Facebook posts directly about the buyer's problem.** They are Swann (595 comments), Christopher (257), Rowe (167) and Coppersmith (99). That's where owners answer each other in the moment. It would be a new purchase, and I have not priced it.
6. **Competitor candidates for `PRODUCT_DECISION.md`:**
   - **Vetanica**, seen advertising a charcoal syringe on Facebook to Florida toad owners, and present as a TikTok handle in report 02
   - **NOW Activated Charcoal**, a human product used by owners and pushed by affiliates
   - PawMergency and PetVet Medic, from report 02

   Vantage could check Vetanica's ad structure. That is market intelligence only, never proof.
7. **Objections to log for copy:**
   - "my vet didn't like the fact that I bought it"
   - "does anyone know if it's legitimate?" (ad skepticism)
   - black staining on white coats
   - human charcoal as a cheaper substitute (xylitol risk, per the affiliate post)
   - off-label "detox" use, which should not be invited in claims
8. **A proposed line for `NEVER_REPEAT_MISTAKES.md`.** This has now gone wrong twice (Vylaras 2026-10-20, SavePet 2026-11-02):
   > "Don't queue avatar clean-up until the avatar stage has written files to `avatar/` and the Clean-up row has a registry ID (2026-11-02, second occurrence)."
9. **Find what is starting the untagged Facebook Ads Library runs** (§8.7), and make the `job` tag stick on `web-fetch` runs.
10. **Add the clean-up to `FULL_COURSE_TREATMENT.md`**, under block 8 or as its own row, so `COVERAGE_V2.md` can tick it once it runs.
11. **Correct the stale Supermemory memory** `rt13wF2CCVkUvpbA7krzhy`.

## 10. Unavailable or failed sources

- **Clean-up prompt (merge, then cluster):** MISSING from the registry, Supermemory, Scaler docs, the Scaler community and both repos.
- **Avatar stage prompt:** MISSING (`ADD_ID`).
- **Supermemory course space:** none. The only space is `research_bot`, which holds chat logs and step notices.
- **Reddit:** still not run (step one blocked; approved but not queued).
- **Quora answers:** still MISSING (report 02).
- **ClickUp:** not configured and not used. No tasks were created.
- **Vantage:** not used. It gives ad structure only and is never avatar evidence.
- **Tool failures this run:** none. The stage stopped on missing inputs, not on a source error.

## 11. Outputs of this run

- `01_petmergency_activated_charcoal_first_aid/avatar/cleanup/`: **not created.** There is no registered prompt and no avatar input. A placeholder or improvised merge/cluster file would misrepresent the course's output.
- `course_v2/COVERAGE_V2.md`: unchanged. No block ticked.
- Rating out of 10: **not applicable.** There is no block output to rate.
- Facebook dataset `uQBfIcoXY0boLKb5r`: read in full (30 of 30). Its kept quotes are in §4, ready to be added to the category document as `## Added 2026-11-02: Facebook groups`.
- Apify: **$0.00** this run.
- This report is the only file written.
