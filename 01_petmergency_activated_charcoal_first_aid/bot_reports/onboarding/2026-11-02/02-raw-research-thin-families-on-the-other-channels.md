# PetMergency Activated Charcoal First Aid Kit (SavePet): EB raw research step two, other channels for the thin families

- **Run:** onboarding / 02-raw-research-thin-families-on-the-other-channels, 2026-11-02 (UTC), cloud research agent, Apify job tag `raw-research`
- **Product folder:** `01_petmergency_activated_charcoal_first_aid/` in `exobvious/savepet-research`
- **Status: PARTIAL, and honestly labeled.**
  - Amazon, YouTube and TikTok were each pulled once, aimed at the gaps, and kept.
  - Facebook groups were bought (30 posts) but **not read** before the run had to stop.
  - Quora returned question titles and one owner story, but **no answer text**.
  - The Reddit Answers lane (step one) **still has not run**, so this step ran *before* Reddit. That is out of the course order: Reddit comes first.
- **Spend:** about **$0.70 to $0.75** on Apify (log in §6).
- **Files written:** this report only.
  - The system rule for this run is to publish exactly one file. So the category document's raw quote bank is started **inside this report** (§4), formatted as the `## Added 2026-11-02` section that `RAW_RESEARCH_METHOD.md` says goes into `EB_CATEGORY_CONTEXT_<category>_v2.md`.
  - Copy it into that file once the filename is settled.

---

## 1. What was read first

| # | Source | Result |
|---|---|---|
| 1 | `gateway_status` | scaler, vantage, apify and supermemory were OK. **clickup: false** (and no tasks are created by policy). Apify today before this run: $1.49, with no daily stop. |
| 2 | `get_playbook`: `UNIFIED_PLAYBOOK.md` (sha 02e8ca8) | **Every prompt registry row still says `ADD_ID`.** This includes "Raw research lesson" and "Problem question bank". |
| 3 | `PRODUCT_DECISION.md` (3f08d1e), `product_truth.md` (a2a4a93) | Six buyer problems. Competitors: "none given yet". Page claims, "Made in USA" and "third-party tested" are seller claims. The avatar-profile numbers are hypotheses. The page's dose guidance contradicts itself. |
| 4 | `RAW_RESEARCH_METHOD.md` (f11ed6d) | Step 4: "Other channels only for thin families, in course order (Amazon, YouTube, TikTok, Facebook, Quora), each aimed at the gap." Step 5: small pages, stop at saturation. Step 6: log every pull. Step 7: end with the coverage table. |
| 5 | `AGENTS.md`, `NEVER_REPEAT_MISTAKES.md` | Rule 2: a stage with no ID is reported missing, not improvised. Rule 4: two independent reports before an angle enters the bank. Never-repeat is empty. |
| 6 | Step one report `01-raw-research-reddit-answers-bank.md` (ec5bca1) | BLOCKED. Zero questions run, $0 spent, no category document. Coverage table: **all 7 families thin, 0 quotes, for all 6 problems.** |
| 7 | `telegram_log/2026-11-02.md` | Brand confirmed as **SavePet** (16:40). At 17:06 the assistant said the other-channels step "has tried once and failed with 'Request not allowed'". The owner has **not yet replied "go"** to the four Reddit approvals. |
| 8 | Supermemory `search_memory` (raw research prompt, SavePet) | **No matching memories.** No prompt has been registered since step one. |
| 9 | Scaler `get_doc(51)`: "Learn E-Commerce Builders (3): Raw Research and Category Context" | Read again for its other-channel guidance (details below). |
| 10 | `listening/SOURCES.md` | Search terms and subreddits from the owner's profile. These were used as search seeds. |
| 11 | `list_apify_runs` (8 h) | No earlier other-channel pull existed to reuse. The 23 untagged runs are the Facebook Ad Library actor, not SavePet. |

The lesson's guidance on other channels (Scaler doc 51), which this run followed:

- **Amazon:** search the product type and read the reviews. The lesson says reviews show "the pain points people are having / why they bought the product / what they are trying to fix", and that negative reviews have value too.
- **YouTube:** use the transcript and the comments.
- **TikTok, FB Groups, Quora:** paste "the exact comments, quotes, and stories under RAW RESEARCH". The lesson says it is "a data dump, not a polished doc."

