# PetMergency Activated Charcoal First Aid Kit (SavePet): all research so far, in one document

- **What this is:** a compile step. It gathers everything in the 9 SavePet reports written so far, plus `product_truth.md` and `PRODUCT_DECISION.md`, into one readable file.
- **Run:** telegram / 01-all-research-in-one-document, written 2026-11-06 (UTC), cloud research agent.
- **Repo / folder:** `exobvious/savepet-research` / `01_petmergency_activated_charcoal_first_aid/`
- **Spend for this step: $0.00.** I did not call Apify, Vantage or any other paid source, and I opened no new threads. Every quote below comes from a report already in the repo.
- **No ClickUp tasks were created.** Next steps are written as ideas only.
- **Labels used throughout:**
  - `customer_report`: a pet owner talking about their own pet.
  - `pro_opinion`: someone who says they are vet staff, or a peer giving advice. Not verified.
  - `competitor_claim`: what a seller or affiliate says, including our own product page.
  - `hypothesis`: an idea to test. Not proven.
  - `conclusion`: something a report could check directly from its sources.
  - `owner's summary`: lines from the owner's avatar profile. These are not customer evidence.
- **Tier A / Tier B (Reddit only):**
  - Tier A: read in the opened thread itself, with a date.
  - Tier B: a short excerpt with a permalink, taken from a Reddit Answers answer. The thread was not opened and the date is unknown. Treat as unverified.

### Files I could not read in full (no guessing about the missing parts)

Three source reports were cut off by the tool when I read them. Repo search returned 0 hits for text from the missing parts, so I could not recover them.

1. **`telegram/2026-11-02/01-reword-reddit-questions.md`**: cut off from partway through question P5.8 to P6.2 in the 156-question list. Earlier runs hit the same cut.
2. **`telegram/2026-11-02/03-avatar-copy-and-check.md`**: cut off from partway through point W5 to the end of the owner's profile text in Appendix A. I can see **49 of the 66 profile points**. The other 17 (W6 onward, including the profile's objections) are not readable. The 2026-11-05 report hit the same limit.
3. **`telegram/2026-11-05/01-read-unread-reddit-answers.md`**: cut off from item P6-13 through the start of its §5 table. **Not readable:**
   - the rest of the P6 items
   - **all of its P2, P3 and P5 kept items**
   - its §3 drop counts
   - the first rows of its avatar-update table

   Where those items are named elsewhere in the report (§5–§7), I quote only the fragments shown there and mark them as fragments.

Everything else was read in full:
- `product_truth.md`
- `PRODUCT_DECISION.md`
- onboarding reports 01–05
- telegram report 02 (2026-11-02)
- `raw/README.md`

**The raw research / category document does not exist yet.** `raw/` holds only its README ("Raw pulls, saved verbatim with links. Never edited."), and no `EB_CATEGORY_CONTEXT_*` file is in the folder. The quote banks live inside the reports.

### Duplicate quotes merged

Many quotes appear in more than one report:
- Telegram report 03 (the avatar check) collected no new quotes. It re-cites quotes from onboarding 02 and 03 and from telegram 02.
- Onboarding reports 04 and 05 also re-cite quotes from 02 and 03.

**By my count, 101 distinct quotes appear in two or more reports.** This document shows each one once, at its first source, with a link.

The 2026-11-05 report also found the same quote under different permalinks 5 times. It kept 2 with both links and dropped 3. Those 2 sit in its truncated part, so they are not repeated here.

---

## 1. One-page summary

### The most important findings

1. **Two "Verified Buyer" testimonials on our product page are word-for-word copies of Amazon reviews of a competitor, PawMergency (ASIN B0FXBQSFJP).** `conclusion`, onboarding 05 §6.
   - One copy has "Pawmergency" changed to "Petmergency".
   - The other has its price complaint taken out.
   - The page also uses the name "PawMergency" in the cat FAQ, and it says "WE DO NOT SELL ON AMAZON … Beware of fakes on Amazon".
   - This is the biggest risk found so far.
2. **Vets and vet staff push back hard on home charcoal and home peroxide, and owners repeat what their vets tell them.** The top comment on a 1.27M-view TikTok (2,533 likes) reads: "as a vet assistant never give this without consulting a vet first! charcoal can cause dangerous electrolyte imbalances!"
   - Owners report their own vets saying no (aspiration, "didn't like the fact that I bought it").
   - Across all reports, **no owner tells a success story about charcoal given at home without a vet involved.** Success stories are about charcoal given by the vet, or charcoal plus a trip to the ER.
3. **The poison control fee and hold time is the strongest, best-backed pain.** Owner-reported fees run from **$40 to $125**, and **$95** is the most common single figure.
   - Holds: 15–20 minutes, 35+ minutes, 1.5 hours and 2 hours.
   - Example: "It costs $85.00 on my credit card to even be put through to Animal Poison Control." (r/AskVet, 2026-05-07)
   - Many ER vets won't treat until there's a poison control case number.
4. **The "vet closed at night" problem is real, and "the nearest vet is hours away" comes up just as often.** Rural owners with no ER nearby may be a separate buyer group (`hypothesis`).
5. **"$2,000 emergency bill" is not the typical figure.**
   - Poisoning bills owners report mostly run **$350–$600**, with some at **$2,400–$2,500** and one Tier B "3 grand".
   - Entry and after-hours fees ($500 admission, "$700 just to walk in the door", $900) and "pay up front, insurance pays you back later" come up often.
6. **Owners panic about *how much* and *when*,** not just whether to act.
   - Some pay the hotline mainly to learn the amount: "They changed me $95 before they would tell me how much hydrogen peroxide to give him to make him vomit."
   - A competitor's powder "didn't say anything about how to serve it."
   - Our own page gives conflicting dose and timing guidance, which needs fixing first.
7. **Nobody on Reddit mentions SavePet, PawMergency or PetVet Medic.** Every product-specific customer quote is about another brand (PawMergency, PetVet Medic, Toxiban, VetDTox, NOW, generic powder, Vetanica).
   - SavePet at **$39.95 is the highest price seen.** PawMergency sells at $36.99 on Amazon, PetVet Medic at $24.99, and generic tubes at $9.99–$16.60.
   - Price objections are common: "they be charging 60$ for a 10 dollar product".
8. **The cat claim on our page is contradicted.** The page says "For cats, this is the only safe at-home option … the ASPCA confirms no safe alternatives." A TikTok comment with 575 likes says "NOT SAFE FOR CATS". **Do not use the cat claim.**

### Biggest risks

- **Fake or borrowed testimonials** (finding 1). Review rules generally require testimonials to be genuine and about the product being sold. This is a compliance risk for the owner to review, not a legal conclusion.
- **Unproven page claims,** all locked as seller claims in `PRODUCT_DECISION.md`:
  - "#1 Vet Recommended", "60,000+ Pet Lives Saved", "Made in USA", "Third-Party Tested"
  - the named DVM and the ® mark
  - "No Vomiting" and "wide safety margin"
  - "100% Activated Charcoal", even though kaolin clay is also in it
  - a "62% OFF" banner on a 50% discount
- **"Instead of the vet" framing** will draw the vet pushback above. Owners themselves describe charcoal as a step *alongside* the vet or poison line.
- **Possibly the same goods as PawMergency** (`hypothesis`), sold cheaper on Amazon with 687 reviews.
- **The process is incomplete.** The category context, deep research, avatar and clean-up stages are all blocked: the prompt registry still says `ADD_ID`.

### What to do next (ideas only; nothing was assigned)

1. Fix the product page first (fix list in §7). Remove the two PawMergency testimonials and the cat claim.
2. Ask the supplier ("My Vereli"):
   - Is this PawMergency stock?
   - What is the tube volume in mL?
   - Is there a printed lot and expiry?
   - Where is it made, and is there a third-party test certificate?
   - What are the 2–5 tube prices?
3. Build ads around "**use it with your poison control call / on the way to the vet**", not "instead of the vet" (`hypothesis`, §9).
4. Make free reads before any paid step: re-read the already-bought thread dataset `w0fhweSFZ0i7lN3ew` to move 6 Tier B quotes to Tier A. Then, if approved, open 18 more threads (about $0.036).
5. Register the course prompts in the playbook so the blocked stages can run (§10).

---

## 2. The product as sold (from `product_truth.md` and `PRODUCT_DECISION.md` only)

| Item | What the files say | Status |
|---|---|---|
| Name | PetMergency Activated Charcoal First Aid Kit | confirmed |
| Brand | SavePet. The owner confirmed it on Telegram 2026-11-02 16:40 ("SavePet is the brand"), and again for this run. `PRODUCT_DECISION.md` still says "Brand spelling SavePet vs SavePets not confirmed". It was never updated, because the proposed update was blocked (§10). | confirmed by owner; file out of date |
| Price, 1 tube | $39.95 (shown as down from $80) | confirmed |
| Prices, 2–5 tubes | "Bundle prices for 2-5 tubes unknown." | **NOT CONFIRMED** |
| Label / ingredients | "Named on page: coconut shell activated charcoal and kaolin clay. Full ingredient list, amount per mL and tube volume NOT CONFIRMED." | **partly**: two ingredients named on the page only |
| Format | "Tube with a dial-a-dose mouth applicator, dosed 1 mL per lb of pet weight (per product page; page dose guidance is internally inconsistent)." | page claim |
| Tube volume | Not stated anywhere. Onboarding 05 worked out **about 30 mL per tube** from the page's own numbers (`hypothesis`). | **NOT CONFIRMED** |
| Supplier / SKU | "store lists \"My Vereli\"; owner to confirm whether this is the maker." | **NOT CONFIRMED** |
| Lead time | "lead time … unknown" | **NOT CONFIRMED** |
| Made in USA | Seller claim (locked in `PRODUCT_DECISION.md`). On Telegram 16:12 the assistant asked whether it is true, and no answer is in the log. | **unverified seller claim** |
| Third-party tested | Seller claim (locked). Same open question. | **unverified seller claim** |
| Product page | https://savepet.co/products/petmergency (store: savepet.co) | confirmed |
| Competitors in the decision file | "none given yet" | not updated (§6 has candidates) |

**Page claims captured on 2026-11-02 (onboarding 05 §4).** These are `competitor_claim` grade, not product truth:
- 90-day guarantee
- "Ships in 2 Days" vs "3-5 business days"
- "Two years" tube life
- "Recap after use"
- can be mixed with food
- black stools expected
- "charcoal can bind medications"
- the ASPCA number is shown

---

## 3. Buyer problems

The six problems come from `PRODUCT_DECISION.md`, word for word. Quotes are `customer_report` unless marked otherwise. Coverage counts mean different people with kept quotes.

### 3.1 P1: "My dog ate something toxic and I have nothing at home to help"

**Status:** strong coverage on every channel.

**What owners say**
- "Is there anything I should do right now? It's 1138 at night. Has anyone had anything like this happen and what did you do and what did you notice? 😳😳😳"
  - Facebook, French Bulldog Owners, https://www.facebook.com/groups/7138117442873230/posts/26281064311485256/, 2026-02-02
  - 283 reactions, 595 comments
  - The same text was reposted under another name, so it is counted as one person.
