# PetMergency (SavePet): copying the owner's avatar profile, updating the brand in product truth, and checking the profile against the evidence

- **Run:** telegram / 03-avatar-copy-and-check, 2026-11-02 (UTC), cloud research agent
- **Repo / folder:** `exobvious/savepet-research` / `01_petmergency_activated_charcoal_first_aid/`
- **Status: PARTIAL. Task 3 is done, but tasks 1 and 2 could not be committed.**
  - **Task 1 (avatar copy): NOT COMMITTED.** The gateway turned down the write to `01_petmergency_activated_charcoal_first_aid/avatar/owner_avatar_profile.md` with: `This job may publish only to 01_petmergency_activated_charcoal_first_aid/bot_reports/telegram/2026-11-02/03-avatar-copy-and-check.md`. The full file (header plus the profile text) is in **Appendix A**, ready to commit. **The original in `exobvious/research` was not touched.**
  - **Task 2 (product_truth.md): NOT COMMITTED.** The same error came back on `01_petmergency_activated_charcoal_first_aid/product_truth.md`. The new file text is in **Appendix B**. It adds only a Brand section and a change-log line.
  - **Task 3 (checking the profile): DONE** (§3–§5). Every point is marked supported, contradicted or not yet tested, with the verbatim quote and its URL or stable ID. Every quote comes from reports already in the repo. **This run collected no new quotes.**
  - **This report is the only file written.** The repo's `product_truth.md` (sha a2a4a93) is unchanged, and `avatar/` still holds only `README.md`.