**Why I ran the channels despite `ADD_ID`.** Step one stopped because running the Reddit question bank needed an unregistered, untailored course prompt, and writing that prompt myself would have been forbidden reconstruction. Step two needs no prompt. It is searching and keeping verbatim lines, as `RAW_RESEARCH_METHOD.md` (a repo rule, not a course prompt) and the lesson text describe. No course prompt was run, rewritten or substituted. **The "Raw research lesson" registry row is still `ADD_ID`, and that is reported as missing.** If the owner wants step two held until the registry is filled, this run's kept quotes stay valid as raw data, but the run should be treated as provisional.

**Order caveat.** Every family was thin only because Reddit never ran. Under the method, the other channels fill gaps *after* Reddit. Reddit will probably change this table once it runs.

## 2. Coverage table at the start (from step one)

The table was the same for all six problems: every family **thin, 0 quotes**. No category document exists.

## 3. What each channel returned (searches aimed at the gaps)

| Channel | Searches / targets | Result |
|---|---|---|
| **Amazon** | Product search "activated charcoal for dogs". Reviews pulled for the three listings with the most reviews (helpful sort), then a second page aimed at critical reviews. | Page 1 added many new lines, so page 2 (critical) was pulled. It added new negative evidence. Not saturated, but held at 2 pages for budget. |
| **YouTube** | Video search: "my dog ate chocolate what to do", "hydrogen peroxide make dog vomit", "dog poisoning emergency vet story" (15 videos). Comments pulled only from 4 videos directly about the owner's problem. Bondi Vet entertainment compilations were skipped on purpose. | Rich, especially emotional and failed-attempt lines. |
| **TikTok** | Keyword search: "dog ate chocolate", "activated charcoal for dogs", "emergency vet bill dog". **All 20 results came from the first two keywords' feed and are about charcoal products, mostly PawMergency affiliate posts.** Comments pulled on the 5 most-viewed videos. | Strong trust/proof and negative evidence, plus price objections. Captions are creator/affiliate content, so they count as `competitor_claim`, not customer voice. |
| **Facebook** | No group URLs exist in `SOURCES.md` ("none yet"), so I ran a keyword search of public group posts: "dog ate chocolate emergency vet", "activated charcoal dog poison". | **30 posts bought ($0.15), NOT READ.** The run stopped first. The dataset is preserved for the next run (§6). Nothing from Facebook is in the quote bank. |
| **Quora** | Search: "my dog ate chocolate what should I do", "should I make my dog throw up with hydrogen peroxide", "emergency vet bill dog poisoning". Then a direct pull of the question with 26 answers. | 7 question records, with titles only. The peroxide query returned nothing. The direct question pull returned 1 record and no answers. A plain page fetch of that question **failed** (exit 1). One long owner story was kept. **Quora answers: MISSING.** |

## 4. Raw quote bank (start of the category document)

> Paste this as `## Added 2026-11-02: other channels (Amazon, YouTube, TikTok, Quora)` into `EB_CATEGORY_CONTEXT_<category>_v2.md` once that filename is chosen. Quotes are verbatim, typos included.
>
> **Source class key:**
> - `customer_report` = an owner speaking about their own pet.
> - `pro_opinion` = a commenter who self-identifies as vet staff. This is unverified and recorded as negative evidence.
> - `competitor_claim` = seller or affiliate content.
>
> Amazon review links: `https://www.amazon.com/gp/customer-reviews/<id>`. YouTube comments: video ID plus comment ID. TikTok comments: video URL plus comment ID.

### 4.1 Emotional experience