- "Lf activated charcoal for dogs asap". Facebook, https://www.facebook.com/groups/326828460987298/posts/3044464939223623/, 2026-10-27
- "I can not find activated charcoal in the stores anywhere. Has anyone ever used human activated charcoal for substitute?" Facebook Pet Vet Corner, https://www.facebook.com/groups/petvetcorner/posts/1684184149272280/, 2026-04-12
- "I order activated charcoal from amazon but it's gonna arrive just on Sunday. CVS has AC capsules but it has vegetable magnesium stearate on formula. Is it still safe for cats? I can't wait till Sunday." Reddit r/AskVet (cat), https://www.reddit.com/r/AskVet/comments/10hdn3j/, 2023-01-21
- "my dogs got on counter and ate chocolate unfortunately I dont have funds for vet til next week is there anything I can do at home to counter the chocolate so wife and I dont lose our fur babies?" Facebook, https://www.facebook.com/groups/theleessummitcommunity/posts/28439017415799009/, 2026-10-23
- "What can I give a dog that seemed to have picked up poison?" Facebook, https://www.facebook.com/groups/2185259998371204/posts/4797300193833825/, 2026-10-07, 167 comments
- "Can anyone recommend activated charcoal that I can have at home and give my dog the next time they get into something?" and "I feel like we're playing with fire, our dogs are constantly getting into potentially dangerous stuff and the nearest vet is 2+ hours away". Reddit r/DogAdvice, https://www.reddit.com/r/DogAdvice/comments/1urz7u6/, 2026-07-09
- "i am balling my eyes out and frantically searching for information. my dog ate chocolate and i think he's going to get ill 😭😭😭". YouTube https://www.youtube.com/watch?v=Mtx6oLVVJ7k&lc=Ugy-A6F81CjZUsP0w354AaABAg
- "My dog ate a half eaten box of chocolate chip cookies and I'm shaking and I looking up videos on what to do". YouTube https://www.youtube.com/watch?v=eKRzJ3sxUlc&lc=UgyayF849co2HRGmcjB4AaABAg
- "my 3 puppies accidentally ate a choco butternut cake earlier I'm scared and crying because I don't have money to take them to the vet and they are kinda pale.. :(". YouTube https://www.youtube.com/watch?v=eKRzJ3sxUlc&lc=UgzoRXrLkASnluf7gjx4AaABAg
- "My dog just got into my pills of risperidone and im freaking out its literally 12:00am in the morning and". YouTube https://www.youtube.com/watch?v=v-k4ezLEkLU&lc=Ugx6W1QeNc8_-G-nHql4AaABAg
- "I'm kicking myself and currently a mess of guilt". Reddit r/AskVet, https://www.reddit.com/r/AskVet/comments/irkjyg/, 2020-09-12
- "I know I'm such a dumbass but I need help idk how many she ate but there were quite a few and she ate the wrapper and all I'm so worried and feel like a terrible dog mom :(". Reddit Tier B, https://www.reddit.com/r/DogAdvice/comments/1rcuag3/hey_guys_im_severely_worried/

**Already keeping charcoal at home (Tier B, 2026-11-05)**
- "Eventually I just kept activated charcoal at hand just in case she ingested something." https://www.reddit.com/r/DogAdvice/comments/1hji198/took_my_dog_to_the_emergency_vet_at_5am_and_still/
- "I now keep activated charcoal & hydrogen peroxide on hand for emergencies." https://www.reddit.com/r/DogAdvice/comments/158xlnj/comment/jtcoor7/
- "I would now have charcoal on hand in case he decides to scruff down some pills again." https://www.reddit.com/r/DobermanPinscher/comments/1anrg6x/comment/kpujlk8/
- caretaker: "I carry a 1st aid kit in my car. It includes Hydrogen Peroxide with a baby medicine syringe to get it down the dog or if vomiting is not recommended I carry activated charcoal." https://www.reddit.com/r/WagWalker/comments/1ofbfib/comment/nldsw67/
- "I've sorted out a decent first aid kit for the family but then it hit me I've got nothing set aside for the dog." https://www.reddit.com/r/UKPreppers/comments/1o904o0/do_you_keep_extra_meds_for_pets/ (UK)
- Facebook: "Just bought it to have on hand just in case." https://www.facebook.com/groups/holisticandnaturalpets/posts/4520364248227111/, 2026-10-30

**What they tried, and how it went**
- Charcoal given at home, then still unsure:
  - "My dog swallowed my mothers naproxen pill we induced vomiting and gave activated charcoal. Do i need to take her to emerge still ? I'm freaking out help". Facebook, https://www.facebook.com/groups/asktheveterinarian/posts/1520850722800456/, 2026-03-17
- Competitor product used at home, then the vet:
  - "He ate 1/2 slice of chocolate banana bread. Gave him 40ml Toxiban (charcoal) and now taking him to the vet." Then: "The vet said they'll do some bloodwork & give probiotics. They don't want him throwing up toxiban bc it can cause more problems." Reddit r/Pomeranians, https://www.reddit.com/r/Pomeranians/comments/1u31u8h/, 2026-06-11
- No instructions on the bottle:
  - "the bottle didn't say anything about how to serve it. So I sprinkled it on top of some kibble." and "I feel hypervigilant of his behavior and it's stressing me out." VetDTox powder, r/DogAdvice, https://www.reddit.com/r/DogAdvice/comments/18l9sv8/, 2023-12-18
- Home remedies that went wrong:
  - "My parents said to give her milk and I did i don't want to do I'm very worry". Tier B, https://www.reddit.com/r/Pets/comments/1is1hx4/i_need_help_i_think_my_dog_ate_poison_and_dont/
  - pro_opinion anecdote: "Finally she told us she had given him blended milk and garlic to settle his stomach. Poor guy didn't make it." Tier B, https://www.reddit.com/r/veterinaryprofession/comments/1rurzfk/home_remedies/
- Charcoal side effects:
  - "I've had to give my puppy 2 doses of activated charcoal… he hasn't really been wanting to eat or drink much and has been a bit tired." r/DogAdvice, https://www.reddit.com/r/DogAdvice/comments/1bc0je3/, 2024-03-11
- Charcoal used together with the ER (Amazon, PetVet Medic, written by a self-described retired vet tech/RN):
  - "I gave her the activated charcoal and rushed her to the emergency veterinary hospital where the treatment was completed and she was released the next morning." https://www.amazon.com/gp/customer-reviews/RIFGTSSJTXYV1
- Home charcoal that worked (Amazon, PawMergency and PetVet Medic buyers):
  - "I immediately grabbed the Pawmergency from my purse and gave it to him… he didn't end up having any bad reactions to it and we avoided a trip to the vet!" https://www.amazon.com/gp/customer-reviews/RU0M4MDBVULVD, 2026-09-21. **This review was copied onto our page; see §7.**
  - "unlike the first time, he showed absolutely no symptoms at all from the chocolate poisoning or the activated charcoal… saved us from what could've been an extremely high vet bill." https://www.amazon.com/gp/customer-reviews/R98C0V79UQ94X

