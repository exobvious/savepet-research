# PetMergency Activated Charcoal First Aid Kit (SavePet): onboarding step five, deep research prompts 1–4 and "rate out of 10"

- **Run:** onboarding / 05-deep-research, 2026-11-02 (about 19:05–19:30 UTC), cloud research agent, Apify job tag `deep-research`
- **Variant:** 1 tube, $39.95 (shown as down from $80)
- **Product folder:** `01_petmergency_activated_charcoal_first_aid/` in `exobvious/savepet-research`
- **Status: BLOCKED.** Nothing in this stage was produced:
  - Prompts 1–4 were **not run**.
  - There is **no deep research document** and **no rating**.
  - **Nothing was written to `course_v2/`.**
  - Block 4 in `course_v2/COVERAGE_V2.md` is **not ticked**. The instruction asked for the tick, but ticking a block with no file to link would be false.
- **What stops it.** Any one of these five reasons is enough on its own:
  1. **There is no registered prompt to fetch.** Both playbook rows, "Deep research | Deep research prompts 1-4" and "Deep research | Deep research lesson", still say `ADD_ID`, and the Container column is empty. Block 4 in `FULL_COURSE_TREATMENT.md` also says `ADD_ID`. The run instruction says "fetch each prompt by ID … never reconstruct a prompt", and no ID exists. The playbook says: "A stage whose prompt column still says `ADD_ID` is reported as missing; the bot never reconstructs a prompt from memory or substitutes a similar one." AGENTS.md rule 2 says the same.
  2. **Prompt 2 has no input.** The instruction says prompt 2 absorbs "the four books in `00_rules_and_process/books/`". **That folder has 0 files in both repos**, and a search for "Bencivenga" finds nothing in either repo. The lesson says the books come from "the Knowledge Vault within the Discord".
  3. **Prompt 4 needs a tool the gateway doesn't have.** The lesson says: "Copy and paste the deep research prompt back into ChatGPT's deep research mode." OpenAI Deep Research is not available through this gateway. If I wrote the document myself, I would be quietly swapping in a different engine and method.
  4. **It is out of order.** The playbook order is: raw research, then the category context template "Only when the raw research is in", then deep research. Reddit (the course's main source) is at **0 of 156** questions run, and category context (step 4) was **BLOCKED and not run**.
  5. **A prompt 2 blank is undecided.** Prompt 2 contains "understand internal dialogue around **{INSERT ANGLE}**", and the lesson gives no default for a broad first run. One input is now settled: the "category problem" for prompt 1. `PRODUCT_DECISION.md` names the core category and six buyer problems, which the Vylaras run didn't have.
- **What this run did instead, all real and usable now:**
  - **Captured our own product page**, which is prompt 1's input, for **$0.00005** (Apify `apify/web-fetch`). It has not been captured before: no earlier run exists, and the repos have no hits for "savepet.co". The capture is in §4.
  - **Audited the page.** It has **at least 16 internal contradictions or claim risks** (§5). Prompt 1 tells the model to "internalize" the page as foundational knowledge, so these must be fixed or verified first.
  - **Checked the page testimonials against our Amazon data.** Two on-page testimonials **match word for word** reviews of the competitor listing **PawMergency (B0FXBQSFJP)** that we already hold. The only differences are a brand-name swap and one deleted sentence (§6). This is the most important finding of the run.
- **Files written:** this report only.

---

## 1. What was read (in order)

| # | Source | Result |
|---|---|---|
| 1 | `gateway_status` | scaler, vantage, apify and supermemory OK. **clickup: false** (not configured; no tasks are created by policy). GitHub OK. Apify spend today before this run: $2.23, no daily stop. |
| 2 | `get_playbook` → `UNIFIED_PLAYBOOK.md` (sha 02e8ca8) | Both Deep research rows are **`ADD_ID`**, Container empty. Research order item 4: "Deep research prompts, then rate the deep research out of 10 with named improvements." **No Supermemory space is named** for prompts or evidence. |
| 3 | `PRODUCT_DECISION.md` (sha 3f08d1e) | Core category: "Pet first aid / at-home pet poisoning response (activated charcoal)". Six buyer problems (P1–P6). Competitors: "none given yet". Locked rules: page claims, "Made in USA" and "third-party tested" are seller claims. The profile's quotes are illustrative and its numbers are hypotheses. |
| 4 | `product_truth.md` (sha a2a4a93) | 1 tube, $39.95. Coconut shell activated charcoal plus kaolin clay. Label, mL per tube, supplier, origin and bundle prices **NOT CONFIRMED**. The page's dose guidance is "internally inconsistent". |
| 5 | Reports 01–04 in `bot_reports/onboarding/2026-11-02/` (shas ec5bca1, 78576b8, 9e931f7, 52ab0a2) | 01 BLOCKED (Reddit 0/156). 02 PARTIAL (Amazon, YouTube and TikTok kept, about 75 quotes; Quora answers MISSING). 03 BLOCKED (read 30 Facebook posts, 25 owners). 04 BLOCKED (category context not run). P3 and P5 still thin. |
| 6 | `get_playbook course-treatment` → `FULL_COURSE_TREATMENT.md` (sha 9133008) | Block 4 "Deep research document" = `ADD_ID`. How a block runs: "Fetch the block's prompt by its ID, read the lesson, follow it 1:1, rate the result out of 10 … save it to `course_v2/`, tick the block". |
| 7 | `course_v2/COVERAGE_V2.md` (sha 7843df6) | All 24 blocks `[ ]` for this variant. |
| 8 | `AGENTS.md` (sha 60cd2dd), `NEVER_REPEAT_MISTAKES.md` (sha 42777e1, still empty) | Rule 2 (no ID: report missing), rule 3 (keep evidence classes apart), rule 7 (no ClickUp). |
| 9 | `telegram_log/2026-11-02.md` (sha 8290e0c) | The owner confirmed **"SavePet is the brand"** (16:40). At 17:24 she approved the rewording plus the Reddit run, which are still unqueued. **No message registers a deep research prompt, supplies books, or chooses a Deep Research engine.** |
| 10 | `00_rules_and_process/books/` (main repo) and `00_rules_and_process/` (savepet repo) | **0 files** and **0 files**. |
| 11 | `search_project_files` "Bencivenga" in both repos | 0 hits each. |
| 12 | Supermemory `list_spaces` | One space only: `research_bot` (49 docs, 118 memories). No `courses` space. |
| 13 | Supermemory `search_memory` "deep research prompts 1-4 document ID registered" (`research_bot`) | 10 hits, all status notes. Top hit: `FRJfY7wJ7Dof7nSVD5c1ap`, "Deep research could not run due to missing registered prompt, no book files, no named buyer problem, and no ChatGPT deep research tool." (doc `G3nm9qLsrf6NbPV5v7VLgk`, the Vylaras run). **No prompt document.** |
| 14 | Scaler `search_docs` (3 queries) → `get_doc(52)` | **"Learn E-Commerce Builders (4): Deep Research Using AI"** (parent "Creative Strategy", skool_url null). **I read the lesson in full** (§3). It contains the prompt 1–3 templates, the prompt 4 instruction and the rating tip. **It is not registered.** |
| 15 | Main repo `01_ai_translator_earbuds/.../05-deep-research-…md` (sha e4c9a17) | The **same stage was blocked for Vylaras** on 2026-10-21 for the same reasons. That makes this the **second occurrence** (§9, idea 9). |
| 16 | `list_apify_runs` (12 h) and repo search "savepet.co" | No earlier capture of the product page, so it was clear to buy once. The untagged Facebook Ads Library runs (actor `XtaWFhbtfxyzqrFmd`, 26 runs, $1.08) show **no new run since 18:28 UTC**. |
| 17 | Apify `apify/web-fetch`: run `NTQ3rv3WYxcBwzf1q`, dataset `k6m5i9PoGnUih17tH` | HTTP 200, fetched 2026-11-02 19:20:18 UTC. Page title "Be Prepared Instead of Too Late with PetMergency® Activated Charcoal F – SavePet". Captured as markdown (§4). |
| 18 | Apify `get-dataset-items` on `Da2ivMrrTuvpdIR5n` (step two's Amazon helpful reviews, 36 items) | A free re-read for the testimonial cross-check (§6). Nothing new was bought. |

## 2. Why I didn't run the lesson's prompts from Scaler doc 52

The lesson text is available, so running it would have been easy. I didn't, for the same reasons step 4 didn't run doc 51 and the Vylaras deep-research run didn't run doc 52:

- **The registry doesn't point to doc 52.** The playbook allows `scaler: <lesson name>` as a registry entry, but nobody has written it in. The repo, Telegram and Supermemory have no owner instruction saying "use doc 52".
- **Even if it were registered, gates 2–4 would still stop the run today:** there are no books, there is no Deep Research engine, and the raw research and category context are not done.
- **Writing a "deep research document" myself would be a reconstruction,** and with no Deep Research engine it would also be a substitution. The playbook forbids both.

## 3. What the lesson (Scaler doc 52) requires, so the owner can register it and prepare the inputs

Quoted lines are verbatim. **None of this was run.**

| Step | What the lesson says | Input needed | State for SavePet, 1 tube at $39.95 |
|---|---|---|---|
| Prompt 1 | "get ChatGPT to analyze the sales page. The goal is not to generate copy at this stage". "Go to the product page and use web2pdf to extract the PDP as a PDF file." The template is Situation / Task / Objective / Knowledge. The example is written for "a lymphatic drainage supplement". "The first prompt is filled by inserting the product name and the category problem." | PDP as a PDF; product name; category problem | PDP **captured as markdown** (§4), not as a web2pdf PDF. Product name known. **Category problem available** from `PRODUCT_DECISION.md` (core category and P1–P6), but the owner should say which wording goes in the slot (§3.1). **The page has 16 open contradictions (§5) that prompt 1 would absorb.** |
| Prompt 2 | "Now internalize ONLY the useful parts of the following persuasion frameworks. Do not adopt their writing style." The four books are **Breakthrough Advertising (Eugene Schwartz), The Bencivenga 100 (Gary Bencivenga), Scientific Advertising (Claude Hopkins), Cashvertising (Drew Eric Whitman)**. It includes "understand internal dialogue around {INSERT ANGLE}". It ends with "Frameworks internalized. Ready for Prompt 3." Then: "Attach the book files. They are found in the Knowledge Vault within the Discord." | 4 book files; angle | **Books: 0 files** in `00_rules_and_process/books/`. **{INSERT ANGLE}: undecided** for a broad run. |
| Prompt 3 | "Create a complete, fully optimized Deep Research Prompt for OpenAI's Deep Research feature." The document must be "a maximum of 8 pages", "focused ONLY on critical insights", "rich in real customer language", "optimized for use in direct response scriptwriting". "Output ONLY the final Deep Research Prompt". It ends with "Your Deep Research Prompt is ready. Paste this into Deep Research Mode". | Chat context from prompts 1–2 | Blocked upstream. |
| Prompt 4 | "Copy and paste the deep research prompt back into ChatGPT's deep research mode. This will give you your final deep research document." It "usually takes about 15 to 20 minutes." | OpenAI Deep Research | **Not available on this gateway.** |
| Rate | "ask ChatGPT to rate the deep research out of 10". Example prompt: "rate this deep research out of 10". The example scored 9.2. Improvements are optional: "you can make changes if you want to push it to a 10 out of 10." | The deep research document | Nothing to rate (§7). |
| Scope | "At the start, the research is done broadly". Rerun "with prompts adjusted to be hyper-specific" once an angle works. | n/a | Matches playbook item 6. |

### 3.1 Wording points the owner must settle when registering

These are her decisions, not mine.

1. **Prompt 1 is written for a supplement.** It mentions "ingredients", "women/men seeking solutions for lymphatic drainage" and "the Lymphatic Drainage Supplement". For SavePet, she needs to say which line fills "category problem". Options:
   - the core category verbatim ("at-home pet poisoning response")
   - P1 verbatim ("My dog ate something toxic and I have nothing at home to help")
   - or another wording of her choice
2. **Prompt 2's `{INSERT ANGLE}` on a broad run.** The lesson's example only shows angle reruns (PCOS, strawberry legs). For the first SavePet run she needs to say what goes there. The core category is the obvious candidate, but that is her call.
3. **Output filename in `course_v2/`.** The lesson gives none. A suggestion only, not decided: `course_v2/04_deep_research_1-tube-39-95.md`, with prompt 3's generated prompt saved next to it as `course_v2/04_deep_research_prompt_1-tube-39-95.md`.
4. **Regulated-claim framing.** This category is animal health and poisoning. The prompt 3 output will tell Deep Research to collect "real customer language". It should also tell it to collect **vet and poison-control positions**, which the raw research shows are loud (§5, rows 4–6). This needs to be decided **in the registered prompt**, not improvised by a bot.

## 4. Our product page as captured (prompt 1's input)

**Class:** own-brand seller claims (`competitor_claim` grade). These are **not product proof and not customer proof**.

- **Source:** https://savepet.co/products/petmergency
- **Fetched:** 2026-11-02 19:20:18 UTC, HTTP 200
- **Apify:** run `NTQ3rv3WYxcBwzf1q`, dataset `k6m5i9PoGnUih17tH`. It can be re-read for free; don't buy it again.
- Quotes are verbatim, typos included. Repeated blocks (the FAQ, the badge carousel and the review cards render 2–5 times) are listed once.

**Banner and hero**
- "🎃 **SPOOKTOBER SALE:** 62% OFF + FREE GIFTS 🎃"
- "60,000+ devoted pet parents"
- H1: "Be Prepared Instead of Too Late with PetMergency® Activated Charcoal First Aid Kit"
- "#1 VET RECOMMENDED"
- "Made in the USA | Third-Party Tested"
- "Most pet parents have nothing in the house when their dog eats chocolate off the counter or their cat licks something toxic. One ready-to-use tube of PetMergency puts the same first-response tool vets reach for in your kitchen drawer."
- Icons: "Binds Toxins Fast", "No Vomiting", "Ready in Seconds", "Dogs and Cats"
- "PLEASE BE CAREFUL OF SCAMS — WE DO NOT SELL ON AMAZON. … PetMergency is only sold here at savepets.co. Beware of fakes on Amazon/Ebay."

**Tube calculator ("How Many Tubes to Buy")**
- "larger pets need **more tubes** to get the job done"
- Weight bands:
  - "<30 lbs … Dogs & cats 1 tube"
  - "31–60 lbs … Dogs 2 tubes"
  - "61–90 lbs … Dogs 3 tubes"
  - "91–150 lbs … Dogs 5 tubes"
- Default state shown: "45lbs", giving "**2** tubes per dog × **1** dog / Total to order 2tubes"
- "Pets over 150 lbs (68 kg): start with 5 tubes and check in with your vet."
- Labelled "Vet Recommendation"

**Offer, guarantee and shipping**
- Price: "$39.95 $80.00"
- "90-Day Guarantee", "Ships in 2 Days"
- "90 Days Risk-Free Trial … We understand the skepticism. In a market full of questionable products, we believe in proof over promises."
- "100% Satisfaction / Fast Shipping / Easy Returns"
- Shipping tab: "Standard shipping typically takes 3-5 business days within the continental US."

**Scarcity**
- "SELLING OUT FAST … Once our fur parents find us, they never stop ordering."
- "88% SOLD"
- "Almost Sold Out" (button)

**Social proof**
- A Facebook-styled comment card, "Sarah LeMaster", showing "13952" and "Like Reply 8d" (see §6)
- "Rated 4.8/5 based on 7,752+ Reviews"
- "## Over 60,000+ Pet Lives Saved"
- Six review cards labelled "Verified Buyer":
  - **"Sarah, R"**: silica dust, "coughing then vomiting foam … Immediately the vomiting stopped", "Purchased on March 14th, 2025"
  - **"Mary, W, 30"**: "Not everyone can afford an emergency visit for their fur babies"
  - **"Jessi M., 32"**: the cheesesteak story (see §6)
  - **"Diane H., 58"**: "Quality is the same as what the vets use"
  - **"User1, 30"**: "I loved it came in the two pack, one for mine and one for my parents."
  - **"User1, 30"**: "Everyone who has fur babies should have this on hand"
- Survey block: "0% Feel more prepared", "0% Found it easy to give their pet in a stressful moment", "0% Would recommend", with the footnote "\* In a post-purchase survey of 900 dogs and cat owners who've bought Petmergency."

**Vet endorsement**
- "Miranda Brightstein, DVM / Board-Certified Critical Care Veterinarian"
- Quote: "I recommend _every_ pet owner keep multiple of these around the house. Don't let your lack of preparation be the reason **you lose your fur baby.**"
- Link: "Try SavePets →"

**Ingredients and mechanism**
- "Coconut Shell Activated Charcoal Kaolin Clay"
- "The Toxin Binder": "massive surface area that traps certain toxins in the gut before they can be absorbed into the bloodstream", and "Coconut shell charcoal is considered a premium, cleaner source compared to wood or coal-based charcoal."
- "The Gut Soother" (kaolin): "help absorb excess fluid and irritants, coat and soothe the stomach, and support firmer stools"
- Badges: "Made in USA", "Vet Formulated", "Pure Activated Charcoal", "Third-Party Tested"
- Comparison table, "Why SavePets Stands Out" (Original vs Others). Rows: "Immediate Release / Veterinarian Formulated / 100% Activated Charcoal / Kaolin Clay / Ready-To-Use Oral Applicator / No Artifical Flavors / Made in USA". The cell ticks don't render in text.

**Timing and the "what happens" timeline**
- "Activated charcoal is most effective within the first hour of toxin ingestion, and still effective within 4 hours for common toxins like chocolate, grapes, caffeine, medications, and rat poison."
- Tiles: Chocolate / Human Meds / Rat Poison / THC / Grapes/Raisins / Plants / Onions / Caffeine
- "First 15 Minutes": "Activated charcoal reaches the stomach and starts binding certain toxins" … "✓ Call your vet or ASPCA Animal Poison Control (888-426-4435)"
- "1 to 6 Hours": "buying your vet valuable time … follow your vet's guidance on repeat doses"
- "24 to 48 Hours": "Black stools are normal and expected … check in with your vet for follow-up care"

**FAQ (upper block)**
- Unsure what they ate: "PetMergency has a wide safety margin, so you can give it even if unsure. Unlike hydrogen peroxide, it doesn't induce vomiting or risk aspiration or throat damage."
- Use: "the dial-a-dose applicator removes guesswork—set your pet's weight (1 mL per lb), place at the side of the mouth, and dispense. No mixing, measuring, or math—even in a panic."
- Cats: "For cats, this is the only safe at-home option. Hydrogen peroxide should never be used, and the ASPCA confirms no safe alternatives. **PawMergency** is formulated for both dogs and cats."
- Timing: "Most effective within 1 hour, but still helpful up to 6. … You won't have time to order it in an emergency."
- **"Is there a shelf life?"** → "Standard shipping typically takes 3-5 business days within the continental US. International shipping times vary by location."

**FAQ (lower block)**
- Toxins covered: "Chocolate, grapes and raisins, caffeine, human medications, rat poison, THC, toxic plants, mushrooms, cane toad poison, nicotine, moldy food, household chemicals, blue-green algae, onions, and garlic."
- When to use: "The moment you suspect ingestion. Do not wait for symptoms. If you have questions, contact your veterinarian or the ASPCA Animal Poison Control Center first."
- Peroxide: "can cause esophageal burns, gastric ulcers, and aspiration pneumonia. SavePet binds toxins instead, with no vomiting needed."
- Cats: "Yes. It is dosed by weight for dogs and cats of all breeds and sizes."
- Medications: "Tell your veterinarian, since charcoal can bind medications as well as toxins."
- Picky pet: "Give it straight from the tube, or mix it with food or a favorite treat."
- Dose: "1mL per 1lb of bodyweight. Under 15 lbs: half a tube. 16 to 30 lbs: one tube. 31 to 60 lbs: two tubes. 61 to 90 lbs: three tubes. 91 to 150 lbs: five tubes. When in doubt, round up."
- Tube life: "Two years. Recap after use, store in a cool dry place, and it is ready for the next emergency."

**Merchant data:** Shopify `merchantName` "SavePet", shop-id 75028562224.

**Not on the page (still MISSING in `product_truth.md`):**
- full ingredient list and concentration
- **tube volume in mL** (see §5, row 9)
- lot or expiry printing
- manufacturer
- the 2–5 tube bundle prices (only one price renders)
- the "FREE GIFTS" contents

## 5. Contradictions and claim risks on our own page (fix or verify before prompt 1 absorbs it)

| # | Contradiction or risk | Evidence (§4 unless noted) | Why it matters |
|---|---|---|---|
| 1 | **Discount maths.** The banner says "62% OFF", but $39.95 against $80.00 is **50% off**. The banner is also "SPOOKTOBER" on 2 November. | §4 | An advertised discount that doesn't match the price is a pricing-claim risk, and the seasonal banner is stale. |
| 2 | **"Only on savepets.co / fakes on Amazon"** vs the page itself. Two testimonials are word-for-word copies of Amazon reviews of **PawMergency** (§6), and the cat FAQ says "**PawMergency** is formulated for both dogs and cats". | §4, §6; report 02 §5 (PawMergency B0FXBQSFJP, 687 reviews, $36.99) | A buyer who searches "PawMergency" finds a cheaper listing carrying our testimonials. That supports the "don't trust internet pet products" objection ("ya i don't trust any pet products that come from the internet and not the vet🥹", TikTok, 78 likes, report 02 §4.3). |
| 3 | **Cats.** The page says "For cats, this is the only safe at-home option … the ASPCA confirms no safe alternatives." The second FAQ only says "Yes. It is dosed by weight". | §4 vs "NOT SAFE FOR CATS" (TikTok, 575 likes, report 02 §4.6) | Locked as a seller claim in `PRODUCT_DECISION.md`. The ASPCA attribution is **unverified** (no source cited), and customer voice disputes the claim. Don't let prompt 1 internalize it as fact. |
| 4 | **"No Vomiting" / "no aspiration"** vs the page's own lead review and vet-staff warnings. "Sarah, R" gave it to a dog that was "coughing then vomiting foam". | §4 vs "My vet said please don't use that she could aspirate the charcoal in her lungs and get pneumonia so I returned it." (Amazon RXIWHMIQJDOQL, B0FXBQSFJP) and "charcoal can cause dangerous electrolyte imbalances!" (TikTok, 2,533 likes) | An absolute safety claim faces the loudest negative evidence in the category. It needs verification in block 2 (clinical). |
| 5 | **Call the vet first, or dose first?** One FAQ says "If you have questions, contact your veterinarian or the ASPCA … **first**." Another says "you can give it even if unsure". The 15-minute timeline puts "Call your vet or ASPCA" **after** dosing. | §4 vs "PLEASE … do not give activated charcoal without FIRST REACHING OUT TO PET POISON HELPLINE!!!" (TikTok, 92 likes) and "do not give unless instructed by a vet or poison control" (65 likes), report 02 §4.6 | Customers already split on this (report 03 §8.5: "charcoal plus the call to your vet"). The page says three different things. |
| 6 | **"Wide safety margin … When in doubt, round up."** | §4 | A dosing-safety claim with no source. A pro commenter: "in some cases you can ABSOLUTELY cause more harm than good" (320 likes, report 02 §4.6). Block 2 territory. |
| 7 | **Effective window: 1 h / 4 h / 6 h.** "still effective within 4 hours" vs "still helpful up to 6" vs the "1 to 6 Hours" timeline. | §4 | Internal inconsistency on the one fact owners ask about most: "when do you know when to administer the charcoal?" (Facebook, Mangels, report 03 §4.4). |
| 8 | **Toxin list breadth.** It includes "household chemicals", "nicotine", "blue-green algae", "THC", "mushrooms". | §4 vs "not all toxins can be treated with charcoal so make sure you do your own research" (Amazon R98C0V79UQ94X, B0FNY9J7ZT, customer_report) | Coverage of each named toxin is **unverified** (hypothesis to test in block 2). Over-broad claims invite the vet pushback in rows 4–6. |
| 9 | **Dose and tube volume.** The calculator says "<30 lbs Dogs & cats 1 tube"; the FAQ says "Under 15 lbs: half a tube. 16 to 30 lbs: one tube"; and "1mL per 1lb". | §4; `product_truth.md` | Read together, this works if the calculator means **tubes to buy** and the FAQ means **dose**. 1 mL/lb with "16 to 30 lbs: one tube" and "91 to 150 lbs: five tubes" **implies about 30 mL per tube**, which matches the Amazon reviewer's "One tube covers 30 lbs" (R1PJXSAJA58WNE). **Hypothesis, NOT CONFIRMED**: the label must state the volume. The page never says it. |
| 10 | **"100% Activated Charcoal" / "Pure Activated Charcoal"** vs "Coconut Shell Activated Charcoal **Kaolin Clay**". | §4 | A two-ingredient product sold as "100%" charcoal. Ingredient-claim risk. |
| 11 | **Shelf life.** The "Is there a shelf life?" answer is shipping text. A separate FAQ says "Two years". There is no lot or expiry information. | §4 vs "There is no manufacturing date on the charcoal on any of the five … we could be buying old charcoal that will in fact do nothing" (Amazon R2L1FFS3VVEJ4O, B0FXBQSFJP) | Already flagged on Telegram (15:05). Still live. |
| 12 | **Survey stats show 0%.** "0% … Would recommend", from a "survey of 900 dogs and cat owners". | §4 | It reads as broken or invented proof, and the survey has no source. |
| 13 | **The same "60,000+" number is used for two different claims:** "60,000+ devoted pet parents" and "Over 60,000+ Pet Lives Saved". | §4 | Locked as a seller claim. Buyers are not the same thing as lives saved. |
| 14 | **Review count signals don't agree.** "4.8/5 based on 7,752+ Reviews", while the Facebook-style card shows "13952" reactions on one comment, which is an Amazon review (§6). | §4, §6 | The trust family already carries fake-proof suspicion ("does anyone know if it's legitimate?", Facebook, Graziano, report 03 §4.6). |
| 15 | **Brand spelling.** SavePet (title, Shopify merchant) vs "SavePets" ("Try SavePets →", "Why SavePets Stands Out", "savepets.co"), plus "PawMergency" and "Petmergency". | §4; owner confirmed "SavePet is the brand" (Telegram 16:40) | The page still contradicts the owner's decision. The "savepets.co" domain on the anti-scam line may not be the store's domain (savepet.co). |
| 16 | **Named vet, "#1 Vet Recommended", "Made in USA", "Third-Party Tested", "Vet Formulated", "PetMergency®".** | §4 | All are locked as seller claims. I had no licence lookup, trademark lookup or test-certificate source, so **none of them was checked**, and the report makes no finding about whether they are true. Prompt 1 must not internalize them as product truth. |

**Minor items, possibly the theme or the capture:**
- "Ships in 2 Days" vs "3-5 business days". This may be processing time vs transit time.
- "88% SOLD" and "Almost Sold Out" sit next to an orderable product.

**What the page does add (brand claims only; candidates for `product_truth.md` as "page claims"):**
- 90-day guarantee, consistent everywhere on the page
- ASPCA number shown on the page
- "Recap after use"
- "Give it straight from the tube, or mix it with food"
- black stools expected
- charcoal can bind medications
- implied tube size of about 30 mL (row 9, a hypothesis)

## 6. Page testimonials that match competitor Amazon reviews (cross-check against data we already hold)

I compared the page capture with step two's Amazon dataset `Da2ivMrrTuvpdIR5n` (36 reviews), re-read for free.

| Page card | Amazon source | Match |
|---|---|---|
| **"Sarah LeMaster"**, Facebook-style card, "13952", "Like Reply 8d": "This stuff absolutely works and offers huge piece of mind. We've had to use it twice on a puppy who was able to inhale chocolate on two occasions where their human looked away for two seconds. A huge mistake and lesson learned for the human, but also having this for such human mistakes was a lifesaver. One tube covers 30 lbs in weight, so be sure to purchase enough to cover the weight of all babies in your home, in case it's a team effort to ingest something bad. All in all I'm so thankful for this product." | **R1PJXSAJA58WNE**, PawMergency **B0FXBQSFJP**, 5★, 2026-05-27, user `AFTJIGUIWQTITDJ2IMEFCA7DHSNQ`, title "This absolutely works - had to use it twice on a rambunctious puppy" | **Word for word**, except that one sentence is **missing** from the page version: "**It's expensive but 100% worth the emergency use, piece of mind, and health of your precious baby.**" The price remark is the line that was removed. |
| **"Jessi M., 32" Verified Buyer**: "I was baking a pie and eating a cheesesteak one night … I immediately grabbed the **Petmergency** from my purse and gave it to him. … we avoided a trip to the vet! Will definitely be buying more soon!" | **RU0M4MDBVULVD**, PawMergency **B0FXBQSFJP**, 5★, 2026-09-21, user `AG434AREOFTXHCDWREOMGL7TIPNA`, title "Essential for every household with pets" | **Word for word**, with "**Pawmergency**" changed to "**Petmergency**". |
| "Sarah, R" (silica dust), "Mary, W", "Diane H.", both "User1" cards | — | **No match** in the 44 Amazon reviews we hold (36 helpful plus 8 critical). Origin unknown. Not checked further. |

**Class:** `conclusion` for the text match, which can be checked from the two sources above. `hypothesis` for any explanation.

**Possible explanations, none verified:**
- (a) SavePet and PawMergency are the same white-label goods, and the reviews were taken from the supplier's listing.
- (b) The page copy was lifted from the competitor's Amazon listing.

Either way, the page presents another brand's Amazon reviewers as a SavePet "Verified Buyer" and as a Facebook commenter. It also says "WE DO NOT SELL ON AMAZON … Beware of fakes on Amazon".

- **This is a compliance risk for the owner to review.** It is not a legal conclusion from me. Endorsement and review rules generally require testimonials to be genuine and about the advertised product.
- **For this stage specifically:** prompt 1 would "internalize" these cards as SavePet customer voice and social proof. They must be removed or relabelled before any deep research run, or the research will be built on another brand's reviews.
- **It strengthens report 02's open question (§8.6):** "Ask the supplier ("My Vereli") whether SavePet = PawMergency stock."

## 7. "Rate out of 10" step

**Not applicable: there is no deep research document to rate.** I did not rate an improvised document as a stand-in.

For the owner's planning only, here is an **input-readiness check** against the lesson's inputs. It is **not** the course's rating and carries no score.

| Input the lesson needs | Ready? |
|---|---|
| Registered prompt and lesson IDs (registry and block 4) | **No.** `ADD_ID` |
| PDP for prompt 1 | Captured as markdown (§4). Needs a web2pdf PDF and **the §5–§6 fixes first.** |
| Product name and category problem (prompt 1) | **Yes, mostly.** The owner should choose the slot wording (§3.1). |
| Four book files (prompt 2) | **No.** Folder empty in both repos. |
| `{INSERT ANGLE}` for a broad run (prompt 2) | **No.** Undecided. |
| OpenAI Deep Research access (prompt 4) | **No.** Not on this gateway. |
| Raw research in, then category context run once (playbook order) | **No.** Reddit 0/156, Quora answers MISSING, P3 and P5 thin. Category context not run (report 04). |

## 8. Unavailable or failed sources

- **Deep research prompts 1–4 and the deep research lesson:** `ADD_ID` in the registry and in block 4. They exist only as unregistered text in Scaler doc 52. There is no Supermemory prompt document.
- **The four books:** absent from `00_rules_and_process/books/` in both repos, from Supermemory, and from repo search.
- **OpenAI Deep Research mode:** no such tool on this gateway.
- **Supermemory course space:** none. `research_bot` holds Telegram copies and step notices only.
- **Vantage:** not used. It gives ad structure only, never product or customer proof. On Telegram (15:05) the assistant reported that Vantage had nothing on SavePet or pet first aid.
- **Verification of page claims** (named DVM, ® mark, Made in USA, third-party testing, ASPCA cat statement): no source tool for licences, trademarks or certificates. **Not checked.** They stay seller claims.
- **ClickUp:** not configured and not used. No tasks were created.
- **Reddit, TikTok, Facebook, Quora:** not in this stage's scope. Reddit is still unrun from step one.
- **Tool failures this run:** none. Every call answered. The stage stopped on missing inputs.

## 9. Ideas for the owner (not tasks; nothing was assigned or scheduled)

In order of what unblocks block 4:

1. **Fix the page before anything "internalizes" it**, starting with §6:
   - Remove or replace the two PawMergency-sourced testimonials.
   - Settle whether SavePet is PawMergency stock (ask "My Vereli").
   - Rework the "WE DO NOT SELL ON AMAZON / fakes" line in light of that answer.
   - Then work through §5:
     - 62% vs 50%, and the Spooktober banner
     - the cat claim and the ASPCA attribution
     - "No Vomiting / no aspiration"
     - one clear vet-call order
     - one effective window
     - the toxin list
     - "100%/Pure" charcoal
     - the shelf-life answer, plus lot and expiry on the tube
     - the 0% survey
     - the two "60,000+" claims
     - SavePets / PawMergency / Petmergency spellings
2. **Register the stage.** Write `scaler: Learn E-Commerce Builders (4): Deep Research Using AI (doc 52)` in both Deep research rows and in block 4 of `FULL_COURSE_TREATMENT.md`. Or upload your own versions of prompts 1–3 and the lesson to Supermemory (for example a `courses` space) and paste the IDs. Settle the §3.1 points at the same time: the category-problem slot, `{INSERT ANGLE}` on a broad run, the output filename, and whether vet and poison-control positions are explicitly in scope.
3. **Put the four books in `00_rules_and_process/books/`, or in Supermemory with IDs.** The books are Breakthrough Advertising, The Bencivenga 100, Scientific Advertising and Cashvertising. They are copyrighted Knowledge Vault files, so keep them in a private location, and confirm the repo is private before committing them.
4. **Decide how prompt 4 runs**, since no Deep Research tool is available here. Options:
   - (a) you run prompts 1–4 in ChatGPT yourself and commit the output to `course_v2/`, and a bot then rates it ("rate this deep research out of 10"), files it and ticks block 4;
   - (b) a Deep Research-capable tool is added to the gateway; or
   - (c) you approve a named substitute in writing.

   Until then, every bot run of this stage will block the same way.
5. **Finish what comes first in the playbook order.**
   - Send "queue reddit" so the approved rewording and the Reddit run go ahead (cap $6). Aim hardest at P3 ("vet closed") and P5 ("poison control fee", "hold").
   - Build `EB_CATEGORY_CONTEXT_<slug>_v2.md` from report 02 §4 and report 03 §4.
   - Run category context once.
   - **Then** deep research.
6. **Update `product_truth.md` with the page's facts, labelled "page claim".** These are the 90-day guarantee, "Recap after use", the mix-with-food option, the expected black stools, the medication-binding caution, and the implied tube size of about 30 mL (§5, row 9). Have the label confirm the mL.
7. **Add PawMergency (B0FXBQSFJP), PetVet Medic (B0FNY9J7ZT), Vetanica and NOW to Competitors** in `PRODUCT_DECISION.md`. The §6 finding makes PawMergency the most important of these.
8. **Send block 2 (clinical, "a plus, never a gate") the questions this page raises:**
   - which of the 15 listed toxins charcoal actually helps with
   - aspiration risk when a pet is vomiting or coughing
   - electrolyte risk
   - use in cats
   - the real effective window
   - dosing at 1 mL/lb
9. **Proposed `NEVER_REPEAT_MISTAKES.md` line.** This has now gone wrong twice (Vylaras 2026-10-21, SavePet 2026-11-02):
   > "Don't queue deep research (block 4) until its registry rows have IDs, the four books are in `00_rules_and_process/books/`, a Deep Research engine or a human hand-off is decided, and category context has run (2026-11-02, second occurrence)."
10. **Possible standing rule:** capture our own PDP once per onboarding and cross-check its testimonials against the review data already bought, before any prompt internalizes it. It cost $0.00005 here and caught §6.

## 10. Outputs of this run

| Output | State |
|---|---|
| `01_petmergency_activated_charcoal_first_aid/course_v2/<deep research document>` | **Not created.** There is no registered prompt, no books, no Deep Research engine, and the earlier stages are incomplete. An improvised document would misrepresent the course's output. |
| Prompt 3's generated deep research prompt | **Not created** (blocked upstream). |
| Rating out of 10 | **Not applicable** (§7). |
| `course_v2/COVERAGE_V2.md` block 4, variant "1 tube - $39.95 (shown as down from $80)" | **Not ticked.** It has no output file to link. All 24 blocks are still `[ ]`. |
| Product page capture | §4 of this report. The full markdown is in dataset `k6m5i9PoGnUih17tH`. |
| Testimonial cross-check | §6 of this report. |

**Pull log**

| Actor | runId | datasetId | Bought | Kept | Cost |
|---|---|---|---|---|---|
| `apify/web-fetch` https://savepet.co/products/petmergency (job `deep-research`) | NTQ3rv3WYxcBwzf1q | k6m5i9PoGnUih17tH | 1 page | 1 (§4) | $0.00005 (reported at poll) |
| `get-dataset-items`, Amazon helpful reviews (step two's purchase) | — | Da2ivMrrTuvpdIR5n | 0 (free re-read of 36) | 2 matches (§6) | $0.00 |

**Total Apify spend this run: about $0.00005.** Scaler (`search_docs`, `get_doc`), Supermemory (`list_spaces`, `search_memory`) and GitHub reads were free.