- "IM LITTERLY CRYING BECAUSE MY DOG ATE CHOCOLATE AND I HEARED THAT ITS POISONS BUT SHE ONLY ATE A SMALL AMOUNT BUT IM STILL WRORIED". YouTube eKRzJ3sxUlc, cid Ugy1z0YTs9E-3-Y5pxt4AaABAg, @daianazazueta2768, about 6 years ago. customer_report
- "my 3 puppies accidentally ate a choco butternut cake earlier I'm scared and crying because I don't have money to take them to the vet and they are kinda pale.. :(". YouTube eKRzJ3sxUlc, cid UgzoRXrLkASnluf7gjx4AaABAg, @qtxvall6825. customer_report
- "i am balling my eyes out and frantically searching for information. my dog ate chocolate and i think he's going to get ill 😭😭😭". YouTube Mtx6oLVVJ7k, cid Ugy-A6F81CjZUsP0w354AaABAg, @cryinqinclouds24. customer_report
- "My dog ate a half eaten box of chocolate chip cookies and I'm shaking and I looking up videos on what to do". YouTube eKRzJ3sxUlc, cid UgyayF849co2HRGmcjB4AaABAg, @Fty-yi8lo. customer_report
- "he's asleep now, and i think he'll be alright but damn i never looked up a 24 hour vet in my area so quickly. i was so worried lolol". YouTube eKRzJ3sxUlc, cid UgySTruZkUmlSHXiqml4AaABAg, @delusional767. customer_report
- "My mid sized dog had a lick of chocolate ice cream today. I don't think it was enough to hurt her at all, but I am a bit paranoid and I'm freaking out." YouTube eKRzJ3sxUlc, cid UgxHbpueKezrNEJoFLx4AaABAg. customer_report
- "My dog just got into my pills of risperidone and im freaking out its literally 12:00am in the morning and". YouTube v-k4ezLEkLU, cid Ugx6W1QeNc8_-G-nHql4AaABAg, @CarlosVeleska. customer_report **(P3: vet closed at night)**
- "I place the most pertinent info into the notes app on my phone so that in an emergency (when my anxiety turns my brain to mush) I don't have to fumble around for it." YouTube xG1nLBTzPDo, cid UgxQ3qhsMdCkh75Ol8B4AaABAg, @GabrieleMerkel. customer_report **(P6: panic)**
- "It was so scary. I'm with them almost every minute, but they still get into everything at that age." YouTube xG1nLBTzPDo, cid Ugwe3IGhMDsKmksLJqV4AaABAg, @munster3311. customer_report
- "Luckily I caught him with it before he got through the wrapper but I was so scared…" TikTok jeremysfinds/7541048399605353741, cid 7541428598461383454, @roman.buggy.and.friends. customer_report

### 4.2 Failed attempts and frustration