**Fears and objections**
- "It won't happen" / "he'll be fine":
  - "Dogs can eat more chocolate than you'd think, I'm sure he will be fine!" (comment or1v1ms, https://www.reddit.com/r/Pomeranians/comments/1u31u8h/)
  - "He also got into MOUSE POISON and ate a pellet and never got sick, I swear this dog is indestructible." (Tier B, https://www.reddit.com/r/Pets/comments/s40foh/comment/hso6qm3/)
  - "That told me either the chocolate and dogs is a myth or the chocolate cake was fake" (YouTube https://www.youtube.com/watch?v=eKRzJ3sxUlc&lc=UgxrkDqCW231F_CpI-V4AaABAg)
- Blame from strangers:
  - "i mean don't get me wrong it's nice to be safer than sorry but don't leave ur stuff out lmao then u won't have this issue". TikTok @jeremysfinds, https://www.tiktok.com/@jeremysfinds/video/7541048399605353741, cid 7546489362982404878
  - "Go to the vet anyways. Would you rather your dog die?" Tier B, https://www.reddit.com/r/Pets/comments/1is1hx4/comment/mdcyl5w/
- Too much scary information:
  - "Every God dang website I've come across says that everything is toxic to my dog, even if they're referencing a substance that has to be ingested by the half ton to be deadly." Tier B, https://www.reddit.com/r/unpopularopinion/comments/fkhuus/pet_health_advice_should_not_always_consist_of/

### 3.2 P2: "Should I make him throw up with peroxide?"

**Status:** strong coverage on both sides. Peroxide works for some owners, fails for others, and vets disagree with each other.

**What owners say and what happened**
- Failed:
  - "Did 2 tablespoons and she never puked". YouTube https://www.youtube.com/watch?v=v-k4ezLEkLU&lc=UgySWxyk1G6jWq9V-gp4AaABAg
  - "I immedtiately tried to get her to vomit with peroxide but I didn´t suceed, ofcourse I called the vet but it would have taken a great time to get there for me so I rushed to get some activated charcoal". YouTube https://www.youtube.com/watch?v=xG1nLBTzPDo&lc=UgwVKn1Piu2LdusOJvx4AaABAg
  - "My little bischon ate an entire package of exlax. We gave him hydrogen peroxide and nothing happened." YouTube https://www.youtube.com/watch?v=xG1nLBTzPDo&lc=UgzwhrKP57WzxArILkd4AaABAg
  - "I gave her two teaspoons of hydrogen peroxide… It's been about 3 hours since the HP and other than some nauseated licks she hasn't thrown anything up." and "I'm nervous that both the peroxide and chocolate will end up poisoning her." r/AskVet, https://www.reddit.com/r/AskVet/comments/1ld0da7/, 2025-06-16
  - "I talked to my vet who recommended inducing with hydrogen peroxide. One of my dogs threw up all 4 tampons, and the other dog 86lb retriever did not vomit at all. He was given the max dose of 45mL" and "I did not know it was corrosive to their stomach lining so now I'm worried it's sitting in there." r/AskVet, https://www.reddit.com/r/AskVet/comments/1ttxg2h/, 2026-06-01
  - Tier B: "My fucking dog is immune to this method.." (r/Columbus xqhh7j, comment iqc34n0). "I woke up to find that he had thrown up blood and rushed him to the vet." (r/DogAdvice 175ezey, comment kj2xjt3)
  - Couldn't get it into the dog (Tier B): "But then we couldn't get him to drink it. We were trying to pour it down his throat and use a spoon and it just didn't work." https://www.reddit.com/r/Yorkies/comments/1tb4ru7/what_to_do_and_how_to_protect_your_dog_from/
- Worked:
  - "he's a big 100lbs rottie/dobie and i gave him 2tbsp and he threw up 5 min later… I'm so thankful for this video." YouTube https://www.youtube.com/watch?v=v-k4ezLEkLU&lc=UgwEOdoUpi5i2IPUXrN4AaABAg
  - "call the vet on my way home and they tell me to give her hydrogen peroxide asap to induce vomiting. I take her outside, use a turkey baster to get it down her, and moments later, everything is all over the yard… Poor pupper looks at me with the saddest eyes, full of reproach. She was fine." r/Pets comment k9nxh9x, https://www.reddit.com/r/Pets/comments/17xefh8/, 2023-11-17
  - "the vets I called can't legally give advice so I watched this video and he threw up in about 4 minutes." YouTube https://www.youtube.com/watch?v=v-k4ezLEkLU&lc=UgzWLMdzWv_UHGrXhVt4AaABAg
- Asking the question:
  - "got a hold of a chocolate chip cookie … not sure if he ate the other half. Should I induce vomiting?" Facebook, https://www.facebook.com/groups/asktheveterinarian/posts/1584055409813320/, 2026-06-01
- Tips owners share: "Just make sure your peroxide isn't too old." YouTube https://www.youtube.com/watch?v=xG1nLBTzPDo&lc=UgyQwgQokpnunmNbhi54AaABAg

**Fears and objections**
- Online advice says different things: "My vet said it was safe at that dose but I've read a lot online that says otherwise." (comment op5u0xe, https://www.reddit.com/r/AskVet/comments/1ttxg2h/)
- Tier B: "I was apprehensive about giving him hydrogen peroxide, though, knowing that it can sometimes do more harm than good, and he's a senior dog". https://www.reddit.com/r/WagWalker/comments/1ofbfib/
- **Who tells owners to use peroxide** (2026-11-05 §7, contradiction 1): ER vets, regular vets and Pet Poison Helpline told owners to give it. Other vet staff call it "ulcerative", "no longer recommended", or something for a "true life or death situation". Those last items sit in the truncated part of that report, so only these fragments are visible.
- Vet pushback is in §5.

### 3.3 P3: "The vet is closed at night" (also: the vet is far away)

**Status:** it was thin before the Reddit run and is now covered. Rural distance shows up as often as night closure.

**What owners say**
- "As it's around 11PM, our vet is closed so we have no other option than to go to one of  the emergency vets". r/puppy101, https://www.reddit.com/r/puppy101/comments/utaup0/, 2022-05-19
- "He lives in a very rural area, nearest vet is nearly 2 hours away." and "I'm at a loss for what to do next, ended up calling the nearest vet and they are not open until tomorrow." https://www.reddit.com/r/AskVet/comments/1ld0da7/, 2025-06-16
- "Nothing is open right now, so I am not sure what to do." and "it costs a ton of money to bring him to the vet". https://www.reddit.com/r/AskVet/comments/fsplqw/, 2020-04-01
- "Vet is closed and I can't afford the upfront fees anyway" and "No my area does not have an emergency vet clinic". r/DogAdvice 1l5jsxn, https://www.reddit.com/r/DogAdvice/comments/1l5jsxn/, 2025-06-07
- "We tried five vets, in a city of 42,000, but none would see her" and "We even told each office we felt our dog might die. Nothing." https://www.reddit.com/r/DogAdvice/comments/1196aql/, 2023-02-22 (marijuana)
- "I tried to call a few vets, but they didn't answer, any of them." and "I feel like such a moron." https://www.reddit.com/r/DogAdvice/comments/1u3aj2r/, 2026-06-11 (UK; cooked bones, not a toxin)
- Thread title: "Help!!!! my dog just ate chocolate. I tried to take it from him but he became aggressive and bit me Our vet is closed.What should i do???" https://www.reddit.com/r/DogAdvice/comments/z5x6ve/, 2022-11-27
- "he's asleep now, and i think he'll be alright but damn i never looked up a 24 hour vet in my area so quickly. i was so worried lolol". YouTube https://www.youtube.com/watch?v=eKRzJ3sxUlc&lc=UgySTruZkUmlSHXiqml4AaABAg
- Quora (holiday): "Because it was a holiday we couldn't find any regular vets open… we were asked to make a deposit… A student staying at my place from India offered his credit card for a deposit of $ 1000… The outcome ( at 4:00 a.m. ) was that Pther may have been poisoned." https://mariatrudelsspace.quora.com/This-past-July-01-holiday-I-was-dog-sitting-my-brother-his-wife-s-dog-while-they-were-in-Ontario-We-have-dog-sat-thi
- Tier B:
  - "I am shaking and crying and it's midnight and I freaking hate myself." https://www.reddit.com/r/DOG/comments/1nivkg5/followed_my_vets_advice_and_now_im_finding_out_i/
  - "the closest one is 3 hours away and that's not feasible for me right now." (r/AskVet 1n4lw7u, comment nbm4wqq)
  - "Since we live two hours from the closest emergency vet, I called them, and they advised me to give 2 tbsp of 3% hydrogen peroxide to induce vomiting." https://www.reddit.com/r/AskVet/comments/1s7cy6j/gave_peroxide_to_induce_vomiting_scared_about/
  - "I have no money so I hung up and called the emergency hospital. They said I could come in but doesn't recommend because it's currently a lightning storm and I'm sixteen." https://www.reddit.com/r/PetAdvice/comments/1vid717/i_think_i_accidentally_killed_my_dog/

**What they tried:** calling vets that didn't answer, peroxide while waiting for morning, bamboo charcoal ("I have activated bamboo charcoal… It's the kind that goes inside the care", fsplqw), and Facebook groups (the biggest threads have 595, 257 and 167 comments).

**Still thin:** beliefs and self-image, and transformation (Telegram 02 §7). Facebook gave no literal "vet is closed" line.

### 3.4 P4: "A $2,000 emergency vet bill"

**Status:** the cost pain is covered. The $2,000 figure is not typical (see the price list).

**What owners say**
- "My dog ate a whole box of dark chocolate. This would've saved me 2 grand 😅". TikTok @jeremysfinds, https://www.tiktok.com/@jeremysfinds/video/7541048399605353741, cid 7572279429965300493
- "Rooster managed to counter surf his way into a bag of chocolate chips and ended up with chocolate poisoning. Thankfully he's on the mend after a $600 vet visit 😩🐾🍫". Facebook Dogalogue, https://www.facebook.com/groups/dogalogue/posts/1869962833683603/, 2026-03-09
- "the worlds most expensive bowl of chipotle ($400!)" https://www.reddit.com/r/puppy101/comments/utaup0/, 2022-05-19
- "Visit fee was $125, x-ray another $110, plus $50 for the med to try and induce vomiting… Total cost almost $350." https://www.reddit.com/r/AskVet/comments/1i0mqo2/, 2025-01-13 (possible yarn, not a toxin)
- "$500 at the emergency vet and he would probably still do it again if given the opportunity." r/Pets comment k9oc6vw, https://www.reddit.com/r/Pets/comments/17xefh8/
- "That was an expensive visit to the emergency vet and a sleepless night but they pumped his stomach and he was okay afterwards." r/Pets comment k9nkdy4, same thread
- "I have a problem with my dogs being poisoned by toads/frogs.... the medical bills are just insane!! How can I treat them at home … I have 5 beautiful shepards". Facebook (Belize), https://www.facebook.com/groups/communityanimalrescue/posts/2823914071316110/, 2026-06-10
- "trust me if the vet administrator activated charcoal it will Cost $$$$." Amazon https://www.amazon.com/gp/customer-reviews/RP39F77QYNIHQ
- Tier B (2026-11-05):
  - "My 80lb German Sheppard ate a full container of Ice Cubes black cherry gum... 2500 dollars later and I took him home the next day." https://www.reddit.com/r/Pets/comments/17xefh8/comment/k9ojuej/
  - "Emergency vet is $900 and ours is waaay cheaper, however opens in 2 hours." https://www.reddit.com/r/DogAdvice/comments/1o5jhd5/please_help_emergency_situation/
  - "it's highway robbery when they charge you 700 just to walk in the door!" https://www.reddit.com/r/rant/comments/1bgntw6/comment/kynrnlw/
  - "they could bring the cat by the 'after hours' clinic - starting with an admission fee of $500." https://www.reddit.com/r/unpopularopinion/comments/exc1od/if_people_value_pet_lives_so_much_vet_clinics/
  - "I can't afford another $4,000 surgery and I'm terrified he's going to eat something that kills him before I can stop it." https://www.reddit.com/r/DogAdvice/comments/1quc75f/my_dog_eats_everything_dangerous_despite_training/ (**flag:** the post may contain casino spam; check before use)
  - "Over two thousand spent from my bf's 401k and we will have zero moneys by the end of treatment." https://www.reddit.com/r/legaladvice/comments/1v643ah/landlord_didnt_complete_inspection_and_my_cat_ate/ (cat; substance not shown)
  - "I sure as shit don't have an extra thousand just sitting around." https://www.reddit.com/r/PetPeeves/comments/1ijl060/comment/mbfakzy/
  - "It was 3 grand, but I know I would've never forgiven myself" (r/Pensacola 1ty5w5l, comment oq141hk)
  - "all of a sudden you're thinking about money when you should be thinking of the fragile life" (r/Pets 1qmnc2p, comment o25vp17)

**Insurance pays after the fact (Tier B)**
- "Even with insurance you have to be able to pay upfront before they reimburse you." https://www.reddit.com/r/Pets/comments/1vs0u9a/handling_pet_vet_bills/
- "Our Figo won't pay unless we prove we paid the bill in full first." https://www.reddit.com/r/Pets/comments/1o7lkf1/comment/nn721es/
- Counter-evidence: "It saved me over $20,000 in one year with my dog." https://www.reddit.com/r/Pets/comments/1xlef2m/comment/19rzwran8jneo/

**Poisoning bill amounts owners report** (each linked above)

| Amount | What it was |
|---|---|
| about $350 | Total cost |
| $400 | ER |
| $500 | ER |
| $600 | Vet visit |
| $1,000 | Deposit |
| "2 grand" | 1 TikTok comment |
| $2,500 | Gum / xylitol |
| "3 grand" | Tier B |

- **Also seen, not tied to a poisoning:** $2,400 [context not stated], $4,000 surgery, $4K for a cat, $500 and $700 entry fees, $900 ER.
- **Where the reports disagree on the range:**
  - Telegram 01 says "real bills seen so far run from $600 to $2,000".
  - Onboarding 03 lists $600, a $1,000 deposit and one "2 grand".
  - The 2026-11-05 report says poisoning bills ranged "from about $300 to $2,500".
  - All three are correct for the data each one had. The widest current range is about $350 to $2,500, plus one unverified "3 grand".

### 3.5 P5: "Poison control charges a fee and puts me on hold"

**Status:** thin until the Reddit run, now the strongest problem. All 7 question families are covered.

**What owners say (Tier A unless marked)**
- r/AskVet, https://www.reddit.com/r/AskVet/comments/1t6mhey/pet_poison_control/, 2026-05-07:
  - "It costs $85.00 on my credit card to even be put through to Animal Poison Control."
  - "Once you navigate the fee, you get put on hold for an agent. I've never waited less than 35 min. That's now at least an hour since he ate and started metabolising the toxin. Every minute counts. In some cases, I hung up before speaking to someone because I \*had\* to find someone who would help, NOW."
  - "On a small animal, that kind of wait time is a death sentence.  Who is this serving?"
- r/Pets, https://www.reddit.com/r/Pets/comments/1o68fek/, 2025-10-14:
  - "We spent 2 hours on hold with ASPCA poison control tonight before giving up and calling another service  (Pet Poison Helpline). This took us 10 minutes…"
  - "ASPCA was 110 USD while Pet Poison Helpline was 89 USD."
  - "most ER vets (at least close to us) require a poison control call"
- r/DobermanPinscher, https://www.reddit.com/r/DobermanPinscher/comments/1anrg6x/, 2024-02-10:
  - Title: "Augh- I've been on hold 15 minutes with poison control"
  - "the emergency vet won't work with us until we connect with poison control- is this a lethal dose?!?!?"
  - "poison control charged us $95 when they finally picked up to tell us that he should be fine."
  - kpufboy: "they wouldn't take my call until I gave them a credit card. After almost 20 minutes on hold. I was in a bit of a panic but now I feel a lot better."
  - kpunp6j: "But damn $95 is just crazy"
  - kpuqulv: "they charged me $125 IIRC back in 2013/14."
  - kpxg9rz: "Had to pay 40 to get them to tell us the plant the dog ate would just irritate his stomach, not kill him."
- r/puppy101, https://www.reddit.com/r/puppy101/comments/kzmwje/, 2021-01-18:
  - Title: "Why Tf does animal poison control charge $50.00 freaking dollars?!"
  - "Thank goodness I had someone I could borrow the money from"
  - "Paid 50 dollars just to be told that he will be perfectly fine except for possibly upset tummy. Ridiculous."
  - gjov3dq: "I called four different vets… and was told every time to call animal poison control… not everyone has the funds on hand for situations like that." and "my phone was on 2% and my toddler misplaced my phone charger so I was panicking"
- "it would be a ***$75 consultation fee***. Wtf? No thanks." and "the vet wouldn't see her *UNLESS WE PAID THE $75 CONSULTATION FEE OVER THE PHONE TO THE THIRD PARTY BEFOREHAND!*" (https://www.reddit.com/r/puppy101/comments/utaup0/). The poster was downvoted and the thread was locked.
- "I waited for 1.5 hours or so while the vet waited on the line to speak with poison control… he charged me $150 of poison control communication fee." https://www.reddit.com/r/AskVet/comments/1i2u1bu/, 2025-01-16 (cat, lily)
- "I can't afford the $90 poison control call" and "still shaking". https://www.reddit.com/r/AskVet/comments/1otlu68/, 2025-11-10
- "ASPCA wants to charge $95 (lol)" and "I'd rather not chance $95 just to possibly be told that he needs to have constant access to water." https://www.reddit.com/r/AskVet/comments/126bjlc/, 2023-03-30
- "When I heard that they have a $110 fee i decided to go to the vet after a quick google search." and "they have been on hold with poison control for the last 2 hours." https://www.reddit.com/r/AskVet/comments/1xgibir/, 2026-10-27
- "they all charge somewhere between U$80 and U$100" and "Is calling them worth anything at all or just a waste of money and time". https://www.reddit.com/r/AskVet/comments/1hrl17d/, 2025-01-02
- "I can't really afford the $95 animal poison control fee rn." and "I'm feeling so stupid". https://www.reddit.com/r/AskVet/comments/1g5cd9h/, 2024-10-16
- "We used Peroxide/called the poison control line ($65) /went to the 24hr Emergency Vet… by the time we got to the Vet (30min drive) she had already vomited allot...and they didn't do much". YouTube https://www.youtube.com/watch?v=Mtx6oLVVJ7k&lc=UgxXCSUapCNwSmim4sZ4AaABAg
- Tier B:
  - "…will try to force you to give your credit card and $70 before getting advice about whether your animal has been poisoned." (r/assholedesign raeaqq, comment hnhntoq)
  - "called the animal poison control but they charge $110 and I'm pretty strapped for cash." (r/Rottweiler 1v8xzzl)
  - "I'm on hold waiting for a member of animal poison control to pick up" (r/CATHELP 1ovriv0)

**What they tried:** calling human poison control first and being redirected; calling a second hotline; skipping the call and going to the vet (the ER then called and billed for it); free or cheap routes:
- Chewy chat: "i used chewy chat for free and they were able to get me a discount" (1otlu68)
- microchip company plans (pro_opinion, comment okjau8x)
- AKC Reunite, "a one time payment $20", Tier B (r/legaladvice 1v643ah, comment oztmnjc)
- a free online calculator: "the online calculator is free the poison contol hotline is $95 upfront" (comment my4m6lw, https://www.reddit.com/r/AskVet/comments/1ld0da7/)

**Counter-evidence**
- After vet staff explained the fee, the angry 1t6mhey poster wrote: "Thank you for this very thoughtful and reasonable response. It makes perfect sense and I'm grateful." (comment okm5ksi)
- There is a thread titled "Had a great experience with poison control" (r/puppy101, 2021-06-25; title only).
- Tier B: "Poison control stayed on the line with me as I drove to the hospital and... My dog is now ok." (r/YouShouldKnow 1ihevsn, comment mawjagt)
- The 2026-11-05 report also lists fragments, whose links are in its truncated part:
  - "100% worth it", "invaluable", "Well worth the $70", "saved us a ton of money", "half the price of the emergency visit"
  - against: "all they did was read the same article i read" and "perma hold and pay $75 to be told to bring your dog to the vet"
  - a "free" claim: "They have never charged"

**Fees owners report (Telegram 02):** $40, $50, $70, $75, $85, $89, $90, $95 (×4 independent), $110 (×3), $125 (2013/14), plus a $150 vet "communication fee".

**Holds reported:** 15–20 min, 35+ min, 1.5 h, 2 h (×2).

**Where the reports disagree:**
- Onboarding 02 and 03 said the only fee found was **$65**, and called the profile's $95 "unconfirmed".
- Telegram 02 later found $95 as the most common figure (4 independent reports), with a range of $40–$125.
- The later finding replaces the earlier gap. It does not contradict it.

### 3.6 P6: "I'm scared I'd give the wrong amount in a panic"

**Status:** covered across channels. Owners also worry about **when** to give it, not only how much.

On Reddit, the P6 question family mostly drifted to prescription-medicine dosing (2026-11-05 C3: 89 of its excerpts were off-problem).

**What owners say**
- "When your stressed, the less time you spend trying to figure out how large a dose, could be a life saver." Amazon (PawMergency) https://www.amazon.com/gp/customer-reviews/R3V8DHN3ZZHS1Z, 2026-10-26
- "I place the most pertinent info into the notes app on my phone so that in an emergency (when my anxiety turns my brain to mush) I don't have to fumble around for it." YouTube https://www.youtube.com/watch?v=xG1nLBTzPDo&lc=UgxQ3qhsMdCkh75Ol8B4AaABAg
- "I have the Now charcoal. How much do I give a 60 pound pit and a 37 pound Pittie mix." Facebook, https://www.facebook.com/groups/DuncanStrong/posts/2078592759537933/, 2026-04-29
- "I don't want to be a nervous Nelly but when do you know when to administer the charcoal?" Update: "****Update, I will have it on hand if the time comes that the vet says so.****" Facebook Aussie Friends, https://www.facebook.com/groups/837889829591939/posts/27967074699580085/, 2026-09-03
- "Have charcoal capsules, should I give her some? She's 3 years old and weighs around 55/60lbs". Update: "she's fine. No issues no puking no pooping." Facebook, https://www.facebook.com/groups/asktheveterinarian/posts/1571570144395180/, 2026-05-17
- "My dog ate approx 2 tablespoons of dry cocoa she is 70 lbs do we need to go to the vet?" Facebook, https://www.facebook.com/groups/holisticandnaturalpets/posts/4522115424718660/, 2026-11-01
- Title: "About to feed my dog 40 grams of activated charcoal", plus "I would just like a double check on dosage!" and "tried calling HomeAgain medical line to get this question answered but no one could renew my membership. Please help me save $85". https://www.reddit.com/r/AskVet/comments/189k2n6/, 2023-12-03
- Big dogs:
  - "what if my dog is 147lbs 😭" (TikTok, cid 7504989224321188651)
  - "Do they make it for bigger dogs? My dog is expected to get as big as 120lbs" (TikTok, cid 7505254368082969374)
  - Onboarding 02 does not give the video URL for these two comment IDs, so the link is missing.
- "One tube covers 30 lbs in weight, so be sure to purchase enough to cover the weight of all babies in your home". Amazon https://www.amazon.com/gp/customer-reviews/R1PJXSAJA58WNE
- Tier B (2026-11-05):
  - "In a panic I gave her ~40 ml peroxide and it worked in maybe 5-10 minutes." (Its two permalinks are in the truncated part of that report.)
  - "I know it was stupid, but I induced vomiting with peroxide. It was 3% and it was a little under a teaspoon. I gave it to her and it did nothing. It still has done nothing and it's 9 at night." https://www.reddit.com/r/AskVet/comments/1oz665m/please_help_hydrogen_peroxide/
  - pro_opinion reply: "To induce vomiting, she would have needed almost double what you gave her." https://www.reddit.com/r/AskVet/comments/1oz665m/comment/np9tby6/
  - "They changed me $95 before they would tell me how much hydrogen peroxide to give him to make him vomit." https://www.reddit.com/r/DobermanPinscher/comments/1anrg6x/comment/kpuxhv0/
  - Peer rules of thumb: "a few capfuls (depending on dog weight) and they will throw it right up." https://www.reddit.com/r/Columbus/comments/xqhh7j/comment/iqbmz3s/ ; "you need to follow body weight guidelines for it so you don't give too much." https://www.reddit.com/r/labrador/comments/1uvdj3n/comment/oxakzsi/
  - Label confusion (medicine): "The exact wording on the bottle says, \"Give 1ml (cc)/ 10lbs of body weight. Repeat in 2 weeks.\" \"Give 4ml by mouth for 3 days. Repeat in 2 weeks.\"" https://www.reddit.com/r/DogAdvice/comments/1tnmnde/instructions_unclear/
  - "This is why my dogs medicines are pre-packed ... I don't want our doggo getting the wrong amount." https://www.reddit.com/r/dogs/comments/y3xiql/comment/isb1eyb/
  - "I would like to see if anyone has a dog safe dosing chart." (r/TwoXPreppers 1063esw)
  - "You can use a toxicity calculator to see the severity. That really helped me calm down." (r/Dachshund 1qesw7t, comment nzzy7kk)

**Expectation mismatch:** some owners expect charcoal to cause vomiting:
- "Gave correct amount to my puppy after he chewed on some wood and was eating the splinters. But he never threw up". Amazon 1★ https://www.amazon.com/gp/customer-reviews/R22OQU9696DWL7, 2025-10-24
- A groomer: "the vet have to use activated charcoal to induce vomiting." https://www.facebook.com/groups/1542021025906490/posts/27993132663701966/
- Charcoal binds toxins. It does not make a pet vomit. Copy has to explain this, but the mechanism has not been verified for this product's label.

---

## 4. Buyer language worth reusing in ads

These are exact phrases. Use the words, not the claims around them.

| Phrase | Source |
|---|---|
| "kind of an EpiPen for your curious ones" | Amazon https://www.amazon.com/gp/customer-reviews/RNEFT86O01SYV |
| "inhale chocolate" / "their human looked away for two seconds" | Amazon https://www.amazon.com/gp/customer-reviews/R1PJXSAJA58WNE (**also copied onto our page; see §7**) |
| "My puppy eats everything!" | Amazon https://www.amazon.com/gp/customer-reviews/R25Z1PPLON1W1W |
| "Our big boy will eat just about anything" | Amazon https://www.amazon.com/gp/customer-reviews/RV6VX2KD4A8PS |
| "Hope I never have to use it." | Amazon https://www.amazon.com/gp/customer-reviews/R2XVLZVD62VWS5 |
| "one of those products you hope you never need" | Amazon https://www.amazon.com/gp/customer-reviews/R1A9UDWP5L9AS8 |
| "Haven't Needed It—But So Glad We Have It" | Amazon https://www.amazon.com/gp/customer-reviews/RV6VX2KD4A8PS |
| "Better safe than sorry." | Amazon https://www.amazon.com/gp/customer-reviews/R2B4Q34V2L7YAV |
| "Peace of mind" (review titles) | Amazon R25Z1PPLON1W1W, RYTH1RPGHEUXQ |
| "furbabies" / "fur babies" | Amazon RIFGTSSJTXYV1; Facebook https://www.facebook.com/groups/theleessummitcommunity/posts/28439017415799009/ |
| "the less time you spend trying to figure out how large a dose" | Amazon https://www.amazon.com/gp/customer-reviews/R3V8DHN3ZZHS1Z |
| "when my anxiety turns my brain to mush" | YouTube https://www.youtube.com/watch?v=xG1nLBTzPDo&lc=UgxQ3qhsMdCkh75Ol8B4AaABAg |
| "This would've saved me 2 grand" | TikTok @jeremysfinds cid 7572279429965300493 |
| "I feel like we're playing with fire" | https://www.reddit.com/r/DogAdvice/comments/1urz7u6/ |
| "nearest vet is 2+ hours away" | same |
| "Every minute counts." | https://www.reddit.com/r/AskVet/comments/1t6mhey/pet_poison_control/ |
| "that kind of wait time is a death sentence" | same |
| "Who is this serving?" | same |
| "the worlds most expensive bowl of chipotle" | https://www.reddit.com/r/puppy101/comments/utaup0/ |
| "I can't wait till Sunday." | https://www.reddit.com/r/AskVet/comments/10hdn3j/ |
| "Nothing is open right now" | https://www.reddit.com/r/AskVet/comments/fsplqw/ |
| "a mess of guilt" / "kicking myself" | https://www.reddit.com/r/AskVet/comments/irkjyg/ |
| "I feel like such a moron." | https://www.reddit.com/r/DogAdvice/comments/1u3aj2r/ |
| "I'm feeling so stupid" | https://www.reddit.com/r/AskVet/comments/1g5cd9h/ |
| "My littlest dog is a garbage disposal" | r/Pets comment k9n4vli, https://www.reddit.com/r/Pets/comments/17xefh8/ |
| "the bottle didn't say anything about how to serve it" | https://www.reddit.com/r/DogAdvice/comments/18l9sv8/ |
| "double check on dosage!" | https://www.reddit.com/r/AskVet/comments/189k2n6/ |
| "freaking out" / "frantically searching" / "shaking" | YouTube comments in §3.1 |
| "a little lesson learned for the human" (exact: "A huge mistake and lesson learned for the human") | Amazon R1PJXSAJA58WNE |
| Tier B: "He was like a vacuum!" | https://www.reddit.com/r/puppy101/comments/16jn9ib/comment/k0qu1lb/ |
| Tier B: "the original cast-iron stomach" | https://www.reddit.com/r/puppy101/comments/16jn9ib/comment/k0qxqwa/ |
| Tier B: "like it was a bag of Doritos" | https://www.reddit.com/r/animation/comments/1rjw27o/comment/o8gpmzy/ |
| Tier B: "Dogs will get into anything when determined enough." | https://www.reddit.com/r/breakingmom/comments/wrxfn4/comment/ikvpjel/ |
| Tier B: "feel like a terrible dog mom" | https://www.reddit.com/r/DogAdvice/comments/1rcuag3/hey_guys_im_severely_worried/ |
| Tier B: "the dread of an emergency vet bill hangs over my head" | https://www.reddit.com/r/PetPeeves/comments/1ijl060/comment/mbfakzy/ |
| Tier B: "highway robbery when they charge you 700 just to walk in the door" | https://www.reddit.com/r/rant/comments/1bgntw6/comment/kynrnlw/ |
| Tier B: "Insurance … pay upfront before they reimburse you" (exact: "Even with insurance you have to be able to pay upfront before they reimburse you.") | https://www.reddit.com/r/Pets/comments/1vs0u9a/handling_pet_vet_bills/ |

**Not customer voice (`competitor_claim`, affiliate captions on TikTok):**
- "If your dog eats like they have a death wish" (@tastefullyextra)
- "what if you could prevent your pups unaliving" (@frugal__living)
- "Better to have it and not need it then need it and not have it" (@dailytt.shops)

---

## 5. Vet and expert pushback, and claims we must not make

### 5.1 Pushback, word for word

All `pro_opinion` (unverified) unless marked `customer_report`.

**TikTok** (@melissa_fergus https://www.tiktok.com/@melissa_fergus/video/7489845283237465375 and @mm336777 https://www.tiktok.com/@mm336777/video/7496873206314208554):
- "as a vet assistant never give this without consulting a vet first! charcoal can cause dangerous electrolyte imbalances!" cid 7504847248652600095, **2,533 likes**
- "vet professional here, please consult a veterinarian before administering! in some cases you can ABSOLUTELY cause more harm than good." cid 7505153901018006315, 320 likes
- "PLEASE DO NOT GIVE YOUR PETS PEROXIDE! Take them to a vet where we can induce vomiting safely… please do not give activated charcoal without FIRST REACHING OUT TO PET POISON HELPLINE!!!" cid 7505072267107255071, 92 likes
- "do not give unless instructed by a vet or poison control". cid 7501794719468471082, 65 likes
- "Some things specifically tell you NOT TO INDUCE VOMITING because it's more dangerous." cid 7505107364363715371, 39 likes
- Onboarding 02 lists these last two under the mm336777 video. It does not say which video each one is on.

**Reddit**
- "We have people call poison control on the way to the hospital if they can… There are a lot of things that we can't/shouldnt make the pet vomit for… human poison control is government funded… We dont have that luxury in vet med!" Comment okin3t6, score 20, https://www.reddit.com/r/AskVet/comments/1t6mhey/pet_poison_control/
- "That's a very old school thing to tell owners to induce vomiting themselves at home, particularly because of the risks… there are licensed subcutaneous injections that can be given to induce vomiting at the vets. I would opt for this." Comment op5lrfg, https://www.reddit.com/r/AskVet/comments/1ttxg2h/
- Tier B:
  - "Hydrogen peroxide is no longer really recommended… It can frequently cause abrasions and ulcers in the esophagus and stomach" (r/AskVet 1n5cwt8, comment nbrs3od)
  - "Inducing vomiting on your own leads to a risk of aspiration pneumonia" (r/puppy101 ly4mls, comment gpsutmh)
  - "frequently pets still have to come in to see us because the hydrogen peroxide didn't work." (r/todayilearned kl6ak8, comment gh73oey)
  - "Be careful with activated charcoal. You can overdose your pet on it. I have seen a dog die from this." https://www.reddit.com/r/LifeProTips/comments/507912/comment/d7232qu/
  - "If your dog ate actual poison, pet poison control is only going to direct you to go to the vet. There's no home remedy for a poisoned dog." https://www.reddit.com/r/Pets/comments/1is1hx4/comment/mdczwjg/
  - "Not deciding they're an expert and giving activated charcoal or using hydrogen peroxide UNLESS advised by a medical professional." https://www.reddit.com/r/AnimalAdvice/comments/1w3q0az/comment/p73t58v/
  - "Emergency vet ASAP; this can't be treated at home." https://www.reddit.com/r/AskVet/comments/1c17ad1/comment/kz1htz2/
  - "there are a lot of toxins that START with GI issues and then can cause kidney / liver issues - just because we're not vomiting any more doesn't necessarily mean we're OK." https://www.reddit.com/r/AskVet/comments/1p4w9tn/comment/nqh5fc7/
  - "decontamination AKA \"Vom-it, Bind-it, Dilute-it\" AKA make him vomit, bind the toxin with activated charcoal/carbon, and dilute it with high load IV fluids." https://www.reddit.com/r/Rottweiler/comments/1v8xzzl/comment/p0boa29/ (describes what the vet does)

**Owners passing on what their vet said (`customer_report`)**
- "My vet said please don't use that she could aspirate the charcoal in her lungs and get pneumonia so I returned it." Amazon 1★ https://www.amazon.com/gp/customer-reviews/RXIWHMIQJDOQL, 2026-08-26 (PawMergency)
- "So weird my dog ate chocolate and the emergency vet clinic said inducing vomiting at home or giving charcoal at home weren't recommended. 🙄" YouTube https://www.youtube.com/watch?v=Mtx6oLVVJ7k&lc=UgzG20pNmRcyo4zF1nJ4AaABAg
- "I bought activated charcoal as precaution for poisoning situations. But my vet didn't like the fact that I bought it. What do you guys think?" Facebook, https://www.facebook.com/groups/514612959043998/posts/2623712288134044/, 2026-09-08
- Aspiration fear: "activated charcoal should not be given dry because they can aspirate it into their lungs" (https://www.reddit.com/r/DogAdvice/comments/18l9sv8/) and "I fear she inhaled a little of it via her mouth or am I exaggerating? I don't want to do her more harm than good" (cat, https://www.reddit.com/r/AskVet/comments/1df54i1/, 2024-06-13)
- "not all toxins can be treated with charcoal so make sure you do your own research". Amazon https://www.amazon.com/gp/customer-reviews/R98C0V79UQ94X

**Facebook education post (`pro_opinion`):** "Keep chocolate out of your pet's reach—and if ingestion occurs, contact a veterinarian promptly." https://www.facebook.com/groups/vetjobsworldwide/posts/1090011996996990/

**Facebook affiliate post that contradicts itself (`competitor_claim`):** "Everyone should have activated charcoal on hand for an emergency. it works great for pets and humans." The same post says "Do not administer activated charcoal unless instructed." and warns that "human products may contain sweeteners like xylitol". https://www.facebook.com/groups/DuncanStrong/posts/2037119440351932/

**Other objections**
- Black staining on white coats: "What is good to help with the black staining from the charcoal?" (Facebook groomer post above)
- Off-label "detox" use: "would it be ok to do the activated charcoal gel for a one time detox to clear out their system?" https://www.facebook.com/groups/DuncanStrong/posts/2004915606905649/. This is a claims risk; do not invite it.

**What this adds up to (`conclusion` across reports):** owners and vets both put charcoal **together with** a call to the vet or poison line, not **instead of** one.

### 5.2 Claims we must not make (locked or contradicted)

| Claim (our page) | Why not |
|---|---|
| "For cats, this is the only safe at-home option … the ASPCA confirms no safe alternatives." | Contradicted by "NOT SAFE FOR CATS" (TikTok @melissa_fergus, cid 7504855570481988398, 575 likes). The ASPCA attribution has no source. Our own second FAQ just says "Yes. It is dosed by weight". Some owners do report using powder on cats (Amazon RQ0W5M01QLWPB, R28AQ4RE4PJ6RB, R39B5Y92LBQFYO), so this is **unresolved**. |
| "#1 VET RECOMMENDED", the named "Miranda Brightstein, DVM", "Vet Formulated" | Locked seller claims. Nothing has been verified. |
| "Made in the USA", "Third-Party Tested" | Locked seller claims. The owner's answer on whether these are true is not in the log. |
| "60,000+ … Pet Lives Saved" (the same number is also used for "devoted pet parents") | Locked seller claim. Buyers are not the same thing as lives saved. |
| "No Vomiting", "doesn't … risk aspiration", "wide safety margin", "When in doubt, round up" | Clash with the aspiration, electrolyte and "more harm than good" pushback. These need clinical checking (course block 2). |
| "100% Activated Charcoal" / "Pure Activated Charcoal" | The page also lists kaolin clay. |
| The full toxin list ("household chemicals", "nicotine", "blue-green algae", "THC", "mushrooms"…) | Coverage of each toxin is unverified (`hypothesis`). An owner says "not all toxins can be treated with charcoal". |
| Anything framed as "instead of the vet" | See 5.1. |
| The owner profile's numbers as facts (451,000 calls, 38%, 81%, 82%) | Locked as hypotheses in `PRODUCT_DECISION.md`. |

---

## 6. Competitors (every line is `competitor_claim` or listing data, not proof)

| Brand / product | Price seen | Reviews · stars | Claims and notes | Source report |
|---|---|---|---|---|
| **PawMergency – Activated Charcoal First Aid Kit**, ASIN B0FXBQSFJP | $36.99 (1). 2-pack B0FYL6M55D $62.98. A 1★ reviewer paid "$100" for five. | 687 · 4.7 | Same product name as the "PawMergency" typo on our page. A review says "One tube covers 30 lbs", which matches our "under 30 lbs is one tube". Two of its reviews are copied onto our page (§7). It is pushed on TikTok Shop by affiliates; the posts carry the handles **@PetlyPet** and **@Vetanica**. Top posts: 1.27M views (@melissa_fergus), 1.10M (@mm336777), 640K (@muonline_pc, stitching @RuralVetServices), 535K (@frugal__living), 426K (@jeremysfinds). `hypothesis`: same white-label goods as SavePet, or a direct copy. Not verified. | onboarding 02 §5, 05 §6 |
| **PetVet Medic Activated Charcoal**, ASIN B0FNY9J7ZT | $24.99 | 304 · 4.7 | Seller claims: "beef-flavored", "Veterinarian-Developed, Made in USA", 60 mL | onboarding 02 §5 |
| **Vetanica** | not seen | not seen | Facebook ads for "an activated charcoal syringe", seen by a Florida owner: "I'm seeing some stuff advertised now by Vetanica… Before I take the bait - does anyone know if it's legitimate?" (https://www.facebook.com/groups/holisticdomesticpetcare/posts/2016643172330081/, 2026-09-11). Also a handle in PawMergency affiliate content. | onboarding 02, 03 |
| **NOW Activated Charcoal** (a human product) | not seen | not seen | Owners use it ("I have the Now charcoal", Facebook). An affiliate post links NOW plus a "60ml EZ Dose Bottle" gel and a powder through amzn.to links. Xylitol warning for human products. | onboarding 03 §4 |
| **Generic powder 3.53 oz**, ASIN B0CN6JLXLS | $15.59 | 645 · 4.7 | Low-price alternative. Owners have used it on cats. | onboarding 02 §5 |
| **Cheap Amazon tubes and gels**: 30 ml tube B0H2VH3RQP $9.99; 60 mL gel B0GJ5Z1X68 $12.87; 2 tubes B0H1KR9Z9J $16.60 | $9–18 | 2–56 reviews | These set the floor behind the "$10 product" objection. | onboarding 02 §5 |
| Named on Reddit (mentions only) | — | — | **Toxiban** (an owner gave 40 mL at home); **VetDTox** powder (no serving instructions, the owner says); **Charactol 50** (given by a vet); CVS capsules; activated bamboo charcoal | telegram 02 §4.3 |
| Hotlines and services owners use instead of a kit | — | — | ASPCA Animal Poison Control, Pet Poison Helpline, HomeAgain, AKC Reunite, Chewy chat, microchip plans, free online toxicity calculators | telegram 02 §4.3 |

**Price position:** SavePet at $39.95 is above every listing seen.

**Price objections (customer_report):**
- "why don't they make more affordable so everyone can access it" (TikTok mm336777, cid 7500685011911672607)
- "Why isn't this cheaper??" (cid 7503171397475222318)
- "You can buy activated charcoal, much cheaper" (TikTok muonline_pc https://www.tiktok.com/@muonline_pc/video/7514895346850336031, cid 7524865301285421854, 106 likes)
- "don't buy this overpriced product bruh they be charging 60$ for a 10 dollar product" (cid 7566770548093895437)

**Price acceptance:**
- "wouldn't have bought if price was outrageous" (Amazon R2B4Q34V2L7YAV)
- "It's expensive but 100% worth the emergency use" (Amazon R1PJXSAJA58WNE). This is the sentence removed from our page's copy of that review.

**Trust in online pet products:** "ya i don't trust any pet products that come from the internet and not the vet🥹" (TikTok @frugal__living https://www.tiktok.com/@frugal__living/video/7493593664329944350, cid 7493975684151837486, 78 likes)

**Hearsay, watch only:** "Another creator was advertising this also, then in the comments said she no longer supports this product or company after learning some disturbing info" (TikTok melissa_fergus, cid 7504768888234017566)

**Brand silence:** SavePet, PawMergency and PetVet Medic are mentioned **0 times** in anything read on Reddit (telegram 02). Across the 126 later answers, SavePet, PawMergency, PetVet Medic, Toxiban and VetDTox are mentioned **0 times** (2026-11-05).

**Vantage was not used** in any report. Telegram (15:05, 11-02) reported it had nothing on SavePet or pet first aid.

---

## 7. Product page problems: fix list

Source: the page capture of 2026-11-02 19:20 UTC (Apify dataset `k6m5i9PoGnUih17tH`), onboarding 05 §5–§6. Highest priority first.

### 7.1 Copied competitor reviews (fix first)

| Page card | Where it came from | Match |
|---|---|---|
| "Sarah LeMaster", Facebook-style card showing "13952" and "Like Reply 8d" | Amazon R1PJXSAJA58WNE, PawMergency B0FXBQSFJP, 5★, 2026-05-27 | **Word for word, except one sentence was removed:** "It's expensive but 100% worth the emergency use, piece of mind, and health of your precious baby." |
| "Jessi M., 32" Verified Buyer (the cheesesteak story) | Amazon RU0M4MDBVULVD, PawMergency B0FXBQSFJP, 5★, 2026-09-21 | **Word for word**, with "Pawmergency" changed to "Petmergency" |
| "Sarah, R", "Mary, W", "Diane H.", both "User1" cards | — | No match in the 44 Amazon reviews held. Origin unknown. |

`conclusion` for the text match. `hypothesis` for why it happened (white-label supplier listing, or copy lifted from the competitor).

**Fix:** remove both cards. Ask the supplier whether SavePet is PawMergency stock. Rework the "WE DO NOT SELL ON AMAZON … Beware of fakes on Amazon" line once you have that answer.

### 7.2 The 16 contradictions and claim risks (onboarding 05 §5)

1. **Discount maths.** The banner says "62% OFF", but $39.95 against $80.00 is 50% off. The banner also says "SPOOKTOBER" on 2 November.
2. **"Only sold here … fakes on Amazon"**, while the page shows PawMergency reviews and says "PawMergency is formulated for both dogs and cats".
3. **The cat claim** ("only safe at-home option", "the ASPCA confirms"), which another FAQ contradicts and customer voice disputes.
4. **"No Vomiting" / no aspiration.** The page's own lead review describes a dog "coughing then vomiting foam", and vet staff warn about aspiration.
5. **Call the vet first, or give it first?** One FAQ says contact your vet or the ASPCA "first". Another says "you can give it even if unsure". The 15-minute timeline puts the call *after* dosing.
6. **"Wide safety margin … When in doubt, round up."** No source is given.
7. **How long it works:** "within the first hour" vs "still effective within 4 hours" vs "still helpful up to 6" vs a "1 to 6 Hours" timeline. Peers and pros on Reddit say about 2 hours ("the window to vomit up a toxin is limited to 2 hours", Tier B P2-36, in the truncated part of the 2026-11-05 report). The profile says 60 minutes.
8. **The toxin list is too broad** (household chemicals, nicotine, algae, THC, mushrooms). Each one is unverified.
9. **Dose and tube volume.** The calculator says "<30 lbs Dogs & cats 1 tube". The FAQ says "Under 15 lbs: half a tube. 16 to 30 lbs: one tube" and "1mL per 1lb". This implies about 30 mL per tube (`hypothesis`), but the page never states the volume.
10. **"100% Activated Charcoal" / "Pure"**, next to kaolin clay.
11. **Shelf life.** The answer to "Is there a shelf life?" is shipping text. Another FAQ says "Two years". There is no lot or expiry info. An owner on a competitor: "There is no manufacturing date on the charcoal on any of the five… we could be buying old charcoal that will in fact do nothing" (Amazon https://www.amazon.com/gp/customer-reviews/R2L1FFS3VVEJ4O).
12. **The survey block shows "0%"** for all three stats ("survey of 900 dogs and cat owners").
13. **"60,000+"** is used for both "devoted pet parents" and "Pet Lives Saved".
14. **Review count signals don't agree:** "4.8/5 based on 7,752+ Reviews" vs a "13952" Facebook-style card that is really an Amazon review.
15. **Brand spelling:** SavePet vs "SavePets" ("Try SavePets →", "Why SavePets Stands Out", "savepets.co") vs "PawMergency" vs "Petmergency". The store domain is savepet.co.
16. **Named vet, "#1 Vet Recommended", "Made in USA", "Third-Party Tested", "Vet Formulated", "PetMergency®"**: none checked. All stay seller claims.

**Minor:**
- "Ships in 2 Days" vs "3-5 business days"
- "88% SOLD" and "Almost Sold Out" on a product that can still be ordered

### 7.3 Conflicting dosing guidance (summary of 7.2 rows 5, 6, 7 and 9)

The page gives:
- two different weight tables: tubes to buy vs dose
- three different time windows
- two different orders for "call the vet" vs "give it"

Owners in §3.6 ask exactly these questions: how much, and when. **One clear printed card should replace all of these** (see §9), and the label must state the mL.

---

## 8. The avatar profile check (66 points)

**What the profile is:** the owner's written summary ("a deep-dive synthesis"). **Its soundbites and statistics are the owner's summary, not customer evidence.**

The profile's statistics:
- 451,000+ calls, "one call every 70 seconds", "nearly 4% increase"
- $95 hotline fee
- $2,000 bill
- 38%, 81%, 82%
- income $120,000
- 65% female / 35% male
- $80/month food, $200 checkups, $50 treats

Its post-transformation soundbites (for example the vet saying "You did exactly the right thing. Administering activated charcoal within the first hour was the difference here.") are **illustrative, made up by the profile**. They are not quotes.

**Tally from Telegram 03 (2026-11-02):** 66 points checked.

| Verdict | Count |
|---|---|
| Backed up | 30 (4 of them rest on a single report) |
| Partly backed up / with a contradiction | 11 |
| Contradicted | 7 |
| Not tested | 18 |

**The tally was not updated** by the 2026-11-05 read. That report changed a few verdicts in its own table (below), but it published no new totals, and I don't recompute it here.

**Readable points (49 of 66).** "11-05 update" shows the change from the 2026-11-05 read, where its row is readable.

| # | Profile point (owner's summary) | Verdict (Telegram 03) | 11-05 update |
|---|---|---|---|
| B1 | Ages 27–42 / 43–55 | not tested | — |
| B2 | 65% female / 35% male | not tested | — |
| B3 | 1–3 pets | partly (5 shepherds exceeds the range) | — |
| B4 | The pet is a "fur baby" | backed up | — |
| B5 | Renting or owning; may have kids | not tested (1 toddler mention) | — |
| B6 | Income $120k, spends liberally | **contradicted** for the people who have the problem | **contradicted more strongly** ("I have no money", "I cant afford that", "Things are financially tight") |
| B7 | 82% say their pet is like a child | not tested | still not tested |
| B8 | Reactive preparer: a near-miss leads to buying | partly. Two other buying moments also exist: "just in case", and mid-emergency (same-day Prime) | home-charcoal habit after an ER visit (P1-1) fits this |
| C1 | Nothing at home | backed up | more support (P1-1…P1-9) |
| C2 | Toxins named in the profile | backed up (grapes from 1 report). Cane toads added (4 reports) | — |
| C3 | 451,000 calls | not tested | — |
| C4 | $80 / $200 / $50 spend | not tested | — |
| C5 | "first 60 critical minutes" | belief backed up; clinical claim not tested | belief backed up again; peers and pros say about 2 hours |
| P1 | Nothing at home | backed up | — |
| P2 | Peroxide | backed up, with contradictions | more failures; vets disagree |
| P3 | Vet closed at night | backed up; rural distance as common | rural again (H7) |
| P4 | $2,000 bill | cost pain backed up; **$2,000 contradicted as typical** | $2,500 gum bill (Tier B); entry fees |
| P5 | Fee and hold | **backed up (strongest)** | C4: little new (121 repeats) |
| P6 | Wrong amount in a panic | backed up; adds *when* | the hotline paid to learn the dose (H4) |
| E1 | Anticipatory dread | backed up | — |
| E2 | Guilt | backed up | more (P1-12, P1-18, P1-19) |
| E3 | Helplessness | backed up | — |
| E4 | Financial panic, "38%" | feeling backed up; 38% not tested | 38% still not tested |
| E5 | Protective rage | not tested | **partly**: anger aimed at careless people ("be a fucking responsible adult") |
| F1 | "I was right there" (frozen, on hold) | backed up in its parts | — |
| F2 | "Too late" discovery overnight | not tested (closest only) | — |
| F3 | Seen as negligent for *lacking* charcoal | self-blame backed up; **vet judging for lacking charcoal contradicted** (vets object to *having* it) | a vet judging the owner in another way: accused of THC exposure (P1-53) |
| F4 | "$3,000 choice", 81% | fear of cost backed up; $2,500–3,000 above most bills; 81% not tested | — |
| F5 | Telling the kids | not tested | still not tested |
| R1 | Partner thinks she's dramatic | not tested (a mother holding back the vet is the closest) | "My wife thinks I overreacted, and wasted $135." (limp, not poisoning; P4-18) |
| R2 | Kids finding the dog | not tested | still not tested |
| R3 | Shame in front of the vet | **contradicted in direction** | — |
| R4 | Mother-in-law | not tested | — |
| R5 | Worrying in Facebook groups | partly | — |
| H1 | "I'm sure it's fine" | backed up | more ("I expect your dog will be ok.") |
| H2 | "dogs eat weird stuff" | backed up in the category | — |
| H3 | ER vet: "nothing on hand?" | **contradicted** | — |
| H4 | Pet-proofing jab | partly (from strangers) | more (P1-37, P1-38) |
| H5 | "every responsible owner should have charcoal" | backed up only as affiliate content | — |
| S1 | Frantic Googling, mixed advice | backed up | "this warrants a vet trip" without saying how soon (P1-23) |
| S2 | Peroxide, fear of burns; "unsafe for cats" | fear backed up; peroxide works for some; cat not tested | — |
| S3 | ASPCA $95 + hold | backed up, with a fee caveat (newest posts say $85–$110) | — |
| S4 | $2,000+ ER "gave her charcoal" | partly (the ER does more, and bills are lower) | — |
| S5 | "Insurance is money AFTER" | not tested (answers unread then) | **11-05 kept direct Tier B support** (P4-20…P4-24, "pay upfront before they reimburse you") **plus counter-evidence** (P4-25 "saved me over $20,000"). Its verdict row is in the truncated part. This is my reading of its items: partly backed up, Tier B. |
| W1 | Doesn't want to force vomiting | partly, with a contradiction | — |
| W2 | No mixing, measuring or maths | backed up | — |
| W3 | Don't sit on hold | backed up | — |
| W4 | "$2,000 for the same thing… twenty bucks" | partly; **the profile contradicts itself** ($20 here, $40 elsewhere; the real price is $39.95) | — |
| W5 | Learns about the product only after an emergency | partly (row cut off in the source) | — |
| Objection #3 | "My pet has never gotten into anything" | (status not readable in Telegram 03) | **backed up as an objection owners voice** ("I swear this dog is indestructible") |

**Not readable:** the other 17 points (W6 onward, and the rest of the objections). They are in the truncated part of Telegram 03.

**Also not done:** the avatar copy into `avatar/owner_avatar_profile.md` was **never committed**. The gateway blocked the write (§10).

---

## 9. Angle and offer ideas the reports raised (all `hypothesis`, not proven)

Each idea still needs two independent customer reports for its specific claim (AGENTS rule 4) and must not break the §5.2 rules.

1. **"Use it with your poison control call / on the way to the vet."** Reports 02, 03, Telegram 02 and 11-05 H5. Owners and vets both pair charcoal with the call. Some kit-keepers carry peroxide plus charcoal and use charcoal "if vomiting is not recommended". This framing is likely to meet less vet pushback than "instead of the vet".
2. **A weight-based dose card printed on or with the tube.** From 11-05 H4 and Telegram 02 H2. Owners pay $95 to be told "how much", and a competitor's bottle "didn't say anything about how to serve it". **Our own page dosing must be fixed first** (§7.3).
3. **"The minutes between 'he ate it' and reaching help"** (fee, hold, 2-hour drive) as the frame. Telegram 02 H1.
4. **A rural / "nearest vet is 2+ hours away" sub-avatar.** Telegram 02 H3 and 11-05 H7.
5. **Money hooks built on entry fees and "pay first, insurance pays you back later"**, not on "$2,000". From 11-05 H6.
6. **"An EpiPen for your curious ones"**, plus "eats everything" language (garbage disposal, vacuum, Doritos). Onboarding 02.
7. **Owner guilt** ("their human looked away for two seconds"), handled gently. Onboarding 02.
8. **Florida / cane-toad regions as a regional trigger.** 4 reports: Amazon ×2, Facebook ×2, one of them in Belize.
9. **Multi-tube bundles for big dogs and multi-pet homes.** "what if my dog is 147lbs 😭", "cover the weight of all babies in your home". The bundle prices are unknown (§2).
10. **Answer these objections openly in copy:**
    - "call your vet first"
    - cats
    - price vs $10–17 Amazon tubes
    - shelf life and expiry
    - "don't trust internet pet products"
    - "does anyone know if it's legitimate?"
    - black staining
    - human charcoal as a substitute (the xylitol risk)
    - charcoal does not make the pet vomit
11. **Proof that worked for buyers:**
    - a friend's suggestion
    - "recommended by veterinarians who are also close friends"
    - a retired vet tech's endorsement (Amazon RNEFT86O01SYV, R3V0WAMC78GXMM, RIFGTSSJTXYV1)

    Real, verifiable SavePet reviews are needed. Copied ones are not usable.

**Conclusions the reports reached (`conclusion`):**
- C1: P5 and P3 are no longer thin.
- C2: Reddit owners describe charcoal mostly as something the vet gives; home charcoal stories are about worry, not relief.
- C3: the P6 Reddit questions as worded don't reach charcoal dosing.
- C4: Reddit Answers adds little new for P5.
- C5: all 156 answers are now read.

---

## 10. Gaps and open items

### 10.1 Evidence not yet verified

- **Tier B quotes (thread not opened, date unknown):**
  - all items kept on 2026-11-05
  - Telegram 02 §4.2

  Unverified until opened.
- **$0 first step:** six Tier B items sit in threads already bought on 11-02. Re-reading dataset `w0fhweSFZ0i7lN3ew` (free) could move them to Tier A. They are P1-4, P6-6, P5-2, P2-6 and P5-27 in r/DobermanPinscher 1anrg6x, and P4-1 in r/Pets 17xefh8.
- **18 threads worth opening:** about $0.036 in total (11-05 §6), for example:
  - 1hji198 (kept charcoal after a 5am ER visit)
  - 158xlnj
  - LifeProTips 507912
  - DogHealth 1xf2953
  - AskVet 1s7cy6j and 1oz665m
  - Yorkies 1tb4ru7
  - 1quc75f (check for spam)
- **Quotes with no link, dropped by the reports and not used here:**
  - 2 in Telegram 02: "I poured hydrogen peroxide down his throat and he gagged…" and "She told me to give salt to make her vomit…"
  - 7 in 2026-11-05 (5 of them in the P3.19 answer, which reads as invented)
- **Reddit Answers reliability:**
  - 3 quotes in Telegram 02 did not support the claim they were attached to.
  - 2026-11-05 counted 39 mismatches (including human medical posts) and 5 permalink inconsistencies.
- **Missing links in this document:** two TikTok comment IDs (7504989224321188651 and 7505254368082969374) have no video URL in onboarding 02.
- **Truncated reports:** see the top of this document. These items are unreadable in this compile: 2026-11-05's P2, P3 and P5 kept items, P6-13 onward, and the 17 avatar points.

### 10.2 Steps that were blocked, and why

| Step | Status | Why |
|---|---|---|
| Onboarding 01: Reddit Answers bank | Blocked, later done by Telegram 01 + 02 | The registry said `ADD_ID`; 26 vs 27 questions; the wording was written for skincare. The owner then approved lesson 3, the 26 questions and the rewording (Telegram 17:24). |
| Onboarding 03: avatar clean-up ("Zakaria merge, then cluster") | **Blocked** | No prompt anywhere (registry, Supermemory, Scaler, both repos), and no avatar stage output to clean up. Second time (Vylaras 2026-10-20 was the first). |
| Onboarding 04: category context template | **Blocked** | Registry `ADD_ID`; the raw research was not complete (Reddit had 0 questions run at the time); the lesson's prompt is written for an "angle" with an "(INSERT ANGLE HERE)" blank. |
| Onboarding 05: deep research prompts 1–4 and the rating | **Blocked** | Registry `ADD_ID`; the four books are not in `00_rules_and_process/books/` (Breakthrough Advertising, The Bencivenga 100, Scientific Advertising, Cashvertising); no OpenAI Deep Research tool on the gateway; wrong order; the `{INSERT ANGLE}` blank is undecided. Second time. |
| Telegram 03: copy the avatar profile into the repo, and add the brand to `product_truth.md` | **Not committed** | The gateway allowed only the report path. The ready text is in that report's Appendix A (profile) and Appendix B (`product_truth.md` with a Brand section). |
| Category document `EB_CATEGORY_CONTEXT_<slug>_v2.md` | **Not created** | The filename hasn't been chosen. Quote banks sit in onboarding 02 §4, onboarding 03 §4, Telegram 02 §4 and 11-05 §2. |
| `course_v2/COVERAGE_V2.md` | All 24 blocks unticked | No stage output to link. |

### 10.3 Channels still open

| Channel | State |
|---|---|
| Quora | Answers missing; one story and two titles only |
| Facebook | Only the post text of 30 posts read; comments not bought on the big threads (595, 257, 167, 99 comments) |
| YouTube | Transcripts not pulled (the lesson asks for them) |
| r/CatAdvice | Returned 0 |
| r/AskVet and r/DogAdvice | Not saturated; page 2 not pulled |
| r/cats, r/dogs, r/puppy101 | Mostly titles only (55 post bodies unread) |
| Cats overall | Thin |
| P6 on Reddit | Needs charcoal- and weight-specific wording (paid, needs the owner's OK) |
| AdSpy | Not on the gateway |

### 10.4 The 21 rebuilt questions

- Telegram 01's 156-question list could not be read from P5.8 to P6.2 (tool truncation).
- Telegram 02 rebuilt **21 questions (P5.8–P5.26, P6.1–P6.2)** from the approved template and slot wording, and ran them in that rebuilt form.
- Their wording may differ slightly from what the owner approved, and nobody has been able to check, because the file is still truncated.
- If the exact wording matters, rerun those 21 from the file (about $0.21; needs approval).

### 10.5 Unknown Facebook Ad Library pulls

- **What:** untagged runs of actor `XtaWFhbtfxyzqrFmd` (identified on 2026-10-20 as `curious_coder/facebook-ads-library-scraper`) keep running. **No SavePet report started them**, and nobody has found what does.
- **Counts reported:**

| Report | Window | Runs | Cost |
|---|---|---|---|
| Onboarding 01 | 6 h | 23 | $0.96 (`total_usd`) vs $1.03 (`by_job.untagged`), so the tool's own totals disagree |
| Onboarding 04 | 10 h | 26 | $1.08 |
| Telegram 02 | during the run, 20:28–20:29 | 3 more | $0.135 |
| 2026-11-05 | 2026-11-06 | 43 (21 between 20:11 and 21:35 UTC; 22 between 22:29 and 22:35 UTC, during that run) | about $2.03 |

- **Also untagged:** two `apify/web-fetch` runs from onboarding 02.
- The windows overlap, so these figures can't be added together.

### 10.6 Money spent so far on SavePet research (Apify)

| Report | Spend |
|---|---|
| Onboarding 01 | $0.00 |
| Onboarding 02 | **reports disagree:** about $0.64 "reported" / about $0.69 with list-price estimates (its §6); "$0.70 to $0.75" (its header); $0.70 across 13 runs (onboarding 03, from `list_apify_runs`) |
| Onboarding 03 | $0.00 (free read of the paid Facebook dataset) |
| Onboarding 04 | $0.00 |
| Onboarding 05 | about $0.00005 (page capture) |
| Telegram 01 | $0.00 |
| Telegram 02 | $1.79 (13 runs, of a $6 cap) |
| Telegram 03 | $0.00 |
| 2026-11-05 (ran 2026-11-06) | $0.00 |
| This compile | $0.00 |
| **Total** | **about $2.43–$2.54** (about $2.49 using the $0.70 `list_apify_runs` figure). The unexplained Facebook Ad Library runs are **not** included. |

### 10.7 Other open items

- **Prompt registry:** every row of the playbook's prompt registry still says `ADD_ID`, and no Supermemory space is named for prompts or evidence. Supermemory was therefore not used in this compile.
- **`RAW_RESEARCH_METHOD.md`:** missing from the SavePet repo (404). It exists only in the main repo.
- **Stale memory:** Supermemory memory `rt13wF2CCVkUvpbA7krzhy` still says SavePet research goes to the main repo. That is wrong; the owner chose `exobvious/savepet-research`.
- **Owner answers still missing:**
  - Are "Made in USA" and "Third-Party Tested" true?
  - Is "My Vereli" the maker?
  - What are the bundle prices?
- **Competitor list:** PawMergency, PetVet Medic, Vetanica and NOW are not yet added to the Competitors list in `PRODUCT_DECISION.md`.
- **Report dates:** the 2026-11-05 report's path is dated 11-05, but it ran on 2026-11-06.
- **Process note:** two proposed `NEVER_REPEAT_MISTAKES.md` lines are waiting (onboarding 03 §9 and 05 §9). The issue: don't queue clean-up, synthesis or deep research before their inputs and registry IDs exist.

---

## 11. Index of source reports

| # | Report | What it holds | Link |
|---|---|---|---|
| 0a | product_truth.md | Product facts | https://github.com/exobvious/savepet-research/blob/main/01_petmergency_activated_charcoal_first_aid/product_truth.md |
| 0b | PRODUCT_DECISION.md | Category, six problems, locked rules | https://github.com/exobvious/savepet-research/blob/main/01_petmergency_activated_charcoal_first_aid/PRODUCT_DECISION.md |
| 1 | Onboarding 01: Reddit Answers bank | Blocked; lesson notes; actor options | https://github.com/exobvious/savepet-research/blob/main/01_petmergency_activated_charcoal_first_aid/bot_reports/onboarding/2026-11-02/01-raw-research-reddit-answers-bank.md |
| 2 | Onboarding 02: other channels | Amazon, YouTube, TikTok, Quora quote bank; competitor listings | https://github.com/exobvious/savepet-research/blob/main/01_petmergency_activated_charcoal_first_aid/bot_reports/onboarding/2026-11-02/02-raw-research-thin-families-on-the-other-channels.md |
| 3 | Onboarding 03: avatar clean-up | Blocked; the 30 Facebook posts read | https://github.com/exobvious/savepet-research/blob/main/01_petmergency_activated_charcoal_first_aid/bot_reports/onboarding/2026-11-02/03-avatar-clean-up.md |
| 4 | Onboarding 04: category context | Blocked; readiness check | https://github.com/exobvious/savepet-research/blob/main/01_petmergency_activated_charcoal_first_aid/bot_reports/onboarding/2026-11-02/04-category-context.md |
| 5 | Onboarding 05: deep research | Blocked; page capture; 16 contradictions; copied reviews | https://github.com/exobvious/savepet-research/blob/main/01_petmergency_activated_charcoal_first_aid/bot_reports/onboarding/2026-11-02/05-deep-research-1-tube-39-95-shown-as-down-from-80.md |
| 6 | Telegram 01: reworded questions | 26 lesson questions, 156 reworded, cat and dog variants (**truncated in reading**) | https://github.com/exobvious/savepet-research/blob/main/01_petmergency_activated_charcoal_first_aid/bot_reports/telegram/2026-11-02/01-reword-reddit-questions.md |
| 7 | Telegram 02: Reddit Answers run | Tier A and B Reddit quotes; fee and hold data; pull log | https://github.com/exobvious/savepet-research/blob/main/01_petmergency_activated_charcoal_first_aid/bot_reports/telegram/2026-11-02/02-reddit-answers-run.md |
| 8 | Telegram 03: avatar copy and check | 66-point check; uncommitted profile copy and product_truth update (**truncated in reading**) | https://github.com/exobvious/savepet-research/blob/main/01_petmergency_activated_charcoal_first_aid/bot_reports/telegram/2026-11-02/03-avatar-copy-and-check.md |
| 9 | Telegram 2026-11-05: 126 unread answers | Tier B P1, P2, P3, P4, P5, P6 items; avatar updates; 18 threads to open (**truncated in reading**) | https://github.com/exobvious/savepet-research/blob/main/01_petmergency_activated_charcoal_first_aid/bot_reports/telegram/2026-11-05/01-read-unread-reddit-answers.md |
| 10 | raw/README.md | Folder note only; no raw files yet | https://github.com/exobvious/savepet-research/blob/main/01_petmergency_activated_charcoal_first_aid/raw/README.md |

**Datasets you can re-read for free (do not buy again):**

| Dataset | What it holds |
|---|---|
| `Da2ivMrrTuvpdIR5n` | Amazon reviews, helpful sort |
| `cxM8wT7E2E0nPOP8e` | Amazon reviews, critical sort |
| `DNJAqKFgeHTwWtV0p` | YouTube comments |
| `yOhyIAyBMiC8IQ0oz` | TikTok comments |
| `uQBfIcoXY0boLKb5r` | Facebook posts |
| `k6m5i9PoGnUih17tH` | Product page capture |
| `edo30btIGF0NdPkvS`, `lPdySNS03gekOd6iv` | Reddit Answers |
| `w0fhweSFZ0i7lN3ew` | 10 opened threads |
| `mLxSIywSyajQGeJxz`, `gYJGjMfzX4hSYgbPd` | r/AskVet and r/DogAdvice searches |

---

*This compile ran no searches, bought nothing, and created no tasks. A quote that appeared in several reports is shown here once.*