- **Spend: $0.00 on Apify.** No actor was called. The only reads were free: GitHub, one Supermemory `search_memory`, `gateway_status` and `get_playbook`.
- **No ClickUp tasks were created** (ClickUp is not configured, and tasks aren't created by policy). Ideas are listed in §7.

---

## 1. What was read

| Source | Result |
|---|---|
| `gateway_status` | scaler, vantage, apify and supermemory OK. **clickup: false.** GitHub OK. Apify spend today before this run: $4.17. |
| `get_playbook` (UNIFIED_PLAYBOOK.md, sha 02e8ca8) | Every prompt registry row still says `ADD_ID`, and **no Supermemory space is named** for the course method or for evidence. The \"Avatar\" and \"Clean-up\" rows are `ADD_ID` too. That doesn't block this step, because copying and fact-checking an owner document runs no course prompt. **No course avatar prompt was run, rebuilt or substituted.** |
| `00_rules_and_process/telegram_log/2026-11-02.md` (main repo, sha e4a7479) | 16:12: the assistant warned that the profile's \"quotes are made up as examples\", that its numbers aren't sourced, and asked whether \"Made in USA\" / \"third-party tested\" are true. **No answer from the owner on either claim is in the log.** 16:40: the owner wrote \"SavePet is the brand. queue copy.\" The scope of this step was set at 16:40 and 17:25. |
| Owner profile `SavePet PetMergency Avatar Profile.txt` (main repo, sha 10f11d2) | Read in full. It has 12 sections. It contains **no search-word list**. The search words and subreddits were taken from it on Telegram (16:12) and stored in `listening/SOURCES.md` (sha a9f0812). I check those in §4.8. |
| `product_truth.md` (a2a4a93), `PRODUCT_DECISION.md` (3f08d1e) | Six problems. Locked: page claims and \"Made in USA\" / \"third-party tested\" are seller claims, and the profile's quotes are illustrative with numbers as hypotheses. `PRODUCT_DECISION.md` still says \"Brand spelling SavePet vs SavePets not confirmed\", which is now out of date (see §6.4). |
| Onboarding reports 01–05 (ec5bca1, 78576b8, 9e931f7, 52ab0a2, 2e6de73) | 01, 03 (as a stage), 04 and 05 (as a stage) BLOCKED. **Evidence comes from:** 02 (Amazon, YouTube, TikTok, Quora), 03 §4 (30 Facebook posts read), and 05 §4–§6 (our page capture and the testimonial match). |
| Telegram reports 01 (fdc0043) and 02 (f66bec6) | 01 is the question bank and holds no evidence. **The tool output was cut off partway through §5**, but that section holds only questions, so nothing in this check depends on it. 02 is the Reddit run: Tier A quotes verified in opened threads, Tier B excerpts with links but not opened. |
| Supermemory `search_memory` (`research_bot`) | No stored copy or check of the profile. Two memories state things too strongly (§6.5). |

**Source tiers used below**
- **Tier A:** a quote read in the opened post, comment, review or thread.
- **Tier B:** a Reddit Answers excerpt with a permalink, where the thread was not opened. It is unverified and is never the only support for a \"supported\" verdict.

**Evidence classes**
- `customer_report`: an owner describing their own pet.
- `pro_opinion`: someone speaking as vet staff. Unverified.
- `competitor_claim`: seller or affiliate content, including our own page.
- `hypothesis`
- `conclusion`

**URL rules**
- Reddit links are given as in the reports. Where a report gave only the subreddit and post ID, the link is built as `https://www.reddit.com/r/<sub>/comments/<id>/`.
- Amazon reviews: `https://www.amazon.com/gp/customer-reviews/<id>`, as in report 02.
- YouTube: video ID plus comment ID (`lc`).
- TikTok: video URL plus comment ID.

---

## 2. The profile in one line, and what this check can and can't say

The profile is an owner-written summary (\"a deep-dive synthesis\"). Its quoted soundbites are **illustrative**, so none of them is counted as evidence for itself. A **\"supported\"** verdict means real owner voice in the repo says the same thing. It does **not** mean the profile's wording was found. The demographic and percentage claims can't be tested with the customer-voice data we hold, which carries no age, income or gender fields. They are marked **not yet tested**, not contradicted.

**Tally (§3–§5): 66 points checked.**

| Verdict | Count |
|---|---|
| Supported | 30 |
| Supported in part, with a contradiction | 11 |
| Contradicted | 7 |
| Not yet tested | 18 |

The 30 \"supported\" points include 4 resting on a single report.

---

## 3. Who the buyer is (Section 1) and the core problem (Section 2)

| # | Profile point | Verdict | Evidence (class, verbatim, source) |
|---|---|---|---|
| B1 | Composite \"Jessica / Mike\". Ages 27–42 (primary) and 43–55 (secondary) | **Not yet tested** | Nothing we hold records age. Report 01 (telegram) kept the questions neutral as \"pet owners\" for this reason. |
| B2 | \"~65% Female / 35% Male\" | **Not yet tested** | No gender field. Posters include both men and women, for example Facebook \"Christopher Johnson\" (\"so wife and I dont lose our fur babies\") and \"Karen Lunning\". A count of names isn't evidence of the split. |
| B3 | \"1–3 pets (dog and/or cat)\" | **Supported in part** | Dog and cat owners both show up. Cat: \"he charged me $150 of poison control communication fee\" (customer_report, cat ate lily, https://www.reddit.com/r/AskVet/comments/1i2u1bu/). Multi-dog: \"How much do I give a 60 pound pit and a 37 pound Pittie mix.\" (customer_report, https://www.facebook.com/groups/DuncanStrong/posts/2078592759537933/). **Exceeds the 1–3 range:** \"I have 5 beautiful shepards\" (customer_report, Belize, https://www.facebook.com/groups/communityanimalrescue/posts/2823914071316110/). |
| B4 | The pet is a \"fur baby\" and a full family member | **Supported** | \"so wife and I dont lose our fur babies?\" (customer_report, https://www.facebook.com/groups/theleessummitcommunity/posts/28439017415799009/). \"furbabies\" (Amazon https://www.amazon.com/gp/customer-reviews/RIFGTSSJTXYV1). \"the love of our life is possibly sick\" (customer_report, https://www.reddit.com/r/puppy101/comments/utaup0/). |
| B5 | Renting or owning; may have children | **Not yet tested** | One owner with a child: \"my toddler misplaced my phone charger so I was panicking\" (customer_report, comment gjov3dq, https://www.reddit.com/r/puppy101/comments/kzmwje/). That is one person, not a pattern. |
| B6 | \"Income 120,000/yr; spends liberally on pet care\" | **Contradicted** as a picture of the people who have this problem. **Not tested** for actual buyers. | Many owners in the moment can't pay: \"I can't afford the $90 poison control call\" (customer_report, https://www.reddit.com/r/AskVet/comments/1otlu68/). \"I dont have funds for vet til next week\" (customer_report, https://www.facebook.com/groups/theleessummitcommunity/posts/28439017415799009/). \"I'm scared and crying because I don't have money to take them to the vet\" (customer_report, YouTube eKRzJ3sxUlc, lc=UgzoRXrLkASnluf7gjx4AaABAg). \"Thank goodness I had someone I could borrow the money from\" (customer_report, https://www.reddit.com/r/puppy101/comments/kzmwje/). The \"feels exposed to large unexpected vet bills\" half is supported. The income figure has no source. |
| B7 | \"82% of this market says their pet is like their own child\" | **Not yet tested** | Unsourced. B4 supports the feeling, not the percentage. |
| B8 | \"Reactive preparer… One near-miss transforms them into a voracious buyer\" | **Supported in part** | Near-miss leading to a purchase: \"Our super fast Shih Tzu got ahold of my husband's Warfarin pill… A friend of mine suggested keeping this on hand\" (customer_report, https://www.amazon.com/gp/customer-reviews/R3V0WAMC78GXMM). \"Can anyone recommend activated charcoal that I can have at home and give my dog the next time they get into something?\" (customer_report, https://www.reddit.com/r/DogAdvice/comments/1urz7u6/). **But two other buying moments also exist.** Before any incident: \"Just bought it to have on hand just in case.\" (customer_report, https://www.facebook.com/groups/holisticandnaturalpets/posts/4520364248227111/). During the emergency: \"my cat got into some rat poison so prime delivery was same day\" (customer_report, https://www.amazon.com/gp/customer-reviews/R39B5Y92LBQFYO). |
| C1 | Core problem: \"she has absolutely nothing at home to do anything about it\" | **Supported** | \"Lf activated charcoal for dogs asap\" (customer_report, https://www.facebook.com/groups/326828460987298/posts/3044464939223623/). \"I can not find activated charcoal in the stores anywhere.\" (customer_report, https://www.facebook.com/groups/petvetcorner/posts/1684184149272280/). \"I order activated charcoal from amazon but it's gonna arrive just on Sunday… I can't wait till Sunday.\" (customer_report, https://www.reddit.com/r/AskVet/comments/10hdn3j/). \"Is there anything I should do right now? It's 1138 at night.\" (customer_report, https://www.facebook.com/groups/7138117442873230/posts/26281064311485256/). |
| C2 | The named toxins: chocolate, rat poison, a dropped prescription pill, grapes, toxic houseplants | **Supported** (grapes from only 1 report) | Chocolate: many reports, for example the Hershey's bar post above. Rat poison: \"dropped a huge block of rat poison on the ground… We got his stomach pumped\" (customer_report, comment k9nk3yk, https://www.reddit.com/r/Pets/comments/17xefh8/). Pills: \"My dog swallowed my mothers naproxen pill\" (customer_report, https://www.facebook.com/groups/asktheveterinarian/posts/1520850722800456/) and \"My dobie took a half full bottle of ibruprofen off the counter\" (comment kpuso9i, https://www.reddit.com/r/DobermanPinscher/comments/1anrg6x/). Grapes: \"left grapes on the kitchen table, got distracted in another room\" (customer_report, YouTube v-k4ezLEkLU, lc=Ugxf3qrD8WynIcBDwbB4AaABAg). Plants: cat lily (1i2u1bu above) and \"cat ate a plant\" (10hdn3j above). **Not in the profile but in the evidence:** cane toads, in Florida and Belize (4 reports, report 03 §7). |
| C3 | \"451,000+ calls… one call every 70 seconds… nearly 4% increase\" | **Not yet tested** | Unsourced. No source was fetched (no spend allowed, and it isn't customer voice). Hypothesis only. |
| C4 | \"$80/month on premium dog food, $200 on annual vet checkups, $50 on organic treats\" | **Not yet tested** | No evidence either way. |
| C5 | \"the first 60 critical minutes\" / \"the clock starts the moment the toxin goes down\" | **Supported as a belief owners hold.** **Not tested as a clinical fact.** | \"Every minute counts.\" (customer_report, https://www.reddit.com/r/AskVet/comments/1t6mhey/pet_poison_control/). The 1-hour window is a mechanism claim. Our own page says three different things: \"within the first hour\", \"still effective within 4 hours\", \"still helpful up to 6\" (competitor_claim, report 05 §5 row 7). |

## 4. The six buyer problems (from the profile, as registered in PRODUCT_DECISION.md)

| # | Problem | Verdict | Evidence |
|---|---|---|---|
| P1 | \"My dog ate something toxic and I have nothing at home to help\" | **Supported** | See C1. Also \"I feel like we're playing with fire, our dogs are constantly getting into potentially dangerous stuff and the nearest vet is 2+ hours away\" (customer_report, https://www.reddit.com/r/DogAdvice/comments/1urz7u6/). |
| P2 | \"Should I make him throw up with peroxide?\" | **Supported**, with contradictions | The question is asked: \"Should I induce vomiting?\" (customer_report, https://www.facebook.com/groups/asktheveterinarian/posts/1584055409813320/). It fails: \"It's been about 3 hours since the HP and other than some nauseated licks she hasn't thrown anything up.\" (customer_report, https://www.reddit.com/r/AskVet/comments/1ld0da7/). **Contradiction:** it works for some owners. \"he threw up 5 min later… I'm so thankful for this video.\" (customer_report, YouTube v-k4ezLEkLU, lc=UgwEOdoUpi5i2IPUXrN4AaABAg). Some vets still tell owners to use it: \"I talked to my vet who recommended inducing with hydrogen peroxide.\" (customer_report, https://www.reddit.com/r/AskVet/comments/1ttxg2h/). |
| P3 | \"The vet is closed at night\" | **Supported.** Rural distance shows up as often as night closure. | \"ended up calling the nearest vet and they are not open until tomorrow\" (customer_report, https://www.reddit.com/r/AskVet/comments/1ld0da7/). \"Nothing is open right now, so I am not sure what to do.\" (customer_report, https://www.reddit.com/r/AskVet/comments/fsplqw/). \"As it's around 11PM, our vet is closed\" (customer_report, https://www.reddit.com/r/puppy101/comments/utaup0/). Rural: \"He lives in a very rural area, nearest vet is nearly 2 hours away.\" (1ld0da7). |
| P4 | \"A $2,000 emergency vet bill\" | **The cost pain is supported. The $2,000 figure is contradicted as the typical bill.** | Bills reported: \"Total cost almost $350.\" (https://www.reddit.com/r/AskVet/comments/1i0mqo2/); \"the worlds most expensive bowl of chipotle ($400!)\" (utaup0); \"$500 at the emergency vet\" (comment k9oc6vw, 17xefh8); \"a $600 vet visit\" (https://www.facebook.com/groups/dogalogue/posts/1869962833683603/); a deposit \"of $ 1000\" (Quora, https://mariatrudelsspace.quora.com/This-past-July-01-holiday-I-was-dog-sitting-my-brother-his-wife-s-dog-while-they-were-in-Ontario-We-have-dog-sat-thi). **Only one Tier A report reaches $2,000:** \"This would've saved me 2 grand 😅\" (customer_report, TikTok https://www.tiktok.com/@jeremysfinds/video/7541048399605353741, cid 7572279429965300493). One Tier B report is higher: \"It was 3 grand\" (r/Pensacola 1ty5w5l, comment oq141hk, unverified). |
| P5 | \"Poison control charges a fee and puts me on hold\" | **Supported** (strongest of the six) | \"It costs $85.00 on my credit card to even be put through to Animal Poison Control… I've never waited less than 35 min.\" (customer_report, https://www.reddit.com/r/AskVet/comments/1t6mhey/pet_poison_control/). \"they wouldn't take my call until I gave them a credit card. After almost 20 minutes on hold.\" (customer_report, comment kpufboy, https://www.reddit.com/r/DobermanPinscher/comments/1anrg6x/). \"We spent 2 hours on hold with ASPCA poison control tonight\" (customer_report, https://www.reddit.com/r/Pets/comments/1o68fek/). **Counter-evidence:** after vet staff explained the fee, one owner wrote \"Thank you for this very thoughtful and reasonable response. It makes perfect sense\" (comment okm5ksi, 1t6mhey). One thread is titled \"Had a great experience with poison control\" (r/puppy101, 2021-06-25; title only). |
| P6 | \"I'm scared I'd give the wrong amount in a panic\" | **Supported.** The evidence adds *when* to give it, not only *how much*. | \"When your stressed, the less time you spend trying to figure out how large a dose, could be a life saver.\" (customer_report, https://www.amazon.com/gp/customer-reviews/R3V8DHN3ZZHS1Z). \"I would just like a double check on dosage!\" (customer_report, https://www.reddit.com/r/AskVet/comments/189k2n6/). \"the bottle didn't say anything about how to serve it.\" (customer_report, competitor product VetDTox, https://www.reddit.com/r/DogAdvice/comments/18l9sv8/). \"when do you know when to administer the charcoal?\" (customer_report, https://www.facebook.com/groups/837889829591939/posts/27967074699580085/). |

## 5. The rest of the profile, point by point

### 5.1 Emotions (Section 3)

| # | Point | Verdict | Evidence |
|---|---|---|---|
| E1 | Anticipatory dread, a \"low-level hum of 'what if'\" | **Supported** | \"I feel like we're playing with fire\" (1urz7u6). \"It's been my worst nightmare since moving here\" (customer_report, cane toads, https://www.facebook.com/groups/holisticdomesticpetcare/posts/2016643172330081/). \"It was so scary. I'm with them almost every minute, but they still get into everything at that age.\" (customer_report, YouTube xG1nLBTzPDo, lc=Ugwe3IGhMDsKmksLJqV4AaABAg). |
| E2 | Guilt | **Supported** | \"I'm kicking myself and currently a mess of guilt\" (customer_report, https://www.reddit.com/r/AskVet/comments/irkjyg/). \"it's our fault for leaving a half a bowl of Chipotle out\" (utaup0). \"I'm feeling so stupid\" (https://www.reddit.com/r/AskVet/comments/1g5cd9h/). \"A huge mistake and lesson learned for the human\" (customer_report, https://www.amazon.com/gp/customer-reviews/R1PJXSAJA58WNE). |
| E3 | Helplessness: \"STANDING THERE, panicking, Googling, crying\" | **Supported** | \"i am balling my eyes out and frantically searching for information.\" (customer_report, YouTube Mtx6oLVVJ7k, lc=Ugy-A6F81CjZUsP0w354AaABAg). \"I'm shaking and I looking up videos on what to do\" (YouTube eKRzJ3sxUlc, lc=UgyayF849co2HRGmcjB4AaABAg). \"I'm at a loss for what to do next\" (1ld0da7). |
| E4 | Financial panic | **Feeling supported. \"38%\" not yet tested.** | \"I can't really afford the $95 animal poison control fee rn.\" (1g5cd9h). \"I'm pretty strapped for cash.\" (Tier B, r/Rottweiler 1v8xzzl). The 38% figure has no source. |
| E5 | Protective rage (\"If someone broke into my house, I'd act\") | **Not yet tested** | No owner uses an intruder or rage frame. The anger we do see points at the hotline system, not at the threat: \"Who is this serving?\" (1t6mhey) and \"Why Tf does animal poison control charge $50.00 freaking dollars?!\" (customer_report, https://www.reddit.com/r/puppy101/comments/kzmwje/). |

### 5.2 Fears (Section 4)

| # | Point | Verdict | Evidence |
|---|---|---|---|
| F1 | \"I was right there\": frozen, on hold, the vet \"can't see me for three hours\" | **Supported in its parts** | Hold: see P5. No vet will see the pet: \"We tried five vets, in a city of 42,000, but none would see her\" (customer_report, https://www.reddit.com/r/DogAdvice/comments/1196aql/). Distance: \"the closest one is 3 hours away\" (Tier B, r/AskVet 1n4lw7u). The seizure image shows up only once, in a success story: \"Full blown seizure to fine\" (TikTok muonline_pc/7514895346850336031, cid 7524875251797820191). |
| F2 | The \"too late\" discovery after hours or overnight | **Not yet tested** (closest only) | Finding it after the fact: \"I just got home from an event and I found this Hershey's bar on the floor… It's 1138 at night\" (Facebook Swann, above). \"Too late\" from the ER: \"the ER Hospital said I could bring them to have the tummy pumped but at that point...too late\" (customer_report, YouTube xG1nLBTzPDo, lc=Ugwe3IGhMDsKmksLJqV4AaABAg). No overnight or asleep scenario has been found. |
| F3 | Being seen as negligent: the vet's look, \"why didn't you have anything at home?\" | **Self-blame supported. The vet judging you for *lacking* charcoal is contradicted.** | Self-blame: \"I feel like such a moron.\" (https://www.reddit.com/r/DogAdvice/comments/1u3aj2r/). The evidence points the other way on the vet. Vets object to owners **having** charcoal: \"I bought activated charcoal as precaution for poisoning situations. But my vet didn't like the fact that I bought it.\" (customer_report, https://www.facebook.com/groups/514612959043998/posts/2623712288134044/). \"My vet said please don't use that she could aspirate the charcoal in her lungs and get pneumonia so I returned it.\" (customer_report, https://www.amazon.com/gp/customer-reviews/RXIWHMIQJDOQL). |
| F4 | \"The $3,000 choice\": $2,500 on a card, an impossible decision. \"81%\" | **Fear of cost supported. The $2,500–3,000 figure is above most reported bills. \"81%\" not yet tested.** | See P4 and B6. Borrowing: \"Thank goodness I had someone I could borrow the money from\" (kzmwje). Hold-for-payment: \"the vet wouldn't see her UNLESS WE PAID THE $75 CONSULTATION FEE OVER THE PHONE\" (utaup0). |
| F5 | Having to tell the kids | **Not yet tested** | No evidence. |

### 5.3 Relationships (Section 5)

| # | Point | Verdict | Evidence |
|---|---|---|---|
| R1 | The partner thinks she's \"too dramatic\" | **Not yet tested** | Closest is a different family member holding back the vet: \"my mom won't let me go to the vet and take her unless she starts vomiting\" (customer_report, YouTube eKRzJ3sxUlc, lc=UgzRUtH4JE2DRHrPvqF4AaABAg). |
| R2 | Children finding the dog | **Not yet tested** | none |
| R3 | Shame in front of the vet or vet techs | **Contradicted in direction** | See F3. |
| R4 | Mother-in-law: \"spends too much on the dog\" | **Not yet tested** | none |
| R5 | Facebook pet groups as the place she worries | **Supported in part** | Owners post in groups in the middle of the emergency, and the threads are large: the Hershey's post has 283 reactions and 595 comments (Swann). Owners also turn to groups for dosing (Glaeser) and for whether a product is legitimate (Graziano). No \"I lost my dog last night to chocolate\"-type post was found. Report 03 §4.7 suggests (hypothesis) that crowdsourcing in the group may stand in for the hotline. |

### 5.4 Hurtful things people say (Section 6)

| # | Point | Verdict | Evidence |
|---|---|---|---|
| H1 | Best friend: \"I'm sure it's fine — it was probably just a little piece\" | **Supported** | \"Dogs can eat more chocolate than you'd think, I'm sure he will be fine!\" (comment or1v1ms, https://www.reddit.com/r/Pomeranians/comments/1u31u8h/). |
| H2 | Partner: \"dogs eat weird stuff all the time. He'll be fine.\" | **Supported in category** (not from a partner) | \"My Wally ate probably 10 or so miniature chocolates… and he was fine.\" (comment or3yz9y, 1u31u8h). \"That told me either the chocolate and dogs is a myth or the chocolate cake was fake\" (YouTube eKRzJ3sxUlc, lc=UgxrkDqCW231F_CpI-V4AaABAg). |
| H3 | Emergency vet: \"If you had administered activated charcoal at home within the first hour… Was there nothing you had on hand?\" | **Contradicted** | \"So weird my dog ate chocolate and the emergency vet clinic said inducing vomiting at home or giving charcoal at home weren't recommended. 🙄\" (customer_report, YouTube Mtx6oLVVJ7k, lc=UgzG20pNmRcyo4zF1nJ4AaABAg). \"They don't want him throwing up toxiban bc it can cause more problems.\" (customer_report quoting the vet, comment or1wbel, 1u31u8h). \"as a vet assistant never give this without consulting a vet first! charcoal can cause dangerous electrolyte imbalances!\" (pro_opinion, 2,533 likes, TikTok melissa_fergus/7489845283237465375, cid 7504847248652600095). |
| H4 | Mother-in-law: \"maybe if you spent… more time pet-proofing\" | **Supported in part** (the pet-proofing jab, from strangers) | \"don't leave ur stuff out lmao then u won't have this issue\" (TikTok jeremysfinds, cid 7546489362982404878). |
| H5 | Facebook stranger: \"every responsible pet owner should have activated charcoal… that's on you\" | **Supported only as affiliate content** | \"Everyone should have activated charcoal on hand for an emergency.\" This is **competitor_claim**: an affiliate post with amzn.to links that also says \"Do not administer activated charcoal unless instructed.\" (https://www.facebook.com/groups/DuncanStrong/posts/2037119440351932/). No owner was found saying it. |

### 5.5 Past solutions tried (Section 7)

| # | Point | Verdict | Evidence |
|---|---|---|---|
| S1 | Frantic Googling, where \"half the sites said induce vomiting. The other half said don't\" | **Supported** | \"he is acting fined but when i google it is sayin take him to vet right now\" (customer_report, https://www.facebook.com/groups/lynchburgrecommendations/posts/1964171084555916/). \"My vet said it was safe at that dose but I've read a lot online that says otherwise.\" (comment op5u0xe, 1ttxg2h). |
| S2 | Hydrogen peroxide, then fear of burns and crying on the way to the ER. \"completely unsafe for cats\" | **Fear supported. Peroxide also succeeds for some (contradiction). The cat point is not yet tested by owner voice.** | \"I did not know it was corrosive to their stomach lining so now I'm worried it's sitting in there.\" (1ttxg2h). \"I'm nervous that both the peroxide and chocolate will end up poisoning her.\" (1ld0da7). \"I woke up to find that he had thrown up blood\" (Tier B, r/DogAdvice 175ezey kj2xjt3). Success: \"moments later, everything is all over the yard… She was fine.\" (comment k9nxh9x, 17xefh8). Vet staff: \"Hydrogen peroxide is no longer really recommended\" (Tier B pro_opinion, r/AskVet 1n5cwt8). There are no cat peroxide reports. |
| S3 | ASPCA hotline: credit card first, \"$95 per call\", then on hold | **Supported, with a fee caveat** | \"poison control charged us $95 when they finally picked up to tell us that he should be fine.\" (https://www.reddit.com/r/DobermanPinscher/comments/1anrg6x/). \"ASPCA wants to charge $95 (lol)\" (https://www.reddit.com/r/AskVet/comments/126bjlc/). \"the poison contol hotline is $95 upfront\" (comment my4m6lw, https://www.reddit.com/r/AskVet/comments/1ld0da7/). **Caveat:** the newest posts quote other amounts: \"ASPCA was 110 USD while Pet Poison Helpline was 89 USD.\" (2025-10-14, 1o68fek); \"$110 fee\" (2026-10-27, https://www.reddit.com/r/AskVet/comments/1xgibir/); \"$85.00\" (2026-05-07, 1t6mhey). |
| S4 | A \"$2,000+\" ER visit at midnight, where \"They gave her activated charcoal… Something I could have given her at home\" | **Supported in part** | The ER does give charcoal: \"They gave her apomorphine for her to puke everything up… fluids… and charcoal to prevent any more absorption.\" (utaup0, $400). The \"saved me\" belief: \"This would've saved me 2 grand 😅\" (TikTok, above). **But** the bill is usually lower (P4), and the ER does more than give charcoal: apomorphine, fluids, bloodwork, \"activated charcoal with sorbitol (charactol 50)\" (https://www.reddit.com/r/AskVet/comments/1w1t0q4/). |
| S5 | Pet insurance: \"Insurance is money AFTER\" | **Not yet tested** | The P4.9 insurance question was bought but sits among the 126 unread answers (telegram report 02 §6). |

### 5.6 What they don't want to do (Section 8)

| # | Point | Verdict | Evidence |
|---|---|---|---|
| W1 | Force their pet to vomit | **Supported in part, with a contradiction** | \"I was apprehensive about giving him hydrogen peroxide, though, knowing that it can sometimes do more harm than good, and he's a senior dog\" (Tier B, r/WagWalker 1ofbfib). **But** many owners actively want to induce: \"Should I induce vomiting?\" (Facebook, above). \"we induced vomiting and gave activated charcoal\" (Lunning, above). |
| W2 | No mixing, measuring or maths in a panic | **Supported** | See P6, plus \"so that in an emergency (when my anxiety turns my brain to mush) I don't have to fumble around for it\" (YouTube xG1nLBTzPDo, lc=UgxQ3qhsMdCkh75Ol8B4AaABAg). |
| W3 | Don't sit on hold | **Supported** | \"On a small animal, that kind of wait time is a death sentence.\" (1t6mhey). \"In some cases, I hung up before speaking to someone because I *had* to find someone who would help, NOW.\" (1t6mhey). |
| W4 | Don't pay \"$2,000 for a vet to administer the same thing… for twenty bucks\" | **Supported in part. Internal contradiction.** | \"trust me if the vet administrator activated charcoal it will Cost $$$$.\" (https://www.amazon.com/gp/customer-reviews/RP39F77QYNIHQ). \"saves me from extra vet costs!\" (https://www.amazon.com/gp/customer-reviews/R3F533BNXABN7N). **The profile contradicts itself:** \"twenty bucks\" here, \"$40\" in Section 8 #5, and the real price is $39.95 (`product_truth.md`). For \"the same thing\", see S4. |
| W5 | Finding out about the product only after an emergency | **Supported in part** | Learning mid-emergency that they don't have it: \"I can't wait till Sunday.\" (10hdn3j). \"I can not find activated charcoal in the stores anywhere.\" (Runk). No one says they found out at the vet. |

### 5.7 Transformation and outcomes (Sections 9–11)

| # | Point | Verdict | Evidence |
|---|---|---|---|
| T1 | \"The Drawer of Control\", peace of mind | **Supported** | \"Hope I never have to use it.\" (https://www.amazon.com/gp/customer-reviews/R2XVLZVD62VWS5). \"Haven't Needed It—But So Glad We Have It\" (https://www.amazon.com/gp/customer-reviews/RV6VX2KD4A8PS). \"kind of an EpiPen for your curious ones\" (https://www.amazon.com/gp/customer-reviews/RNEFT86O01SYV). All three are reviews of competitor products. |
| T2 | Being the person who acted (\"set the dial to her weight\") | **Supported** for acting. The dial is product description, not tested. | \"I immediately grabbed the Pawmergency from my purse and gave it to him… we avoided a trip to the vet!\" (customer_report about the **PawMergency** product, https://www.amazon.com/gp/customer-reviews/RU0M4MDBVULVD). **Note:** our page reuses this review word for word with \"Petmergency\" swapped in (report 05 §6). |
| T3 | Buying time, then the vet (\"Not a guarantee. A fighting chance.\") | **Supported.** Fits the \"charcoal plus vet\" framing. | \"I gave her the activated charcoal and rushed her to the emergency veterinary hospital where the treatment was completed and she was released the next morning.\" (https://www.amazon.com/gp/customer-reviews/RIFGTSSJTXYV1). \"Update, I will have it on hand if the time comes that the vet says so.\" (Mangels, above). |
| T4 | The $2,000 bill that never happened; the vet says \"you did the right thing\" | **Avoided cost supported. Vet praise not found and contradicted by vet pushback (H3).** | \"unlike the first time, he showed absolutely no symptoms… saved us from what could've been an extremely high vet bill.\" (https://www.amazon.com/gp/customer-reviews/R98C0V79UQ94X). |
| T5 | Identity upgrade: friends ask her for the link | **Supported by 1 report** | \"A friend of mine suggested keeping this on hand\" (R3V0WAMC78GXMM). Only one report, so this is below the two-report bar. |
| T6 | Section 10: anxiety softens, she becomes \"the responsible one\", her partner converts, she stops feeling like a fraud, she tells the story everywhere | **Not yet tested** (anxiety softening is covered by T1) | No partner, fraud or storytelling evidence. |
| T7 | Section 11 vet soundbite: \"Administering activated charcoal within the first hour was the difference\" | **Contradicted** | See H3. |
| T8 | Section 11 Facebook group: \"How did you know the dose?\" | **Supported** (dose questions in groups) | \"How much do I give a 60 pound pit and a 37 pound Pittie mix.\" (Glaeser, above). |

### 5.8 Market specifics (Section 12), search words and subreddits

| # | Point | Verdict | Evidence |
|---|---|---|---|
| M1 | \"This market doesn't lack information… They know vets use activated charcoal\" / \"The problem isn't knowledge\" | **Contradicted** | Owners don't know how or when charcoal works: \"I have activated charcoal and I know it's suppose to be used if he eats poison but is that it?\" (https://www.facebook.com/groups/holisticandnaturalpets/posts/4520364248227111/). \"How does this work, and should I be doing more?\" (1w1t0q4). Some believe charcoal makes the dog vomit: \"Gave correct amount to my puppy… But he never threw up\" (https://www.amazon.com/gp/customer-reviews/R22OQU9696DWL7); \"the vet have to use activated charcoal to induce vomiting\" (groomer, https://www.facebook.com/groups/1542021025906490/posts/27993132663701966/). |
| M2 | \"The gap between knowing and having\" | **Supported** | See C1 and W5. |
| M3 | Who they blame: themselves | **Supported** | See E2. |
| M4 | Who they blame: the vet industry and the system (\"Why is an emergency vet visit $2,000?\") | **Supported, aimed mainly at the hotline fee** | \"Like 10-20 would be way more reasonable, considering the human one is free.\" (kzmwje). \"But damn $95 is just crazy\" (comment kpunp6j, 1anrg6x). |
| M5 | Who they blame: the pet, affectionately | **Supported** | \"My littlest dog is a garbage disposal and will eat ANYTHING I drop on the ground.\" (comment k9n4vli, 17xefh8). \"Not his first time. Won't be his last time. 🙄😒\" (1t6mhey). |
| M6 | Who they blame: online misinformation about peroxide | **Supported in part** | See S1 (op5u0xe). No owner says the safe option is \"buried\". |
| M7 | \"My vet has never once mentioned I should have activated charcoal at home\" | **Contradicted in direction** | Vets do raise it, mostly against: see F3 and H3. |
| M8 | \"What they must give up\" (the \"couldn't have known\" excuse, the victim narrative, procrastination) | **Not yet tested** | none |
| M9 | Search words: dog ate chocolate / grapes / rat poison / ibuprofen, cat ate lily, activated charcoal for dogs, peroxide to make dog vomit, emergency vet bill | **Supported for all 8 as real situations** (grapes and ibuprofen 1 report each) | See C2, P2, P4. **Negative evidence:** on TikTok, \"dog ate chocolate\" returned no results in the mix (report 02 §9). **Owners' own words not in the list:** \"poison control fee\", \"toad\", \"Toxiban\", \"VetDTox\", \"how much do I give\", \"when do you know when to administer\". |
| M10 | Subreddits AskVet, dogs, DogAdvice, puppy101, cats, CatAdvice, Pets | **Supported for AskVet, DogAdvice, puppy101 and Pets. r/CatAdvice returned 0. r/dogs and r/cats: titles only.** | Telegram report 02 §6, rows 7–13. Productive subreddits outside the list: r/DobermanPinscher (1anrg6x) and r/Pomeranians (1u31u8h). |

### 5.9 Objections (Section 12, top 5)

| # | Objection | Verdict | Evidence |
|---|---|---|---|
| O1 | \"I should probably just call my vet\" | **The objection is supported. The profile's rebuttal (\"doesn't survive contact with reality\") is contradicted in part.** | Calling the vet does fail: \"I tried to call a few vets, but they didn't answer, any of them.\" (1u3aj2r). \"the vets I called can't legally give advice\" (YouTube v-k4ezLEkLU, lc=UgzWLMdzWv_UHGrXhVt4AaABAg). **But** the strongest voices say call first: \"do not give unless instructed by a vet or poison control\" (TikTok, cid 7501794719468471082, 65 likes). ERs often require the hotline call: \"the emergency vet won't work with us until we connect with poison control\" (1anrg6x). |
| O2 | \"What if I make it worse?\" | **Supported (strongly)** | \"I fear she inhaled a little of it via her mouth or am I exaggerating? I don't want to do her more harm than good\" (https://www.reddit.com/r/AskVet/comments/1df54i1/). \"I'm worried about the adverse effects of activated charcoal.\" (irkjyg). \"activated charcoal should not be given dry because they can aspirate it into their lungs\" (18l9sv8). **The profile's answer, \"The Dial-A-Dose system is the direct antidote\", is not tested,** and our page's dose guidance contradicts itself (`product_truth.md`; report 05 §5 row 9). |
| O3 | \"My pet has never gotten into anything toxic\" | **Supported in a different form** (\"it'll be fine\" / \"it's a myth\") | See H1 and H2. The \"451,000\" answer is not tested (C3). |
| O4 | \"Is it safe to buy something like this online? Shouldn't I get this from a vet?\" | **Supported** | \"ya i don't trust any pet products that come from the internet and not the vet🥹\" (TikTok frugal__living/7493593664329944350, cid 7493975684151837486, 78 likes). \"Before I take the bait - does anyone know if it's legitimate?\" (Graziano, about **Vetanica** ads). \"my vet didn't like the fact that I bought it\" (Dupont). **The profile's answers (\"vet formulated\", \"third-party tested\", \"Made in USA\", \"ASPCA-aligned\") are all unverified seller claims (§5.11).** Our page's copied PawMergency testimonials (report 05 §6) would make this objection worse if found. |
| O5 | \"$40 feels like a lot for something I'll probably never use\" | **Supported** | \"Why isn't this cheaper??\" (TikTok mm336777, cid 7503171397475222318). \"You can buy activated charcoal, much cheaper\" (TikTok muonline_pc, cid 7524865301285421854, 106 likes). \"don't buy this overpriced product bruh they be charging 60$ for a 10 dollar product\" (cid 7566770548093895437). Market data (competitor_claim / listing data, report 02 §5): **PawMergency $36.99, PetVet Medic $24.99, powder $15.59. SavePet at $39.95 is above every Amazon listing seen.** Counter: \"It's expensive but 100% worth the emergency use\" (R1PJXSAJA58WNE). That is the very sentence our page cut from the copied testimonial (report 05 §6). |

### 5.10 Numbers in the profile

| Number | Verdict | Note |
|---|---|---|
| 451,000+ ASPCA calls in 2024, one every 70 s, nearly 4% up | **Not yet tested** | Unsourced. Needs a primary source before any ad use. |
| $95 per hotline call | **Supported as the most common owner-reported fee, with a caveat** | Reported by 4 independent owners (S3). The full range is $40–$125, plus a $150 vet \"communication fee\" (telegram report 02 §7). The newest ASPCA mentions say $110 (2025-10, 2026-10). Treat $95 as \"a fee many owners report\", not \"the current ASPCA price\". |
| 38% can't cover an emergency without debt | **Not yet tested** | Unsourced. |
| 81% stressed by a bill under $2,500 | **Not yet tested** | Unsourced. |
| 82% say the pet is like their own child | **Not yet tested** | Unsourced. |
| $2,000 / $2,200 / $2,500 / $3,000 bills | **$2,000 has 1 Tier A report. $3,000 has 1 Tier B report. Most reported bills are $350–$600 (contradicted as typical).** | P4. |
| $80/mo food, $200 checkups, $50 treats; 25 minutes Googling; 40-minute drive; 2-hour wait | **Not yet tested.** Drive times seen elsewhere: \"(30min drive)\" (YouTube Mtx6oLVVJ7k, lc=UgxXCSUapCNwSmim4sZ4AaABAg) and \"nearly 2 hours away\" (1ld0da7). | Illustrative. |
| \"$40\" vs \"twenty bucks\" vs real price $39.95 | **Contradicted inside the profile** | W4. |

### 5.11 Claims in the profile

| Claim | Verdict | Note |
|---|---|---|
| \"Made in USA\" | **Not yet tested (unconfirmed)** | It appears on our page as \"Made in the USA \\| Third-Party Tested\" (competitor_claim, report 05 §4). The owner hasn't answered the question asked on Telegram at 16:12 and 16:16. Country of manufacture is NOT CONFIRMED in `product_truth.md`. Separately, the competitor PetVet Medic also claims \"Made in USA\" on Amazon (competitor_claim, report 02 §5). |
| \"Third-party tested\" | **Not yet tested (unconfirmed)** | Page badge only. No certificate has been seen. |
| \"Vet formulated\" | **Not yet tested** | Page badge only. |
| \"ASPCA-aligned credentials\" | **Not yet tested** | The page shows the ASPCA phone number and attributes an unsourced cat statement to the ASPCA (report 05 §5 row 3). No alignment has been documented. |
| Dial-a-dose: \"pre-dosed\", \"foolproof\", \"set the dial to her weight\" | **Not yet tested.** The page's dose guidance contradicts itself. | `product_truth.md`: \"dosed 1 mL per lb… page dose guidance is internally inconsistent\". |
| \"Trapping\" the toxin in the first hour (mechanism and timing) | **Not yet tested** | Clinical, block 2 territory. Our page's own timing claims disagree with each other (C5). |
| Charcoal at home is \"the same thing\" the ER gives | **Not yet tested.** The evidence shows ERs do more (S4). | Hypothesis at best. |
| Peroxide \"can burn your dog's esophagus or kill a cat\" | **Esophagus: supported only by Tier B pro_opinion. Cats: not yet tested.** | \"It can frequently cause abrasions and ulcers in the esophagus and stomach\" (Tier B, r/AskVet 1n5cwt8, comment nbrs3od). |

---

## 6. Conclusions, hypotheses and contradictions to carry forward

**Conclusions (from the evidence above)**
1. **The six buyer problems all hold up.** Each has at least two independent owner reports. P5 (hotline fee and hold) is the strongest. The profile's **feelings** (dread, guilt, helplessness, money fear) also hold up.
2. **The profile's picture of the vet is backwards.** Three points (H3, T7, M7) have the vet wishing the owner had used charcoal at home. In the evidence, vets and vet staff mostly push back on home charcoal or peroxide without a call first. Owners' success stories describe **charcoal plus the vet**, not charcoal instead of the vet.
3. **\"The problem isn't knowledge\" is contradicted.** Owners are unsure what charcoal does, when to give it and how much to give, and some think it makes the dog vomit.
4. **Every percentage in the profile (38%, 81%, 82%) and the 451,000 figure is untested.** None can go into ads until a primary source is found. The $95 figure is real owner language, but the current ASPCA fee may be higher.
5. **The income and \"spends liberally\" picture doesn't match the many cash-strapped owners in the evidence.** Whether actual buyers are wealthier is untested.

**Hypotheses (not proven)**
- H-a. A \"call your vet or poison line, and have this ready while you do\" framing would draw less vet pushback than the profile's \"instead of the vet\" soundbites (see O1 and H3).
- H-b. A cash-strapped or rural sub-avatar (\"nearest vet is 2+ hours away\", \"can't afford the $90 call\") may be as large as the profile's devoted, affluent \"Jessica\".
- H-c. Buyers come in three moments: just in case, after a near-miss, and during the emergency. The profile covers only the second.

**Contradictions to fix**
1. **Product price:** the profile says \"twenty bucks\" and \"$40\". The page says $39.95.
2. **Our page vs the profile's trust answer (O4):** the page carries two PawMergency Amazon reviews presented as SavePet proof (report 05 §6).
3. **`PRODUCT_DECISION.md` is out of date.** It still says \"Brand spelling SavePet vs SavePets not confirmed\", but the owner confirmed SavePet at 16:40. I couldn't edit it in this run: the path lock allowed only this report, and the owner didn't ask for that file to change.
4. **Supermemory states two things too strongly:**
   - `XaWK8c9FcfjohKn44PKR61` says PawMergency \"sells the same product\". That sameness is a hypothesis.
   - `h9ZkhAPutRBf3svLfvKEUo` states the profile's buyer (\"mostly women aged 27 to 42\") as fact. It is untested (B1–B2).

   I didn't edit memories.

## 7. Ideas for the owner (not tasks; nothing was created, assigned or scheduled)

- **Commit Appendices A and B** through a job that is allowed to write those paths. This gateway job can write only this report. After that, the main repo's loose `SavePet PetMergency Avatar Profile.pdf/.txt` can stay as the original, as you asked.
- **Answer the two claim questions:** is \"Made in USA\" true, and is \"third-party tested\" true? If not, take them off the page and out of the profile's objection answers (O4).
- **Rewrite the profile's vet soundbites** (H3, T7, M7, F3) to match what owners actually report, or mark them clearly as aspiration, not evidence.
- **Find primary sources for 451,000 / 70 s / 4%, 38%, 81% and 82%,** or drop them from copy. Cite the hotline fee as an owner-reported range, not a single number.
- **Read the 126 paid, unread Reddit Answers** (datasets `edo30btIGF0NdPkvS` items 10–19 and `lPdySNS03gekOd6iv`) at $0. Start with P4.9 (insurance, S5) and the P1/P4/P6 items. That could move several \"not yet tested\" points.
- **Add the new owner search words** (M9) to `listening/SOURCES.md`, and swap r/CatAdvice for a lily-specific search.
- **Update `PRODUCT_DECISION.md`** to say the brand is confirmed as SavePet, and add the competitor candidates (PawMergency, PetVet Medic, Vetanica, NOW) if you agree.
- **Correct the two Supermemory memories** in §6.4, point 4.

## 8. Unavailable or failed this run

- **GitHub writes outside this report path:** refused by the gateway for `avatar/owner_avatar_profile.md` and for `product_truth.md`, with the same error each time. Both are staged below.
- **Course prompts:** the playbook registry is all `ADD_ID` and names no Supermemory space. None was needed or used.
- **ClickUp:** not configured and not used.
- **Apify:** not used ($0), as instructed.
- **Vantage:** not used. It gives ad structure only, never proof.
- **Telegram report 01 §5:** cut off in the tool output. It holds only questions, so this check doesn't depend on it.

---

## Appendix A: `01_petmergency_activated_charcoal_first_aid/avatar/owner_avatar_profile.md` (NOT COMMITTED; ready to commit)

> **Owner-written summary, not real customer posts.** This is a word-for-word copy of the owner's avatar profile, `SavePet PetMergency Avatar Profile.txt` (repo `exobvious/research`, root, file sha 10f11d229c895c18a30efcd2c30fcd108822b371). The original is left untouched in `exobvious/research`.
>
> - Its quotes are **illustrative**. They were written by the owner as examples, and no customer said them.
> - Its numbers are **unsourced**: 451,000 poison calls, $95 per hotline call, 38%, 81% and 82%.
> - **\"Made in USA\" and \"third-party tested\" are unconfirmed.**
> - For what the evidence supports or contradicts, see `bot_reports/telegram/2026-11-02/03-avatar-copy-and-check.md`.
> - Copy note: the original's Windows (CRLF) line endings are normalised to LF, and its tab-indented table cells may render as plain indentation. The words and punctuation are unchanged.

````text
🐾 PetMergency — ELITE BUYER PROFILE REPORT
________________


📋 SECTION 1: DEMOGRAPHIC SNAPSHOT
Field
	Detail
	Composite Name
	Jessica (primary) / Mike (secondary)
	Age Range
	Primary: 27–42 (Millennial) · Secondary: 43–55 (Gen X)
	Gender Split
	~65% Female / 35% Male
	Pet Profile
	1–3 pets (dog and/or cat); pet is a "fur baby" and full family member
	Household
	Renting or homeowner; may be childless-by-choice OR has both human children AND pets
	Income
	120,000/yr; spends liberally on pet care but feels exposed to large unexpected vet bills
	Psychographic Identity
	"Devoted pet parent" — 82% of this market says their pet is like their own child. Buys premium food, schedules regular vet checkups, posts pet content on social media. Being a good pet parent is a core piece of their identity.
	Key Behavioral Trait
	Reactive preparer. They don't think about emergencies until something almost happens — or does. One near-miss transforms them into a voracious buyer of protective products.
	________________


🚨 SECTION 2: THE CORE PROBLEM
Jessica's dog or cat could ingest something toxic at any moment — and she has absolutely nothing at home to do anything about it.
Chocolate left on the counter. Rat poison in the garage. A dropped prescription pill. Grapes in a low bowl. A toxic houseplant she didn't know about. The danger is everywhere, and one moment of inattention can trigger a full-blown crisis. In 2024, the ASPCA Poison Control Center responded to 451,000+ calls — one call every 70 seconds — a nearly 4% increase over the year prior. This isn't paranoia. It's statistical reality.
When it happens, the clock starts the moment the toxin goes down. Jessica doesn't have an hour to figure out what to do. She needs a plan right now. And right now, she has nothing.
The emotional gut-punch: she spends $80/month on premium dog food, $200 on annual vet checkups, $50 on organic treats — and she doesn't own a single thing that could save her pet's life in the first 60 critical minutes of a poisoning emergency.
________________


🔥 SECTION 3: TOP 5 MOST POWERFUL EMOTIONS
#
	Emotion
	Internal Narrative
	1
	Anticipatory Dread
	"Every time I leave the room, I have this low-level hum of 'what if.' What did she get into? Is that plant toxic? Did someone drop something on the floor?"
	2
	Guilt
	"If something happened to him and I had no way to help, I would never forgive myself. He trusts me completely. I'm supposed to protect him."
	3
	Helplessness
	"The most terrifying part isn't the emergency itself — it's knowing I'd just be STANDING THERE, panicking, Googling, crying, doing nothing while he suffered."
	4
	Financial Panic
	"38% of pet parents can't cover an emergency vet visit without going into debt. I'm one of those people. And the idea that money could be the reason I lose her makes me physically sick."
	5
	Protective Rage / Love-Driven Urgency
	"This is my family. If someone broke into my house, I'd act. This is no different. I need to be able to DO something. I refuse to be helpless."
	________________


😱 SECTION 4: TOP 5 DEEPEST FEARS
These are the thoughts they'd never say out loud — the dark spirals that hit at 3AM when the house is quiet.
________________


Fear #1 — The "I Was Right There" Nightmare
"My biggest fear is that something happens while I'm home — I'm literally in the same room — and I still can't do anything. I can't stop thinking about what it would look like to watch Biscuit seize on the floor while I'm frantically Googling, on hold with a hotline, trying to reach a vet who can't see me for three hours. Just me, frozen, and him suffering while I'm useless."
________________


Fear #2 — The "Too Late" Discovery
"What if I wake up in the morning and he got into something overnight, and by the time I find him it's been six hours? The toxin is already in his bloodstream. I had no idea. I was asleep. And now... it's just too late. There was nothing to do. That thought makes me nauseous."
________________


Fear #3 — Being Seen as a Negligent Pet Parent
"The worst part of an emergency vet visit isn't the bill. It's the look. That look from the vet that says 'why didn't you have anything at home? Why did you wait?' I spend everything on this dog. I love her more than most people I know. And I'd be the one who failed her because I just didn't think ahead."
________________


Fear #4 — The $3,000 Choice
"I think about it more than I should. What if they tell me it'll be $2,500 to treat her, and I have to put it on a card I can barely pay, or I have to decide between... I can't even finish that thought. 81% of pet owners would be financially stressed by a bill under $2,500. I'm in that group. And that terrifies me."
________________


Fear #5 — Having to Tell the People She Loves What Happened
"If I lost Coco to something preventable — something where a product existed, was sitting on the internet, cost less than my monthly streaming subscriptions, and I just never got around to it — how do I explain that to my 9-year-old? How do I live with that?"
________________


💔 SECTION 5: HOW THESE FEARS AFFECT KEY RELATIONSHIPS
Fear
	Relationship Affected
	Specific Impact
	Fear of helplessness during an emergency
	Partner/Spouse
	Jessica snaps when he leaves food on the low counter. She's constantly scanning the house for threats. The hypervigilance creates friction. He thinks she's "too dramatic." She feels utterly alone in her worry — like she has to be vigilant enough for both of them.
	Fear of the "too late" discovery
	Children (if applicable)
	She hasn't told her kids about pet poisoning because she doesn't want to scare them — but she plays out the scenario in her head: her 8-year-old finding the dog collapsed, not knowing what happened, screaming for mom. The image never fully goes away.
	Fear of being seen as negligent
	Vet / Vet Technicians
	She already feels mild shame every time she has to admit she didn't know something at a routine visit. The idea of bringing in a poisoned pet and being seen as the owner who "had nothing at home" is almost worse than the emergency itself.
	Financial panic
	Parents / In-Laws
	Her mother-in-law already thinks she "spends too much on the dog." If she had to call and ask to borrow $2,000 because her dog ate rat poison, she'd feel the full weight of every "it's just a dog" comment she's ever had to silently swallow.
	Fear of preventable loss
	Pet Parent Community Online
	She's in three Facebook pet groups. She's seen the posts — "I lost my dog last night to chocolate." She always thinks "that would break me." And she quietly wonders if she'd be the next person writing that post — knowing the whole time there was something she could have done.
	________________


🗣️ SECTION 6: HURTFUL THINGS PEOPLE MIGHT SAY
________________


👩 Her Best Friend (well-meaning, unaware of the depth of the fear)
"Oh my god, your dog got into the chocolate cake? Did you Google it? I'm sure it's fine — it was probably just a little piece..."
What Jessica hears: "I don't take this as seriously as you do. You're overreacting. You're alone in this."
________________


👨 Her Partner (trying to calm her, completely missing the point)
"Babe, dogs eat weird stuff all the time. He'll be fine. You don't need to buy every product on the internet."
He means well. But this makes her feel dismissed, unseen, and somehow MORE anxious — like she has to carry the weight of this fear alone.
________________


👩‍⚕️ The Emergency Vet (professionally neutral, emotionally devastating)
"If you had administered activated charcoal at home within the first hour, we likely wouldn't have needed to treat the secondary symptoms at all. Was there nothing you had on hand?"
She replays this sentence in her head for months.
________________


👵 Her Mother-in-Law (the antagonist, zero filter)
"You spent HOW much on the emergency vet? For a dog? Honey, I love that animal, but maybe if you spent less time spoiling it and more time pet-proofing your house..."
This one lands differently. Not because she agrees — but because a small, exhausted part of her wonders if there's a grain of truth in it.
________________


💻 A Stranger in Her Facebook Pet Group (the comment she can never unsee)
"Honestly, every responsible pet owner should have activated charcoal in the house. It's like a first aid kit. If you don't have one, that's on you. The vets use it for a reason."
She reads this. Feels the sting. Screenshots it. Closes the app. Opens it again.
________________


🔍 SECTION 7: PAST SOLUTIONS TRIED — AND WHY THEY FAILED
#
	Solution Tried
	Soundbite From the Prospect
	1
	Frantic Googling During an Actual Scare
	"I spent 25 minutes down a Google rabbit hole while my dog was right there looking at me. Half the sites said induce vomiting. The other half said don't. I was shaking and I still had no idea what to do. I felt completely useless."
	2
	Trying Hydrogen Peroxide to Induce Vomiting
	"I read it was the 'home remedy.' Then I read further and found out it can cause esophageal burns, internal bleeding, and is completely unsafe for cats. I'd literally just done that to my dog. I cried the whole way to the emergency vet, convinced I'd made it worse."
	3
	Calling the ASPCA Poison Control Hotline
	"They immediately asked for my credit card. $95 per call. I paid it — obviously. But I'm giving my card info while my dog might be dying, then I'm on hold, then they're telling me step-by-step what to do — and I have absolutely nothing in the house to actually DO any of it."
	4
	A $2,000+ Emergency Vet Visit at Midnight
	"We drove 40 minutes to the only 24-hour emergency vet. Waited two hours in the waiting room. The bill was $2,200. They gave her activated charcoal. ACTIVATED CHARCOAL. Something I could have given her at home. I wanted to cry."
	5
	Pet Insurance
	"I thought pet insurance would cover emergencies. And it helps — don't get me wrong. But it doesn't help in the MOMENT. It doesn't help at 11PM when my cat is foaming at the mouth. Insurance is money AFTER. I need something that works RIGHT NOW."
	________________


🚫 SECTION 8: WHAT THEY DON'T WANT TO DO TO FIX THE PROBLEM
#
	What They Don't Want
	Internal Soundbite
	1
	Force their pet to vomit
	"I've read too many horror stories. Hydrogen peroxide sounds like a solution until you find out it can burn your dog's esophagus or kill a cat. I need something that works WITHOUT putting my pet through more trauma."
	2
	Mix, measure, or calculate anything during a panic
	"I can barely do math when I'm calm. You expect me to stand there measuring milligrams while my dog is drooling and my hands are shaking? If I have to think hard to use it, I'll do it wrong. It has to be foolproof."
	3
	Sit on hold with a hotline during an emergency
	"I cannot be on hold. I cannot wait for a callback. Every minute counts. I need something I can grab from a drawer and use right now — not navigate a phone tree at 2AM while my pet is suffering."
	4
	Pay another $2,000+ vet bill for something they could've handled at home
	"I love my vet. But I don't want to pay $2,000 for a vet to administer the same thing I could have given at home for twenty bucks. That's the most avoidable thing in the world and I'm done letting it happen."
	5
	Find out about this product AFTER an emergency
	"The worst version of this story is sitting in the vet's office at midnight, watching them administer activated charcoal, and finding out this product existed the whole time. I'd rather spend $40 and never need it than live that moment."
	________________


✨ SECTION 9: THE MAGIC GENIE — PRIMARY TRANSFORMATION
If the perfect solution existed, here's what Jessica's life would look like:
________________


🌟 Outcome #1 — The Drawer of Control
"I want to walk into my kitchen, open the second drawer on the left, and know it's there. Just knowing that one tube exists — ready, pre-dosed, something I actually understand how to use — changes everything. I stop white-knuckling every moment I leave the house. The anxiety doesn't disappear, but it has a container. It has an answer. And that is worth everything."
________________


🌟 Outcome #2 — Being the Person Who ACTED
"In my worst nightmare, something happens and I'm frozen — Googling, crying, useless. In the version I want? I feel my heart drop, I reach for the tube, set the dial to her weight, and I DO something. I'm not waiting. I'm acting. I'm the thing standing between my dog and that toxin. That feeling — of being useful in the worst moment — that's everything."
________________


🌟 Outcome #3 — Buying Time, Not Just Hope
"I don't need a miracle cure. I just need a window — that first hour where the toxin is being trapped and I can get to the vet calmly instead of screaming into a phone at a call center. One hour of grace. That's what I'm buying. Not a guarantee. A fighting chance."
________________


🌟 Outcome #4 — The $2,000 Bill That Never Happened
"Imagine getting to the vet having already administered it at home, and they check her out and say 'you did the right thing — she's going to be fine.' No overnight stay. No IV drip. No invoice that makes me feel sick for a week. I just handled it. Like a prepared adult who took responsibility. Twenty dollars saved me two thousand. That's the story I want."
________________


🌟 Outcome #5 — The Identity Upgrade: The Prepared Pet Parent
"I want my friends to think of ME when their dog eats something. I want to be the one who says 'I have PetMergency — here's the link' — and they look at me like I'm the most responsible, loving, prepared pet parent they know. Not to show off. Because I genuinely gave a damn and thought ahead. And now everyone's pet is safer because of me."
________________


💫 SECTION 10: HOW THE TRANSFORMATION AFFECTS THEIR LIFE
This is the fantasy — raw, vain, and deeply human. The real emotional drivers they'd never admit out loud.
* The low-level anxiety softens. She stops white-knuckling every moment she's away from home. She can sit through dinner at a restaurant without her leg bouncing. The tube in the drawer is the psychological off-switch for a fear she didn't even realize was running 24/7.

* She becomes the "responsible one" in her circle. She's the one who sends the link in the group chat. She's the one whose pet survived. People ask her for advice now. The feeling of being the expert, the prepared one, the one who has it together — it's quietly intoxicating.

* Her partner's skepticism turns into open acknowledgment. "You were right. I'm glad you got this." Four words she's been waiting to hear about 100 different decisions.

* She stops feeling like a fraud. She spends premium money on her pet — organic food, vet checkups, birthday cakes from the specialty bakery. But there's always been a nagging voice: "Am I actually a good pet parent, or do I just buy the cute stuff?" Having PetMergency in the drawer is the answer. It's proof. It's the line between the performative pet parent and the truly prepared one.

* She tells the story everywhere. "So Max got into the rat poison left by the previous tenant — and I had this thing, PetMergency, right in the kitchen drawer, and I just..." People lean in. People pull out their phones. People buy it before they leave the room.

________________


🗣️ SECTION 11: POST-TRANSFORMATION SOUNDBITES
________________


👩 Her Best Friend (Supporter — completely converted)
"Oh my GOD. You literally had it ready to go? You just used it, and he's totally fine?? Send me that link right now. While we're standing here. Send it."
________________


👨 Her Partner (Former Skeptic — Now Converted)
"Remember when I said you were buying too much stuff for the dog? Don't say anything. I know. I'm just really glad you had it."
________________


👩‍⚕️ The Vet (Professional Validation She Always Craved)
"You did exactly the right thing. Administering activated charcoal within the first hour was the difference here. Honestly, if you hadn't had this at home, we'd be having a very different conversation right now. More pet parents need to know this exists."
________________


👵 Her Mother-in-Law (The Antagonist, Forced to Pivot)
"Well... I have to admit, I'm impressed. You handled that really well. Maybe I should get one of those for when Sophie brings her dog over..."
________________


💻 The Facebook Pet Group (The Chorus She Always Wanted)
"Can you share what you used? My vet just mentioned activated charcoal for home emergencies. How did you know the dose? Is he okay? You SAVED him. You're an incredible pet parent."
________________


🔥 The Person She Was Proving Wrong (The Internal Victory — No Words Needed)
 She doesn't need anyone to say a thing. She just knows. She thought ahead. She acted. Her dog is alive. That's the whole story.
________________


📊 SECTION 12: MARKET SPECIFICS
________________


What Does This Market Hinge Their Success On?
Having the RIGHT tool physically present in their home at the moment of crisis.
This market doesn't lack information. They've Googled pet poisoning. They know the ASPCA hotline exists. They know vets use activated charcoal. What they're missing is the physical object in the drawer — pre-measured, ready in seconds, zero friction.
Their core belief: "If I had the right thing on hand, I could save my pet. The problem isn't knowledge — it's the gap between knowing and having."
The sale is made on the promise of preparedness, not the product mechanism. What they're really buying is the identity of the prepared pet parent and the peace of mind that comes with it.
________________


What Does This Market Have to Give Up?
Hidden Psychological Payoff of NOT Having It
	What They Must Surrender
	The "I couldn't have known" excuse — without a product in the house, they can tell themselves it wasn't their fault if something happens
	Once they buy it, they own the responsibility. Having it means being accountable.
	The victim narrative in pet groups — posting "I had nothing at home and didn't know what to do" generates enormous community sympathy
	Being prepared is quieter. There's no dramatic story to tell if the crisis was calmly handled at home.
	The low-stakes version of pet parenthood — if they never face a crisis, they never have to know how far they'd really go
	Buying the product means accepting that crises will happen. It makes the threat real.
	The comfort of procrastination — "I'll deal with it when I need to" is its own coping mechanism
	Action requires confronting the fear. It's easier to stay numb to it than to plan for it.
	________________


Who Does This Market Blame?
Blame Target
	The Story They Tell
	Themselves (Pre-emptively)
	"I should have known. I should have pet-proofed better. I looked away for two seconds." Self-blame is the #1 emotional currency of this market. It's why guilt-based messaging is so potent here.
	The Vet Industry / Healthcare System
	"Why is an emergency vet visit $2,000? Why isn't this product pushed at every vet office? Why did nobody ever tell me this was an option?"
	Their Pet (Affectionately)
	"She literally cannot help herself. She's a dog. She would eat a sock and a chocolate bar at 2AM if I left them out. I can't control her curiosity — I can only be ready."
	Dangerous Online Misinformation
	"The hydrogen peroxide thing has been on the internet FOREVER. I almost followed that advice. Why is the dangerous option the first thing that comes up, and the safe option is buried?"
	A System That Never Prepared Them
	"My vet has never once mentioned I should have activated charcoal at home. Nobody mentioned it at the shelter when I adopted. I had to find this out the hard way. The system just assumes you'll panic, bring them in, and pay whatever it costs. Conveniently."
	________________


Top 5 Biggest Objections
#
	The Objection
	The Real Emotional Root
	1
	"I should probably just call my vet if something happens."
	Comfort in familiar systems. But this collapses the moment they imagine it's 11PM on a Saturday and the vet is closed. The objection doesn't survive contact with reality.
	2
	"I don't know if I'd use it correctly — what if I make it worse?"
	Fear of doing more harm than good in a panicked state. The Dial-A-Dose system is the direct antidote to this — but the fear must be pre-emptively named and neutralized in copy.
	3
	"My pet has never gotten into anything toxic, so hopefully we're fine."
	Classic normalcy bias. With 451,000+ ASPCA calls in 2024 alone — one every 70 seconds — this "it won't happen to me" thinking needs to be gently but firmly punctured with real numbers.
	4
	"Is it safe to buy something like this online? Shouldn't I get this from a vet?"
	Credibility and trust concern. This is precisely why the "vet formulated," "third-party tested," "Made in USA," and ASPCA-aligned credentials are non-negotiable conversion elements.
	5
	"$40 feels like a lot for something I'll probably never use."
	The psychology of paying for insurance you hope to never claim. The reframe is powerful: you're not buying a product. You're buying the peace of mind that you're the kind of pet parent who was ready.
	________________


This buyer profile represents a deep-dive synthesis of real, observable market psychology — built exclusively for advertising strategy, copy development, and funnel architecture purposes.
````

---

## Appendix B: proposed `01_petmergency_activated_charcoal_first_aid/product_truth.md` (NOT COMMITTED; replaces sha a2a4a93)

The only change is a new **Brand** section and a change-log line. Every other line is unchanged, and no other product claims were added.

````markdown
# PetMergency Activated Charcoal First Aid Kit: product truth

From the onboarding form, 2026-11-02. Research facts stay real: anything not given is MISSING until the label or supplier confirms it.

## Brand
- **SavePet.** Confirmed by the owner on Telegram, 2026-11-02 16:40 UTC: "SavePet is the brand." (`00_rules_and_process/telegram_log/2026-11-02.md` in exobvious/research)
- **Page problem to fix (not only a typo):** the product page https://savepet.co/products/petmergency also shows "SavePets" ("Try SavePets →", "Why SavePets Stands Out") and the domain "savepets.co" ("PetMergency is only sold here at savepets.co"). The store domain is savepet.co. These are errors on the page. Source: page capture 2026-11-02 19:20 UTC, Apify dataset `k6m5i9PoGnUih17tH` (bot_reports/onboarding/2026-11-02/05 §4 and §5 row 15).
- **The page also uses the name "PawMergency" in places** (cat FAQ: "PawMergency is formulated for both dogs and cats."). PawMergency is also a **separate brand** selling a similar activated charcoal first aid kit on Amazon ("PawMergency – Activated Charcoal First Aid Kit", ASIN B0FXBQSFJP, $36.99, 687 reviews, seen 2026-11-02; onboarding report 02 §5), and two page testimonials match PawMergency Amazon reviews word for word (onboarding report 05 §6). So the PawMergency name on our page is a page problem to fix, not just a typo. Whether SavePet and PawMergency are the same goods is NOT CONFIRMED (hypothesis for the supplier).

## Variants
- 1 tube - $39.95 (shown as down from $80)

## Label / ingredients (verbatim)
Named on page: coconut shell activated charcoal and kaolin clay. Full ingredient list, amount per mL and tube volume NOT CONFIRMED.

## Look (colour, texture, packaging)
Tube with a dial-a-dose mouth applicator, dosed 1 mL per lb of pet weight (per product page; page dose guidance is internally inconsistent).

## Size and supply per unit
NOT CONFIRMED: lead time and country of manufacture unknown. Bundle prices for 2-5 tubes unknown.

## Supplier / SKU
NOT CONFIRMED: store lists "My Vereli"; owner to confirm whether this is the maker.

## Product page
https://savepet.co/products/petmergency (store: savepet.co)

## Change log
- 2026-11-02 (telegram step 03): added the Brand section (owner-confirmed SavePet; SavePets / savepets.co / PawMergency flagged as page problems). No other product claims added or changed.
````