- "Did 2 tablespoons and she never puked". YouTube v-k4ezLEkLU, cid UgySWxyk1G6jWq9V-gp4AaABAg, @wearywanderer7018. customer_report **(P2: peroxide)**
- "I immedtiately tried to get her to vomit with peroxide but I didn´t suceed, ofcourse I called the vet but it would have taken a great time to get there for me so I rushed to get some activated charcoal". YouTube xG1nLBTzPDo, cid UgwVKn1Piu2LdusOJvx4AaABAg, @Unfounduser09. customer_report **(P1, P2)**
- "My little bischon ate an entire package of exlax. We gave him hydrogen peroxide and nothing happened." YouTube xG1nLBTzPDo, cid UgzwhrKP57WzxArILkd4AaABAg. customer_report **(P2)**
- "Gave correct amount to my puppy after he chewed on some wood and was eating the splinters. But he never threw up". Amazon 1★ "Doesn't Work!", R22OQU9696DWL7, B0FXBQSFJP (PawMergency), 2025-10-24, verified. customer_report. *Note: the buyer expected charcoal to make the dog vomit. That is a misunderstanding of how the product works.*
- "the vets I called can't legally give advice so I watched this video and he threw up in about 4 minutes." YouTube v-k4ezLEkLU, cid UgzWLMdzWv_UHGrXhVt4AaABAg, @erikathompson1862. customer_report **(P3/P5: no help on the phone)**
- "We used Peroxide/called the poison control line ($65) /went to the 24hr Emergency Vet… by the time we got to the Vet (30min drive) she had already vomited allot...and they didn't do much". YouTube Mtx6oLVVJ7k, cid UgxXCSUapCNwSmim4sZ4AaABAg, @KceeKit. customer_report **(P5: the only poison-control fee figure found is $65, not the profile's $95)**
- "my mom won't let me go to the vet and take her unless she starts vomiting or something like that and she is a little dog!" YouTube eKRzJ3sxUlc, cid UgzRUtH4JE2DRHrPvqF4AaABAg, @sudaxm. customer_report
- "the ER Hospital said I could bring them to have the tummy pumped but at that point...too late, and to bring them in if they exhibited further symptoms. They told me to hydrate, hydrate, hydrate." YouTube xG1nLBTzPDo, cid Ugwe3IGhMDsKmksLJqV4AaABAg, @munster3311. customer_report
- "Just make sure your peroxide isn't too old." YouTube xG1nLBTzPDo, cid UgyQwgQokpnunmNbhi54AaABAg, @chiweenieheros. customer_report

### 4.3 Beliefs and self-image

- "A huge mistake and lesson learned for the human, but also having this for such human mistakes was a lifesaver." Amazon 5★, R1PJXSAJA58WNE, B0FXBQSFJP, 2026-05-27, verified. customer_report (owner guilt)
- "I will always keep this on hand now because dogs can be resourceful and humans can make mistakes." Amazon 5★, R98C0V79UQ94X, B0FNY9J7ZT (PetVet Medic), 2026-06-11, verified. customer_report
- "I was a complete numb knuckle and left grapes on the kitchen table, got distracted in another room." YouTube v-k4ezLEkLU, cid Ugxf3qrD8WynIcBDwbB4AaABAg, @aarontcagle. customer_report
- Counter-belief (the "it won't happen / chocolate is a myth" objection): "We gave them to her, no one ever heard chocolate was dangerous to dogs…she lived to be 15." YouTube eKRzJ3sxUlc, cid UgwdRu_7DJTVdjWUO9F4AaABAg, @Pegily. Also: "That told me either the chocolate and dogs is a myth or the chocolate cake was fake". cid UgxrkDqCW231F_CpI-V4AaABAg, @JSFGuy. Also: "they ate everything including chocolate and avocados and survived". cid Ugzrp4Nasc_nWOC3kMR4AaABAg. customer_report
- "i mean don't get me wrong it's nice to be safer than sorry but don't leave ur stuff out lmao then u won't have this issue". TikTok jeremysfinds, cid 7546489362982404878. customer_report (objection)
- "ya i don't trust any pet products that come from the internet and not the vet🥹". TikTok frugal__living/7493593664329944350, cid 7493975684151837486, 78 likes. customer_report (matches the profile objection "should I buy this online?")

### 4.4 Transformation and hope

- "I immediately grabbed the Pawmergency from my purse and gave it to him… he didn't end up having any bad reactions to it and we avoided a trip to the vet!" Amazon 5★, RU0M4MDBVULVD, B0FXBQSFJP, 2026-09-21, verified. customer_report
- "unlike the first time, he showed absolutely no symptoms at all from the chocolate poisoning or the activated charcoal… saved us from what could've been an extremely high vet bill." Amazon 5★, R98C0V79UQ94X, B0FNY9J7ZT. customer_report **(P4)**
- "I gave her the activated charcoal and rushed her to the emergency veterinary hospital where the treatment was completed and she was released the next morning." Amazon 5★, RIFGTSSJTXYV1, B0FNY9J7ZT, a self-described "retired veterinarian technician and RN". customer_report (charcoal *plus* the ER, not instead of it)
- "I saved my sisters schnauzer this way… Full blown seizure to fine". TikTok muonline_pc/7514895346850336031, cid 7524875251797820191. customer_report
- "he's a big 100lbs rottie/dobie and i gave him 2tbsp and he threw up 5 min later… I'm so thankful for this video." YouTube v-k4ezLEkLU, cid UgwEOdoUpi5i2IPUXrN4AaABAg. customer_report (P2: peroxide success)
- "This has honestly been a lifesaver and I will keep purchasing this product because it does its job and saves me from extra vet costs!" Amazon 5★, R3F533BNXABN7N, B0CN6JLXLS (powder). customer_report

### 4.5 Language, voice and expression (phrases to reuse verbatim)

- "a puppy who was able to **inhale chocolate**… where their human looked away for two seconds". R1PJXSAJA58WNE
- "Must have if you have Pets. **kind of an EpiPen for your curious ones**". RNEFT86O01SYV (B0FXBQSFJP)
- "My puppy eats everything!" R25Z1PPLON1W1W · "my girl likes to eat things she finds" RYTH1RPGHEUXQ · "Our big boy will eat just about anything" RV6VX2KD4A8PS
- "**Hope I never have to use it.**" R2XVLZVD62VWS5 · "one of those products you hope you never need" R1A9UDWP5L9AS8 · "Haven't Needed It—But So Glad We Have It" RV6VX2KD4A8PS
- "Better safe than sorry." R2B4Q34V2L7YAV · "Peace of mind" (titles of R25Z1PPLON1W1W, RYTH1RPGHEUXQ)
- "furbabies" (RIFGTSSJTXYV1, R3V0WAMC78GXMM) · "precious baby" / "babies" (R1PJXSAJA58WNE, R2L1FFS3VVEJ4O)
- "freaking out", "shaking", "balling my eyes out", "frantically searching": YouTube comments above.
- Affiliate phrasing, *not customer voice* (competitor_claim): "If your dog eats like they have a death wish" (@tastefullyextra); "what if you could prevent your pups unaliving" (@frugal__living); "Better to have it and not need it then need it and not have it" (@dailytt.shops).

### 4.6 Trust and proof (includes the main negative evidence)

- "as a vet assistant never give this without consulting a vet first! charcoal can cause dangerous electrolyte imbalances!" TikTok melissa_fergus/7489845283237465375, cid 7504847248652600095, **2,533 likes**. pro_opinion
- "NOT SAFE FOR CATS". Same video, cid 7504855570481988398, **575 likes**. customer_report/opinion. **This contradicts the seller's "only safe at-home option" for cats claim.**
- "vet professional here, please consult a veterinarian before administering! in some cases you can ABSOLUTELY cause more harm than good." cid 7505153901018006315, 320 likes. pro_opinion
- "PLEASE DO NOT GIVE YOUR PETS PEROXIDE! Take them to a vet where we can induce vomiting safely… please do not give activated charcoal without FIRST REACHING OUT TO PET POISON HELPLINE!!!" TikTok mm336777/7496873206314208554, cid 7505072267107255071, 92 likes. pro_opinion **(P2 negative evidence)**
- "do not give unless instructed by a vet or poison control". cid 7501794719468471082, 65 likes. Also: "Some things specifically tell you NOT TO INDUCE VOMITING because it's more dangerous." cid 7505107364363715371, 39 likes.
- "My vet said please don't use that she could aspirate the charcoal in her lungs and get pneumonia so I returned it." Amazon 1★ "Returned", RXIWHMIQJDOQL, B0FXBQSFJP, 2026-08-26, verified. customer_report
- "So weird my dog ate chocolate and the emergency vet clinic said inducing vomiting at home or giving charcoal at home weren't recommended. 🙄" YouTube Mtx6oLVVJ7k, cid UgzG20pNmRcyo4zF1nJ4AaABAg. customer_report
- "There is no manufacturing date on the charcoal on any of the five… it's good for two years what I received for $100 is in fact only good for one year… we could be buying old charcoal that will in fact do nothing". Amazon 1★, R2L1FFS3VVEJ4O, B0FXBQSFJP, 2026-08-02, verified. customer_report (shelf-life trust; the SavePet page's shelf-life answer is also broken, per Telegram 15:05)
- "Another creator was advertising this also, then in the comments said she no longer supports this product or company after learning some disturbing info". TikTok melissa_fergus, cid 7504768888234017566. Hearsay, watch-only.
- "They didn't use charcoal they used something else stop trying to falsely promote this". TikTok muonline_pc, cid 7603145706401350430. customer_report (pushback on affiliate content that stitches a vet's video)
- Proof that worked for buyers: "Not this specific brand, but a product recommended by veterinarians who are also close friends." RNEFT86O01SYV. "A friend of mine suggested keeping this on hand". R3V0WAMC78GXMM. A self-described retired vet tech/RN endorsing PetVet Medic. RIFGTSSJTXYV1.

### 4.7 Catalyst moments / buying psychology

- "When your stressed, the less time you spend trying to figure out how large a dose, could be a life saver." Amazon 5★, R3V8DHN3ZZHS1Z, B0FXBQSFJP, 2026-10-26, verified. customer_report **(P6: dosing in a panic)**
- "One tube covers 30 lbs in weight, so be sure to purchase enough to cover the weight of all babies in your home". R1PJXSAJA58WNE. Also "what if my dog is 147lbs 😭" (TikTok cid 7504989224321188651) and "Do they make it for bigger dogs? My dog is expected to get as big as 120lbs" (cid 7505254368082969374). **(P6, and a bundle/upsell signal)**
- "My dog ate a whole box of dark chocolate. This would've saved me 2 grand 😅". TikTok jeremysfinds, cid 7572279429965300493. customer_report **(P4: the $2,000 bill, one independent report)**
- "trust me if the vet administrator activated charcoal it will Cost $$$$." Amazon 5★, RP39F77QYNIHQ, B0FNY9J7ZT. customer_report (P4)
- "my cat got into some rat poison so prime delivery was same day". Amazon 5★, R39B5Y92LBQFYO, B0CN6JLXLS. Bought *during* the emergency.
- "Good to have on hand in case dog picks up another poison toad again!" R3ULWZZTQKMD4U. Also "we've got lots of toads… (In Florida and the every day rain brings them out.)" R2B4Q34V2L7YAV. A regional trigger.
- "Our super fast Shih Tzu got ahold of my husband's Warfarin pill… A friend of mine suggested keeping this on hand". R3V0WAMC78GXMM. A near-miss turns into a purchase.
- **Price objection** (the profile's "$40 for something I may never use"):
  - "why don't they make more affordable so everyone can access it" (TikTok mm336777, cid 7500685011911672607)
  - "Why isn't this cheaper??" (cid 7503171397475222318)
  - "You can buy activated charcoal, much cheaper" (TikTok muonline_pc, cid 7524865301285421854, 106 likes)
  - "don't buy this overpriced product bruh they be charging 60$ for a 10 dollar product" (cid 7566770548093895437)
  - Positive side: "wouldn't have bought if price was outrageous" (R2B4Q34V2L7YAV); "It's expensive but 100% worth the emergency use" (R1PJXSAJA58WNE)
- "*adds to cart*". TikTok jeremysfinds, cid 7541470680819204894.

### 4.8 Owner story (Quora, long-form, P3 + P4)

"Because it was a holiday we couldn't find any regular vets open… we were asked to make a deposit… A student staying at my place from India offered his credit card for a deposit of $ 1000… The outcome ( at 4:00 a.m. ) was that Pther may have been poisoned." From https://mariatrudelsspace.quora.com/This-past-July-01-holiday-I-was-dog-sitting-my-brother-his-wife-s-dog-while-they-were-in-Ontario-We-have-dog-sat-thi (Quora Space post). customer_report.

Quora question titles found, which are search language only: "What should I do if my dog ate chocolate and the vet isn't an option?" (26 answers, https://www.quora.com/What-should-I-do-if-my-dog-ate-chocolate-and-the-vet-isnt-an-option); "What should I do if my dog ate chocolate and is vomiting?" (17 answers).

## 5. Market facts surfaced (competitor_claim / listing data, not product proof)

| Listing | ASIN | Reviews · stars | Price seen | Note |
|---|---|---|---|---|
| **PawMergency – Activated Charcoal First Aid Kit** | B0FXBQSFJP | 687 · 4.7 | $36.99 | **Same name as the "PawMergency" typo on the SavePet page.** A review says "One tube covers 30 lbs", which matches SavePet's "under 30 lbs is one tube". **Hypothesis:** same white-label product or a direct copy. Not verified. |
| PawMergency 2-pack | B0FYL6M55D | (shared 687) | $62.98 | Bundle price reference. A 1★ reviewer paid "$100" for five. |
| PetVet Medic Activated Charcoal (beef-flavored, "Veterinarian-Developed, Made in USA", 60 mL) | B0FNY9J7ZT | 304 · 4.7 | $24.99 | Seller claims. |
| Activated Charcoal powder 3.53 oz | B0CN6JLXLS | 645 · 4.7 | $15.59 | Low-price alternative. |
| Others: 30 ml tube $9.99 (B0H2VH3RQP), 60 mL gel $12.87 (B0GJ5Z1X68), 2 tubes $16.60 (B0H1KR9Z9J) | | 2–56 reviews | $9–18 | Price floor for the "$10 product" objection. |

- **TikTok Shop:** PawMergency affiliate content carries the handles **@PetlyPet** and **@Vetanica**. The top posts have 1.27M views (@melissa_fergus), 1.10M (@mm336777), 640K (@muonline_pc, a stitch of @RuralVetServices), 535K (@frugal__living) and 426K (@jeremysfinds).
- **Candidates for "Competitors" in `PRODUCT_DECISION.md` (owner's call):** PawMergency (Petly Pet / Vetanica?) and PetVet Medic.
- **SavePet sits at $39.95, above every Amazon listing seen.**

## 6. Pull log

| # | Actor | runId | datasetId | Bought | Kept | Cost (reported) |
|---|---|---|---|---|---|---|
| 1 | apify/web-fetch (Amazon search page) | I4oWgcaRGs0ePJJ2P | DLVlocP89vwEspnVP | 1 (HTTP 503) | 0 | $0.00005 |
| 2 | igolaizola/amazon-search | tg9BRqLBUcfmzERxc | g6ZuVPF3NdaB4vCR8 | 0, FAILED (exit 1) | 0 | $0.0005 |
| 3 | junglee/Amazon-crawler (search) | bmIlKTBEAo5ZMXdAH | iYklexFOx41Uh6Rx7 | 10 products | 10 (as listing data) | $0 at poll, about $0.04 at list price |
| 4 | web_wanderer/amazon-reviews-extractor | 8IceDchBqmsRRJO1w | htsMENr24dwjsyXjo | 0 (succeeded, empty) | 0 | $0.00002 |
| 5 | jdtpnjtp/amazon-reviews | nJfZZC2Y1uuSypH3B | gyJgxGDdk31YhNwkI | 0, FAILED | 0 | $0 |
| 6 | junglee/amazon-reviews-scraper (helpful) | zpV1HpHWN7f2FdBap | Da2ivMrrTuvpdIR5n | 36 reviews | 22 | $0.18 |
| 7 | junglee/amazon-reviews-scraper (critical) | CYkmzt09mXXREEpLR | cxM8wT7E2E0nPOP8e | 8 reviews | 3 | $0.04 |
| 8 | streamers/youtube-scraper (search) | pKploE4hWEaZ2vVFX | eZYd73zYQIuOpndsg | 15 videos | 4 chosen for comments | $0.045 |
| 9 | streamers/youtube-comments-scraper | 51s7iPvR1eeqkygIW | DNJAqKFgeHTwWtV0p | 80 comments | 26 | $0.12 |
| 10 | apidojo/tiktok-scraper (search) | YSwu7LfFtNqKXRObj | VBkj0hMIJsDIP0xXE | 20 posts | 5 chosen for comments, plus captions as competitor_claim | $0.006 |
| 11 | clockworks/tiktok-comments-scraper | UdBUPRzpCDjWcFiWv | yOhyIAyBMiC8IQ0oz | 100 comments | 24 | $0.10 |
| 12 | fatihtahta/quora-scraper (search) | L9SinbOHUq1tdpAeZ | NozQPl1l6r9O7cnZw | 7 questions | 1 story and 2 titles | $0 at poll, about $0.007 at list price |
| 13 | apify/web-fetch (Quora question) | wndUeDqw6EcmKVFKP | 3Hohr4tAFKkBIFXrl | 0, FAILED | 0 | $0.00005 |
| 14 | lofomachines/facebook-groups-posts-search-scraper | mciIc7HradgHcKWf8 | uQBfIcoXY0boLKb5r | 30 posts | **not read (0)** | $0.1497 |
| 15 | fatihtahta/quora-scraper (question URL) | vuPNVMPy26UBt6Qoy | Tb3jlmETV0oZZUPzd | 1 record, no answers | 0 | $0.00099 |

- **Total reported:** about $0.64.
- **With list-price estimates for the two runs that showed $0 at poll:** about $0.69.
- **Plus validation and cap rejections:** no charge.

Two config notes for future runs:
- The YouTube comments actor needs a cap of at least $0.50, and the Quora actor at least $1.00 (runs below that are rejected before charging).
- **Facebook dataset `uQBfIcoXY0boLKb5r` is paid for.** The next run must read it with `get-dataset-items` and not buy it again.

## 7. Coverage table at the end

Counts are distinct people with kept quotes, across the category (all six problems pooled). A per-problem view follows.

| Family | Status | Quotes (different people) | Main channel |
|---|---|---|---|
| Emotional experience | **covered** | 10 | YouTube |
| Failed attempts and frustration | **covered** | 9 | YouTube, Amazon |
| Beliefs and self-image | **covered** | 8 | Amazon, YouTube, TikTok |
| Transformation and hope | **covered** | 6 | Amazon, TikTok |
| Language, voice and expression | **covered** | 8+ (customer only) | Amazon |
| Trust and proof | **covered** (heavy negative evidence) | 11 | TikTok, Amazon |
| Catalyst / buying psychology | **covered** | 12 | Amazon, TikTok |

Per buyer problem:

| Problem | Status | Why |
|---|---|---|
| P1 "My dog ate something toxic and I have nothing at home to help" | covered | Many owner reports. |
| P2 "Should I make him throw up with peroxide?" | covered | Both sides: success stories, failures (3) and vet warnings. |
| P3 "The vet is closed at night" | **thin** | 3 indirect reports: 12:00am, the 24-hour vet search, and the holiday ER story. Needs Reddit. |
| P4 "A $2,000 emergency vet bill" | covered | "saved me 2 grand", the $1000 deposit, "$$$$", "extremely high vet bill", "don't have money to take them". |
| P5 "Poison control charges a fee and puts me on hold" | **thin** | 1 report ($65), plus "vets I called can't legally give advice". The profile's "$95 hotline fee" is **unconfirmed**. Not yet searched as its own query. |
| P6 "I'm scared I'd give the wrong amount in a panic" | covered | Dose-in-stress, big-dog weight questions, the 30 lb per tube comment, the brain-mush comment. |

Channels still open:

- **Facebook:** bought, unread. MISSING until read.
- **Quora answers:** MISSING. Searches tried: the 3 queries above, a direct question pull, and a page fetch (failed).
- **Reddit (step one):** still not run.

**Caution:** "covered" here means three or more quotes from different people. It is **not** the AGENTS rule-4 angle bar. Each angle still needs two independent reports for its specific claim.

## 8. Contradictions and negative evidence (for the owner)

1. **Cats.** The seller's "only safe at-home option" for cats is contradicted by "NOT SAFE FOR CATS" (575 likes). There is also positive owner use on cats with powder (RQ0W5M01QLWPB, R28AQ4RE4PJ6RB, R39B5Y92LBQFYO). Unresolved. Do not use the cat claim.
2. **Home use vs. "call a vet first".** At least 6 self-described vet staff or owners say: don't give charcoal or peroxide without a vet or the poison helpline. Risks named: electrolyte imbalance, aspiration pneumonia, and that vomiting is wrong for some poisons. Ads framing charcoal as *instead of* the vet are likely to draw this pushback. Owner successes mostly describe charcoal **plus** a vet call or ER visit.
3. **Peroxide works for some, not for others.** It vomited in 2–10 minutes in several reports and "never puked" in others. Vet staff say not to use it at all.
4. **Shelf life.** An Amazon 1★ says the "two years" claim isn't backed by any manufacturing date. The SavePet page's shelf-life answer is shipping text (Telegram 15:05). This is a trust gap.
5. **Expectation mismatch.** One buyer expected charcoal to cause vomiting (R22OQU9696DWL7). Another credits charcoal for making the dog vomit (RL2ZLF3636VYI, R34PUPDOVEYAUK). Mechanism claims need care.
6. **PawMergency name overlap.** It is possibly the same goods as SavePet, sold on Amazon for less ($36.99) with 687 reviews. That makes price and differentiation a real risk. **Hypothesis to verify with the supplier ("My Vereli").**
7. **Process.** Step two ran before step one (Reddit), and the registry is still `ADD_ID` (see §1).

## 9. Ideas for the owner (not tasks; nothing was assigned or scheduled)

- Tell me whether to keep or hold this step's provisional status while the "Raw research lesson" row is still `ADD_ID`. Give the four Reddit "go"s from Telegram 17:06 so step one can actually run. It should hit P3 and P5 hardest.
- Next run, read Facebook dataset `uQBfIcoXY0boLKb5r` (already paid for). Then decide whether Facebook needs more pages.
- Add PawMergency (B0FXBQSFJP) and PetVet Medic (B0FNY9J7ZT) to Competitors. Ask the supplier whether SavePet = PawMergency stock.
- Run P5 as its own search ("poison control fee", "ASPCA poison control charge", "pet poison helpline hold") on Reddit first. Treat the $95 figure as unproven: the only real number so far is $65.
- Choose the category document filename (for example `EB_CATEGORY_CONTEXT_pet_poisoning_first_aid_v2.md`) and paste §4 in as its first `## Added` section.
- **Angle signals worth watching (each still needs 2 independent reports per claim):**
  - "an EpiPen for your curious ones"
  - "the less time you spend trying to figure out how large a dose"
  - "it'd have saved me 2 grand"
  - owner guilt ("their human looked away for two seconds")
  - Florida toads (a regional trigger)
- **Objections to answer in copy:** "call your vet first", the cats question, price vs. $10–17 Amazon tubes, shelf life, and "don't trust internet pet products".
- Add the TikTok seed terms "pawmergency" and "activated charcoal for dogs" to `listening/SOURCES.md`. "dog ate chocolate" returned no TikTok results in this run's mix.

## 10. Unavailable or failed sources

- **Course prompts:** registry `ADD_ID`, and none stored in Supermemory.
- **ClickUp:** not configured, and not used.
- **Vantage:** not used. It covers ad structure only and is not product proof.
- **Amazon:**
  - The plain fetch of the search page returned 503.
  - igolaizola/amazon-search failed.
  - jdtpnjtp/amazon-reviews failed.
  - web_wanderer returned an empty result.
  - junglee worked.
- **Quora:** no answer text was obtained, and the web-fetch failed.
- **Facebook:** succeeded but was not read before the run stopped.
