# PetMergency Activated Charcoal First Aid Kit (SavePet): Reddit Answers question bank reworded for pet poisoning

- **Run:** telegram / 01-reword-reddit-questions, 2026-11-02 (UTC), cloud research agent
- **Product folder:** `01_petmergency_activated_charcoal_first_aid/` in `exobvious/savepet-research`
- **Brand:** SavePet (confirmed by the owner on Telegram at 16:40, not "SavePets")
- **Status: DONE (writing step only).** The 26 lesson-3 questions are copied word for word (§2). Each one has a reworded pet-poisoning version (§3). The six buyer problems are turned into search phrases (§4), and all **156 ready-to-type questions** are listed by problem (§5), with dog and cat variants (§6).
- **Spend: $0.00.** No Apify actor was called. The only calls were free reads: Scaler `get_doc`, Supermemory `search_memory`, and GitHub.
- **No searching was done in this step.** No Reddit Answers question was run and no quotes were collected. As the owner approved, the search is the next step and has no further approval gate.
- **No product claims.** The questions ask about the owner's situation. None of them says what the product does. Nothing here goes beyond `product_truth.md`.

---

## 1. What was read, and the owner decisions applied

| # | Source | Result |
|---|---|---|
| 1 | `gateway_status` | scaler, vantage, apify and supermemory were OK. **clickup: false** (and no tasks are created by policy). GitHub OK. |
| 2 | `get_playbook` (UNIFIED_PLAYBOOK.md, sha 02e8ca8) | The prompt registry still says `ADD_ID` for "Raw research lesson" and "Problem question bank", and the Container column is empty. The playbook also says: "A decision made there [Telegram] counts the same as one made here." The owner's Telegram decisions below therefore fill the gap for this step. |
| 3 | `get_playbook raw-research` (RAW_RESEARCH_METHOD.md, sha f11ed6d) | "A problem never covered runs all the bank questions. Never re-run a question already in the document." |
| 4 | `get_playbook course-treatment` (FULL_COURSE_TREATMENT.md, sha 9133008) | Block 1 is raw research. Every prompt column says `ADD_ID`. |
| 5 | `00_rules_and_process/RAW_RESEARCH_METHOD.md` with repo `exobvious/savepet-research` | **HTTP 404.** The file is not in the SavePet repo. It lives only in the main repo, and I read it there through the playbook (row 3). Noted as a gap, not a blocker. `00_rules_and_process/` in the SavePet repo lists 0 files. |
| 6 | `product_truth.md` (sha a2a4a93) | 1 tube at $39.95 (shown as down from $80). Named on the page: coconut shell activated charcoal and kaolin clay. Dial-a-dose applicator, 1 mL per lb (and the page's dose guidance contradicts itself). Everything else is NOT CONFIRMED. |
| 7 | `PRODUCT_DECISION.md` (sha 3f08d1e) | The six buyer problems, quoted verbatim in §4. Page claims are seller claims. The profile's numbers are hypotheses. |
| 8 | Report `onboarding/2026-11-02/01-raw-research-reddit-answers-bank.md` (sha ec5bca1) | BLOCKED on four things: lesson not registered, 26 vs 27, skincare wording, and no approved tailoring. Decisions (1)–(3) below clear all four for this step. |
| 9 | Report `onboarding/2026-11-02/02-raw-research-thin-families-on-the-other-channels.md` (sha 78576b8) | Other channels ran before Reddit. P3 (vet closed at night) and P5 (poison control fee and hold) are **thin**. The other problems are covered across the category. That report's customer words shaped the phrasing below (for example "freaking out", "12:00am", "($65)", "how large a dose"). |
| 10 | `00_rules_and_process/telegram_log/2026-11-02.md` (main repo, sha 6e756ca) | 17:24, the owner: "yes reword it for my offer then run the search". 19:34: the three approved steps are queued (reword at $0, then the Reddit search capped at $6, then copying the profile). |
| 11 | Scaler `get_doc(51)`: "Learn E-Commerce Builders (3): Raw Research and Category Context for Copywriting" (parent "Creative Strategy", skool_url null) | Read in full. The "Reddit Answers Question Bank" section holds **26 questions in 7 families**. The lesson's tailoring prompt: "adjust these questions so it is relevant to our category. Also make sure that this is specifically targeted towards [the audience]." Rule: "Run all of the questions through Reddit Answers. Do not skip any." |
| 12 | Supermemory `search_memory` ("SavePet Reddit Answers question bank pet poisoning reworded") | **No matching memories.** No earlier tailored bank exists to reuse or contradict. (The first call failed on a wrong argument name, `q`. The retry with `query` worked.) |
| 13 | `list_project_files` bot_reports | There is no `telegram/` folder yet, so this path is new. Reports 03–05 exist and were not needed for this step. |

**Owner decisions applied (from Telegram, treated as approved):**
1. The course lesson for the Reddit Answers bank is **E-Commerce Builders lesson 3** (Scaler doc 51).
2. Use **its 26 questions as written**. The earlier "27" was a setup error, so no 27th question was added.
3. **Reword the questions for pet poisoning and this offer.** The search runs in the next step with no further approval gate.

**How the lesson's tailoring step was followed.** The lesson's own prompt rewrites the templated questions "so it is relevant to our category" and targets the audience. For SavePet:
- The category is "Pet first aid / at-home pet poisoning response" (PRODUCT_DECISION).
- The audience is dog and cat owners.
- The owner's profile describes the buyer as mostly women aged 27–42, but that is a hypothesis. So the questions say "pet owners", "dog owners" and "cat owners", not "women". If the owner wants the lesson's audience targeting applied literally, a "women who…" prefix is an easy option, but I did not do it.

---

## 2. The 26 lesson-3 questions, verbatim

Source: Scaler doc 51, section "Reddit Answers Question Bank". Punctuation is copied as given, including the double hyphens.

**EMOTIONAL EXPERIENCE**
1. What makes people feel the most insecure about [problem]?
2. What’s the most frustrating part of dealing with [problem]?
3. What does a “bad day” with [problem] look like?
4. What’s something people don’t understand about having [problem]?

**FAILED ATTEMPTS & FRUSTRATION**
5. What have people tried to fix [problem] that didn’t work?
6. What’s the biggest waste of money or time people have spent trying to fix [problem]?
7. What ingredients or methods made [problem] worse?
8. Why do people think nothing works for [problem]?
9. What do most products for [problem] get wrong?

**BELIEFS & SELF-IMAGE**
10. Why do people believe [problem] happens to them?
11. Do people think [problem] can actually be fixed, or have they accepted it?
12. How has [problem] changed how people see themselves or their confidence?
13. What words do they use to describe themselves because of [problem]?
14. What’s the most ridiculous or unhelpful thing someone’s said to them about [problem]?

**TRANSFORMATION & HOPE**
15. What made people finally decide to do something about [problem]?
16. What would fixing [problem] allow them to do or feel again?
17. What’s life like after solving [problem]?
18. What’s something small but meaningful that improved once they fixed [problem]?

**LANGUAGE, VOICE & EXPRESSION**
19. What metaphors or analogies do people use when talking about [problem]?
20. What exact phrases, jokes, or slang do they use when describing [problem]?
21. How do people express frustration -- calm, sarcastic, hopeless, angry, or funny?

**TRUST & PROOF**
22. What kind of proof or results make people finally believe something works for [problem]?
23. What stories or visuals do they consider real versus fake?
24. Who do they trust most -- peers, dermatologists, influencers, or brands?

**CATALYST MOMENTS (BUYING PSYCHOLOGY)**
25. What’s the moment people realize they can’t ignore [problem] anymore?
26. What emotional state are they in right before trying one last thing?

Count check: 4 + 5 + 5 + 4 + 3 + 3 + 2 = **26**.

---

## 3. Reworded pet-poisoning template, one to one

`{X}` is the problem slot (see §4). "Pet owners" becomes "dog owners" or "cat owners" where the problem is species-specific.

| # | Course question (intent kept) | Pet-poisoning version | What changed and why |
|---|---|---|---|
| 1 | feel most insecure about | What makes pet owners feel the most **guilty, scared or helpless** about {X}? | In an emergency, "insecure" shows up as guilt and helplessness. Our data already has "a huge mistake… for the human". |
| 2 | most frustrating part | What's the most frustrating part of dealing with {X}? | Same wording. |
| 3 | a "bad day" | What does a **"bad night"** with {X} look like for pet owners? | Poisonings in the data cluster late at night ("12:00am", "1138 at night"). For P4 the version below keeps "bad day". |
| 4 | what people don't understand | What's something people don't understand about going through {X}? | "Having" a condition becomes "going through" an event. |
| 5 | tried to fix, didn't work | What have pet owners **tried at home** for {X} that didn't work? | "Fix" becomes what was tried at home. Our data has failed peroxide attempts. |
| 6 | biggest waste of money or time | What's the biggest waste of money or time pet owners have spent trying to deal with {X}? | "Fix" becomes "deal with". |
| 7 | ingredients or methods made it worse | What **home remedies, methods or advice** made {X} worse? | Skincare "ingredients" becomes home remedies and advice. |
| 8 | think nothing works | Why do pet owners feel like nothing they have at home helps with {X}? | Same intent. |
| 9 | what products get wrong | What do most **pet first aid products and kits** get wrong about {X}? | Products in the category, with no brand named. |
| 10 | why it happens to them | Why do pet owners believe {X} happened to them (**whose fault** do they think it was)? | The self-blame angle ("their human looked away for two seconds"). |
| 11 | can be fixed, or accepted | Do pet owners think {X} can actually be **handled at home**, or have they accepted they just have to rush to the vet? | Solvable vs. resigned, reframed for an emergency. |
| 12 | how they see themselves / confidence | How has {X} changed how owners see themselves **as pet owners**, or their confidence in an emergency? | Self-image as a pet parent. |
| 13 | words for themselves | What words do pet owners use to describe themselves after {X}? | Same intent (e.g. "numb knuckle"). |
| 14 | ridiculous or unhelpful thing said | What's the most ridiculous or unhelpful thing someone has said to pet owners about {X}? | Same intent. |
| 15 | finally decided to do something | What made pet owners finally decide to **act, or get prepared**, after {X}? | Covers acting in the moment and preparing for next time. |
| 16 | what fixing would let them do or feel | What would **having a plan for** {X} let pet owners do or feel again? | "Fixing" a one-off emergency means being ready for it. |
| 17 | life after solving | What's life like for pet owners **after** {X}, once they feel prepared? | After the event, plus feeling prepared. |
| 18 | small but meaningful improvement | What's something small but meaningful that changed once pet owners felt ready for {X}? | Same intent. |
| 19 | metaphors or analogies | What metaphors or analogies do pet owners use when talking about {X}? | Same wording (e.g. "an EpiPen for your curious ones"). |
| 20 | exact phrases, jokes, slang | What exact phrases, jokes, or slang do pet owners use when describing {X}? | Same wording. |
| 21 | how frustration is expressed | How do pet owners express frustration about {X} -- calm, sarcastic, hopeless, angry, or funny? | The course list is kept unchanged. Topic added because the original had no [problem] slot. |
| 22 | proof that makes them believe | What kind of proof or results make pet owners finally believe something works for {X}? | Same wording. |
| 23 | stories or visuals, real vs fake | What **stories or videos** about {X} do pet owners consider real versus fake? | "Visuals" becomes videos. Our data has TikTok affiliate pushback ("stop trying to falsely promote this"). Topic added because the original had no slot. |
| 24 | peers, dermatologists, influencers, brands | Who do pet owners trust most about {X} -- **their vet, an emergency vet, a pet poison hotline, other owners online, or brands**? | Dermatologists become vet, emergency vet and pet poison hotline. Peers become other owners online. "Influencers" is folded into "other owners online / brands", per the owner's list. |
| 25 | can't ignore it anymore | What's the moment pet owners realize they can't ignore **the risk of** {X} anymore? | The risk, not a chronic condition. |
| 26 | emotional state before one last thing | What emotional state are pet owners in right before they try one last thing **when** {X}? | Same intent. Topic added because the original had no slot. |

---

## 4. The six buyer problems as search phrases

| ID | Problem (PRODUCT_DECISION.md, verbatim) | Short search phrase (owner's wording, also used for direct subreddit search) | Slot form used inside the questions | Species |
|---|---|---|---|---|
| P1 | My dog ate something toxic and I have nothing at home to help | my dog ate something toxic | their dog ate something toxic (and they had nothing at home to help) | dog as registered; cat variant in §6 |
| P2 | Should I make him throw up with peroxide? | making my dog throw up with peroxide | making their dog throw up with hydrogen peroxide | dog only as written; cat variant in §6 |
| P3 | The vet is closed at night | vet closed at night | the vet being closed at night when their pet ate something toxic | pet (both) |
| P4 | A $2,000 emergency vet bill | emergency vet bill | an emergency vet bill after their pet ate something toxic | pet (both) |
| P5 | Poison control charges a fee and puts me on hold | pet poison control fee and hold time | pet poison control fees and hold times | pet (both) |
| P6 | I'm scared I'd give the wrong amount in a panic | giving my pet the wrong dose | giving their pet the wrong dose in a panic | pet (both) |

Notes:
- **P4:** "$2,000" was taken out of the question. The profile's number is a hypothesis, and real bills seen so far run from $600 to $2,000 (report 03 summary on Telegram). Putting it in the question would steer the answers.
- **P5:** no fee amount was added to the question. The profile's "$95" is unconfirmed, and the only figure found so far is "$65" (report 02).
- **Why the phrases are hand-placed:** pasting the slot form straight into the course's grammar breaks some questions. That was blocker 4 in report 01. So each of the 156 questions in §5 was written to read naturally. Each one keeps the intent of the course question with the same number.

---

## 5. The 156 ready-to-type questions, grouped by problem

Numbering is `P<problem>.<course question #>`, so every line traces back to §2. One question per line, ready to paste into reddit.com/answers.

### P1: my dog ate something toxic (and there's nothing at home to help)

- P1.1 What makes dog owners feel the most guilty, scared or helpless when their dog eats something toxic and they have nothing at home to help?
- P1.2 What's the most frustrating part of dealing with a dog that ate something toxic when there's nothing at home to help?
- P1.3 What does a "bad night" look like when a dog eats something toxic and the owner has nothing at home to help?
- P1.4 What's something people don't understand about going through your dog eating something toxic when you have nothing at home to help?
- P1.5 What have dog owners tried at home after their dog ate something toxic that didn't work?
- P1.6 What's the biggest waste of money or time dog owners have spent trying to deal with their dog eating something toxic?
- P1.7 What home remedies, methods or advice made things worse after a dog ate something toxic?
- P1.8 Why do dog owners feel like nothing they have at home helps when their dog eats something toxic?
- P1.9 What do most pet first aid products and kits get wrong about a dog eating something toxic?
- P1.10 Why do dog owners believe their dog ate something toxic, and whose fault do they think it was?
- P1.11 Do dog owners think a dog eating something toxic can actually be handled at home, or have they accepted they just have to rush to the vet?
- P1.12 How has their dog eating something toxic changed how owners see themselves as dog owners, or their confidence in handling an emergency?
- P1.13 What words do dog owners use to describe themselves after their dog ate something toxic?
- P1.14 What's the most ridiculous or unhelpful thing someone has said to dog owners after their dog ate something toxic?
- P1.15 What made dog owners finally decide to act, or get prepared, after their dog ate something toxic?
- P1.16 What would having a plan for their dog eating something toxic let owners do or feel again?
- P1.17 What's life like for dog owners after their dog ate something toxic, once they feel prepared for next time?
- P1.18 What's something small but meaningful that changed once dog owners felt ready in case their dog eats something toxic?
- P1.19 What metaphors or analogies do dog owners use when talking about their dog eating something toxic?
- P1.20 What exact phrases, jokes, or slang do dog owners use when describing their dog eating something toxic?
- P1.21 How do dog owners express frustration about their dog eating something toxic -- calm, sarcastic, hopeless, angry, or funny?
- P1.22 What kind of proof or results make dog owners finally believe something works when their dog eats something toxic?
- P1.23 What stories or videos about dogs eating something toxic do owners consider real versus fake?
- P1.24 Who do dog owners trust most when their dog eats something toxic -- their vet, an emergency vet, a pet poison hotline, other owners online, or brands?
- P1.25 What's the moment dog owners realize they can't ignore the risk of their dog eating something toxic anymore?
- P1.26 What emotional state are dog owners in right before they try one last thing after their dog ate something toxic?

### P2: making my dog throw up with peroxide

- P2.1 What makes dog owners feel the most guilty, scared or helpless about making their dog throw up with hydrogen peroxide?
- P2.2 What's the most frustrating part of trying to make a dog throw up with hydrogen peroxide?
- P2.3 What does a "bad night" look like when owners try to make their dog throw up with hydrogen peroxide?
- P2.4 What's something people don't understand about having to decide whether to make your dog throw up with peroxide?
- P2.5 What have dog owners tried at home to make their dog throw up, like hydrogen peroxide, that didn't work?
- P2.6 What's the biggest waste of money or time dog owners have spent trying to make their dog throw up at home with peroxide?
- P2.7 What methods, amounts or advice made things worse when owners tried to make their dog throw up with hydrogen peroxide?
- P2.8 Why do dog owners think nothing works when peroxide won't make their dog throw up?
- P2.9 What do most pet first aid products and kits get wrong about making a dog throw up after it eats something toxic?
- P2.10 Why do dog owners believe they end up having to make their dog throw up at home with peroxide instead of getting help?
- P2.11 Do dog owners think making their dog throw up with peroxide can actually be done safely at home, or have they accepted it's a job for the vet?
- P2.12 How has trying to make their dog throw up with peroxide changed how owners see themselves as dog owners, or their confidence in an emergency?
- P2.13 What words do dog owners use to describe themselves after trying to make their dog throw up with hydrogen peroxide?
- P2.14 What's the most ridiculous or unhelpful thing someone has said to dog owners about making their dog throw up with peroxide?
- P2.15 What made dog owners finally decide to act when they were unsure about making their dog throw up with peroxide?
- P2.16 What would having a clear plan, instead of guessing with hydrogen peroxide, let dog owners do or feel again?
- P2.17 What's life like for dog owners after making their dog throw up with peroxide, once the emergency is over?
- P2.18 What's something small but meaningful that changed once dog owners stopped guessing about making their dog throw up with peroxide?
- P2.19 What metaphors or analogies do dog owners use when talking about making their dog throw up with peroxide?
- P2.20 What exact phrases, jokes, or slang do dog owners use when describing making their dog throw up with hydrogen peroxide?
- P2.21 How do dog owners express frustration about making their dog throw up with peroxide -- calm, sarcastic, hopeless, angry, or funny?
- P2.22 What kind of proof or results make dog owners finally believe something works when they're deciding whether to make their dog throw up with peroxide?
- P2.23 What stories or videos about making a dog throw up with hydrogen peroxide do owners consider real versus fake?
- P2.24 Who do dog owners trust most about making their dog throw up with peroxide -- their vet, an emergency vet, a pet poison hotline, other owners online, or brands?
- P2.25 What's the moment dog owners realize they can't just wait and have to decide whether to make their dog throw up with peroxide?
- P2.26 What emotional state are dog owners in right before they try making their dog throw up with peroxide as one last thing?

### P3: vet closed at night

- P3.1 What makes pet owners feel the most guilty, scared or helpless when their pet eats something toxic and the vet is closed at night?
- P3.2 What's the most frustrating part of dealing with the vet being closed at night when a pet eats something toxic?
- P3.3 What does a "bad night" look like when a pet eats something toxic and the vet is closed?
- P3.4 What's something people don't understand about going through your pet eating something toxic when the vet is closed at night?
- P3.5 What have pet owners tried when their pet ate something toxic and the vet was closed at night that didn't work?
- P3.6 What's the biggest waste of money or time pet owners have spent when their pet ate something toxic after the vet closed?
- P3.7 What home remedies, methods or advice made things worse when a pet ate something toxic and the vet was closed at night?
- P3.8 Why do pet owners feel like nothing they have at home helps when their pet eats something toxic and the vet is closed at night?
- P3.9 What do most pet first aid products and kits get wrong about the hours when the vet is closed?
- P3.10 Why do pet owners believe their pet always seems to eat something toxic after the vet has closed, and whose fault do they think it is?
- P3.11 Do pet owners think a late-night poisoning scare can actually be handled until the vet opens, or have they accepted the emergency vet is the only option?
- P3.12 How has dealing with a pet poisoning at night with the vet closed changed how owners see themselves as pet owners, or their confidence in an emergency?
- P3.13 What words do pet owners use to describe themselves after a night when their pet ate something toxic and the vet was closed?
- P3.14 What's the most ridiculous or unhelpful thing someone has said to pet owners whose vet was closed at night when their pet ate something toxic?
- P3.15 What made pet owners finally decide to act, or get prepared, after their pet ate something toxic when the vet was closed at night?
- P3.16 What would having a plan for when the vet is closed at night let pet owners do or feel again?
- P3.17 What's life like for pet owners after a late-night poisoning scare, once they feel prepared for the vet being closed?
- P3.18 What's something small but meaningful that changed once pet owners felt ready for a poisoning when the vet is closed?
- P3.19 What metaphors or analogies do pet owners use when talking about their pet eating something toxic when the vet is closed at night?
- P3.20 What exact phrases, jokes, or slang do pet owners use when describing a pet poisoning scare at night with the vet closed?
- P3.21 How do pet owners express frustration about the vet being closed at night when their pet eats something toxic -- calm, sarcastic, hopeless, angry, or funny?
- P3.22 What kind of proof or results make pet owners finally believe something works when their pet eats something toxic and the vet is closed at night?
- P3.23 What stories or videos about a pet eating something toxic in the middle of the night do owners consider real versus fake?
- P3.24 Who do pet owners trust most when their pet eats something toxic and the vet is closed at night -- their vet's after-hours line, an emergency vet, a pet poison hotline, other owners online, or brands?
- P3.25 What's the moment pet owners realize they can't wait until their vet opens in the morning after their pet ate something toxic?
- P3.26 What emotional state are pet owners in right before they try one last thing when their pet ate something toxic and the vet is closed at night?

### P4: emergency vet bill

- P4.1 What makes pet owners feel the most guilty, scared or helpless about an emergency vet bill after their pet ate something toxic?
- P4.2 What's the most frustrating part of dealing with an emergency vet bill after a pet ate something toxic?
- P4.3 What does a "bad day" look like when pet owners get hit with an emergency vet bill after their pet ate something toxic?
- P4.4 What's something people don't understand about facing a big emergency vet bill when your pet ate something toxic?
- P4.5 What have pet owners tried to avoid or lower an emergency vet bill after their pet ate something toxic that didn't work?
- P4.6 What's the biggest waste of money or time pet owners have spent at the emergency vet after their pet ate something toxic?
- P4.7 What home remedies, methods or decisions made an emergency vet bill bigger after a pet ate something toxic?
- P4.8 Why do pet owners feel like there's no way around an emergency vet bill when their pet eats something toxic?
- P4.9 What do pet insurance, payment plans and pet first aid kits get wrong about emergency vet bills for poisoning?
- P4.10 Why do pet owners believe they ended up with a huge emergency vet bill after their pet ate something toxic?
- P4.11 Do pet owners think an emergency vet bill for poisoning can actually be avoided, or have they accepted it as part of owning a pet?
- P4.12 How has an emergency vet bill after their pet ate something toxic changed how owners see themselves as pet owners, or their confidence about affording an emergency?
- P4.13 What words do pet owners use to describe themselves after paying an emergency vet bill for something their pet ate?
- P4.14 What's the most ridiculous or unhelpful thing someone has said to pet owners about an emergency vet bill after their pet ate something toxic?
- P4.15 What made pet owners finally decide to act, or get prepared, after an emergency vet bill for something their pet ate?
- P4.16 What would not having to fear an emergency vet bill let pet owners do or feel again?
- P4.17 What's life like for pet owners after an emergency vet bill for poisoning, once they feel prepared for next time?
- P4.18 What's something small but meaningful that changed once pet owners stopped worrying about an emergency vet bill for poisoning?
- P4.19 What metaphors or analogies do pet owners use when talking about an emergency vet bill after their pet ate something toxic?
- P4.20 What exact phrases, jokes, or slang do pet owners use when describing an emergency vet bill for something their pet ate?
- P4.21 How do pet owners express frustration about an emergency vet bill after their pet ate something toxic -- calm, sarcastic, hopeless, angry, or funny?
- P4.22 What kind of proof or results make pet owners finally believe something can save them an emergency vet bill when their pet eats something toxic?
- P4.23 What stories about emergency vet bills for pet poisoning do owners consider real versus fake?
- P4.24 Who do pet owners trust most about whether an emergency vet visit for poisoning is worth the bill -- their vet, an emergency vet, a pet poison hotline, other owners online, or brands?
- P4.25 What's the moment pet owners realize they can't ignore the cost of an emergency vet visit for poisoning anymore?
- P4.26 What emotional state are pet owners in right before they try one last thing to avoid an emergency vet bill after their pet ate something toxic?

### P5: pet poison control fee and hold time

- P5.1 What makes pet owners feel the most guilty, scared or helpless when pet poison control charges a fee and puts them on hold?
- P5.2 What's the most frustrating part of dealing with pet poison control fees and hold times when your pet ate something toxic?
- P5.3 What does a "bad night" look like when pet owners are stuck on hold with pet poison control?
- P5.4 What's something people don't understand about having to pay a pet poison control fee while your pet is in danger?
- P5.5 What have pet owners tried instead of paying for pet poison control that didn't work?
- P5.6 What's the biggest waste of money or time pet owners have spent on pet poison control calls?
- P5.7 What home remedies, methods or advice made things worse while pet owners were waiting on hold with pet poison control?
- P5.8 Why do pet owners feel like nothing helps when pet poison control charges a fee and puts them on hold?
- P5.9 What do most pet poison hotlines and pet first aid kits get wrong for owners whose pet just ate something toxic?
- P5.10 Why do pet owners believe they end up paying a fee and waiting on hold when their pet eats something toxic?
- P5.11 Do pet owners think pet poison control fees and hold times can be avoided, or have they accepted them as the only option?
- P5.12 How has paying a pet poison control fee or waiting on hold changed how owners see themselves as pet owners, or their confidence in an emergency?
- P5.13 What words do pet owners use to describe themselves after paying for a pet poison control call?
- P5.14 What's the most ridiculous or unhelpful thing someone has said to pet owners about pet poison control fees and hold times?
- P5.15 What made pet owners finally decide to act, or get prepared, after paying for a pet poison control call or waiting on hold?
- P5.16 What would having a plan before calling pet poison control let pet owners do or feel again?
- P5.17 What's life like for pet owners after a pet poison control call, once they know what to do next time?
- P5.18 What's something small but meaningful that changed once pet owners had a plan before calling pet poison control?
- P5.19 What metaphors or analogies do pet owners use when talking about pet poison control fees and hold times?
- P5.20 What exact phrases, jokes, or slang do pet owners use when describing pet poison control fees and hold times?
- P5.21 How do pet owners express frustration about pet poison control fees and hold times -- calm, sarcastic, hopeless, angry, or funny?
- P5.22 What kind of proof or results make pet owners finally believe pet poison control, or anything else, is worth paying for when their pet eats something toxic?
- P5.23 What stories about pet poison control fees and hold times do owners consider real versus fake?
- P5.24 Who do pet owners trust most when they don't want to pay for pet poison control -- their vet, an emergency vet, a pet poison hotline, other owners online, or brands?
- P5.25 What's the moment pet owners realize they can't ignore pet poison control fees and hold times anymore?
- P5.26 What emotional state are pet owners in right before they try one last thing while stuck on hold with pet poison control?

### P6: giving my pet the wrong dose (in a panic)

- P6.1 What makes pet owners feel the most guilty, scared or helpless about giving their pet the wrong dose in a panic?
- P6.2 What's the most frustrating part of dealing with working out the right dose for a pet in an emergency?
- P6.3 What does a "bad night" look like when a pet owner panics and isn't sure how much to give their pet?
- P6.4 What's something people don't understand about being scared of giving your pet the wrong dose in an emergency?
- P6.5 What have pet owners tried to get the dose right in a panic that didn't work?
- P6.6 What's the biggest waste of money or time pet owners have spent trying to work out how much to give their pet in an emergency?
- P6.7 What home remedies, methods or advice made things worse when pet owners had to dose their pet in a panic?
- P6.8 Why do pet owners feel like nothing helps them get the dose right when their pet ate something toxic?
- P6.9 What do most pet first aid products and kits get wrong about dosing in an emergency?
- P6.10 Why do pet owners believe they'd give their pet the wrong dose in a panic?
- P6.11 Do pet owners think they can actually dose their pet correctly in an emergency, or have they accepted it's too risky to try at home?
- P6.12 How has the fear of giving their pet the wrong dose changed how owners see themselves as pet owners, or their confidence in an emergency?
- P6.13 What words do pet owners use to describe themselves after giving, or almost giving, their pet the wrong dose?
- P6.14 What's the most ridiculous or unhelpful thing someone has said to pet owners about dosing their pet in an emergency?
- P6.15 What made pet owners finally decide to get prepared so they wouldn't have to guess a dose in a panic?
- P6.16 What would knowing the right dose for their pet ahead of time let owners do or feel again?
- P6.17 What's life like for pet owners once they stop worrying about giving their pet the wrong dose in an emergency?
- P6.18 What's something small but meaningful that changed once pet owners knew how much to give their pet in an emergency?
- P6.19 What metaphors or analogies do pet owners use when talking about dosing their pet in a panic?
- P6.20 What exact phrases, jokes, or slang do pet owners use when describing giving their pet the wrong dose?
- P6.21 How do pet owners express frustration about dosing their pet in an emergency -- calm, sarcastic, hopeless, angry, or funny?
- P6.22 What kind of proof or results make pet owners finally believe they're giving their pet the right dose in an emergency?
- P6.23 What stories or videos about dosing a pet in an emergency do owners consider real versus fake?
- P6.24 Who do pet owners trust most about how much to give their pet in an emergency -- their vet, an emergency vet, a pet poison hotline, other owners online, or brands?
- P6.25 What's the moment pet owners realize they can't ignore the risk of getting the dose wrong in an emergency?
- P6.26 What emotional state are pet owners in right before they try one last thing and give their pet a dose in a panic?

Count check: 6 problems × 26 = **156**, numbered P1.1 to P6.26 with no gaps.

---

## 6. Dog and cat variants

**Which questions are tied to one species**
- **P1 (all 26)** is written for dogs because the registered problem says "My dog". It works for cats by swapping "dog/dogs" for "cat/cats" and "dog owners" for "cat owners". Report 02 has cat buyers (rat poison, lily) and the owner's seed term "cat ate lily", so the cat run is worth doing.
- **P2 (all 26)** is written for dogs because the registered problem is about peroxide, and every peroxide story in our data so far is about dogs. A cat version changes the question's intent slightly, so it is listed separately below.
  - Whether peroxide is used or advised for cats is **not stated here**. That is a fact for the research to find, not something this report claims.
  - A related open contradiction from report 02: the seller says the product is the "only safe at-home option" for cats, and a TikTok comment says "NOT SAFE FOR CATS". Neither is used in any question.
- **P3 to P6** say "pet" and work for both species unchanged. If Reddit Answers returns mostly dog content, rerun the key ones as "cat owners".

**Cat variants (short list, ready to type)**
- C1 (P1.1) What makes cat owners feel the most guilty, scared or helpless when their cat eats something toxic and they have nothing at home to help?
- C2 (P1.5) What have cat owners tried at home after their cat ate something toxic that didn't work?
- C3 (P1.10) Why do cat owners believe their cat ate something toxic, and whose fault do they think it was?
- C4 (P1.24) Who do cat owners trust most when their cat eats something toxic -- their vet, an emergency vet, a pet poison hotline, other owners online, or brands?
- C5 (P1.25) What's the moment cat owners realize they can't ignore the risk of their cat eating something toxic anymore?
- C6 (P2.2) What's the most frustrating part of trying to make a cat throw up at home after it ate something toxic?
- C7 (P2.5) What have cat owners tried at home to make their cat throw up that didn't work?
- C8 (P2.11) Do cat owners think making their cat throw up can actually be done safely at home, or have they accepted it's a job for the vet?
- C9 (P2.24) Who do cat owners trust most about making their cat throw up at home -- their vet, an emergency vet, a pet poison hotline, other owners online, or brands?
- C10 (P6.1) What makes cat owners feel the most guilty, scared or helpless about giving their cat the wrong dose in a panic?

**Dog-only splits for the "pet" problems (use if the results are too mixed)**
- D1 (P3.3) What does a "bad night" look like when a dog eats something toxic and the vet is closed?
- D2 (P4.1) What makes dog owners feel the most guilty, scared or helpless about an emergency vet bill after their dog ate something toxic?
- D3 (P5.2) What's the most frustrating part of dealing with pet poison control fees and hold times when your dog ate something toxic?
- D4 (P6.4) What's something people don't understand about being scared of giving your dog the wrong dose in an emergency, especially a big dog?
  - The big-dog wording comes from report 02 customer lines: "what if my dog is 147lbs 😭" and "My dog is expected to get as big as 120lbs".

The variants are extra. They do not replace any of the 156 and do not count toward the "run all, skip none" total.

---

## 7. Contradictions, gaps and negative evidence to carry into the search step

1. **The registry still says `ADD_ID`.** This step relied on the owner's Telegram decisions, which the playbook says count the same as the playbook. Writing `scaler: Learn E-Commerce Builders (3): Raw Research and Category Context for Copywriting (doc 51)` into the "Raw research lesson" and "Problem question bank" rows would stop future runs from blocking again.
2. **RAW_RESEARCH_METHOD.md is missing from the SavePet repo** (404). It exists only in the main repo.
3. **The 26 vs 27 question count is settled.** There are 26, and the "27" was a setup error, as the owner confirmed.
4. **Numbers kept out of the questions** so they don't steer the answers: "$2,000" (P4) and "$95" (P5). Both are profile hypotheses. The only real figures so far are the $65 hotline fee and bills of $600 to $2,000.
5. **Negative evidence to expect in answers.** Report 02 already holds vet-staff warnings against home peroxide or charcoal without a vet or poison helpline: "never give this without consulting a vet first!" (2,533 likes). P2.11, P1.11, P2.24 and P1.24 will probably bring up more of this. It must be kept verbatim as negative evidence, not filtered out.
6. **Wording that could bias the answers.** Q16–18 ("having a plan", "felt ready") lean toward preparedness. That is the closest emergency equivalent of the course's "fixing/solving". It names no product and makes no claim. If answers come back thin, a neutral rerun ("…after the emergency was over") would be an option.

---

## 8. Ideas for the next step (not tasks; nothing was created, assigned or scheduled)

- **Run all 156 (§5), skip none**, per the lesson. Do the cat variants C1–C10 after that if budget remains. The Telegram cap the owner approved for the search step is $6.
- **Run P3 and P5 first.** They are the thin problems in report 02. P1, P2, P4 and P6 already have category coverage, but per the method a problem never run on Reddit still runs all its bank questions.
- **Reddit Answers only gives leads.** Keep only lines from the cited threads and comments, with permalinks and dates. Then search the owner's subreddits directly (AskVet, dogs, DogAdvice, puppy101, cats, CatAdvice, Pets) with the short phrases in §4 plus the seed terms (dog ate chocolate / grapes / rat poison / ibuprofen, cat ate lily, activated charcoal for dogs).
- **Actor choice and run hygiene.** Use one of the listed Reddit Answers actors in report 01 §6 (untested). Tag every run `job: raw-research`, log runId, datasetId, results bought, results kept and cost, and check `list_apify_runs` before any rerun.
- **Store this bank where future runs can fetch it.** Save it as its own Supermemory document and register the ID in the playbook's "Problem question bank" row, so the next run fetches it instead of re-deriving it.

## 9. Sources unavailable or failed

- **ClickUp:** not configured, and not used (no tasks by policy).
- **`00_rules_and_process/RAW_RESEARCH_METHOD.md` in `exobvious/savepet-research`:** 404. Read from the main repo instead.
- **Supermemory:** no stored course prompt or tailored bank. The first `search_memory` call failed on a wrong argument name (my error), and the retry worked.
- **Vantage and Apify:** not used on purpose. This was a writing step with zero spend.

## 10. Outputs of this run

- This report is the only file written. It holds the verbatim bank, the template, the phrases, the 156 questions and the variants.
- Apify spend: **$0.00**.
- `course_v2/COVERAGE_V2.md` block 1 stays unticked until the search step adds real quotes.
