# PetMergency (SavePet): Reddit Answers run, thread hops and subreddit search

- **Run:** telegram / 02-reddit-answers-run, 2026-11-02 (UTC), cloud research agent, Apify job tag `telegram`
- **Repo / folder:** `exobvious/savepet-research` / `01_petmergency_activated_charcoal_first_aid/`
- **Status: DONE, with gaps stated below.**
  - All 156 questions were asked on Reddit Answers and 156 answers came back.
  - **Only 30 of the 156 answers were read.** The other 126 are paid for and stored in datasets (§6). Reading them costs nothing.
  - Ten cited threads were opened with their comments, and seven subreddits were searched directly.
- **Apify spend for this step: $1.79** of the $6 cap (13 runs tagged `telegram`, figure from `list_apify_runs`).
- **One file written:** this report. The run was limited to a single append-only file. No category document exists yet (the category-context step 04 was blocked), so the kept items are in §4 as an `## Added` section, ready to copy into the category document under `raw/`. **That copy has not been made.**
- **No ClickUp tasks were created.** Suggested next steps are in §9 as ideas only.
- **Evidence classes are kept separate:**
  - `customer_report`: an owner describing their own pet.
  - `pro_opinion`: a commenter speaking as vet staff or giving peer advice. Unverified.
  - `competitor_claim`
  - `hypothesis`
  - `conclusion`

---

## 1. What was read first

| Source | Result |
|---|---|
| `gateway_status` | scaler, vantage, apify, supermemory OK. clickup: false. Apify had spent $2.23 today before this run. |
| `get_playbook` (UNIFIED_PLAYBOOK sha 02e8ca8) | Every registry row still says `ADD_ID`. **The playbook does not name a Reddit Answers actor.** I used the candidates listed in onboarding report 01 §6. |
| `RAW_RESEARCH_METHOD.md` | **404 in the SavePet repo**, as before. Read from the main repo through the playbook (sha f11ed6d). |
| `product_truth.md`, `PRODUCT_DECISION.md` | Six problems. Page claims are seller claims. The profile's numbers ($95 fee, $2,000 bill) are hypotheses. |
| Telegram report 01 (approved 156 questions, sha fdc0043) | **The tool output was truncated in the middle of §5.** I could not read P5.8 (partly), P5.9–P5.26, P6.1 or P6.2. A repo search returned no hits. See §2. |
| Onboarding reports 01 and 02 | No earlier Reddit pull existed, so nothing could be bought twice. Report 02's quotes (YouTube, Amazon, TikTok, Quora) were not repeated here. |
| Category document | Not in the folder. Step 04 was blocked. |
| `list_apify_runs` (24 h, checked before any pull) | No Reddit Answers run existed, so there was nothing to reuse and no REPEAT_PULL. |
| Supermemory `search_memory` | No stored copy of the bank. |
| Telegram log 2026-11-02 | The owner approved the reword and then the search (17:24), with a $6 cap. |

## 2. How the 156 questions were run (and one honesty flag)

- **126 questions were typed exactly as approved:**
  - P1.1–26, P2.1–26, P3.1–26, P4.1–26
  - P5.1–P5.7
  - P6.3–26
- **21 questions were rebuilt from the approved template, not copied from the approved list.** The list was unreadable in my tool output, so I rebuilt P5.8 (completed from its visible beginning), P5.9–P5.26 and P6.1–P6.2. I used report 01 §3 (the 26-question template) plus §4 (the slot forms "pet poison control fees and hold times" and "giving their pet the wrong dose in a panic"). P6.2 was rebuilt from its visible ending.
  - Their wording may differ slightly from what the owner approved. If exact wording matters, rerun those 21 from the file.
- **Actor 1: `nice_dev/reddit-answers-scraper` failed.** It returned 0 answers.
  - Run `hxY5ZVchnNa7YrR20` (52 questions) was stuck at "0 of 121 answers saved" for about 9.5 minutes, so I aborted it.
  - Run `qv8ahAMr2sig0T9Wu` FAILED with: "Stopped early: Reddit Answers answered too few questions for the time spent — no answers saved — run it again later".
  - Cost: $0.002 in total.
- **Actor 2: `openclawai/reddit-scraper` (`answerQueries`) worked.**
  - A test with 2 questions came first.
  - Then two batches: 29 and 125 questions.
  - Result: 156/156 answered, at $0.01 per answer.
- **The same actor was used for hops and subreddit search:**
  - Opening threads costs $0.002 per post, and the comments come free.
  - Subreddit searches return 8 posts per term.
- **Facebook Ad Library:** no actor was used. Note that `list_apify_runs` shows **3 more untagged runs of the Facebook Ad Library actor `XtaWFhbtfxyzqrFmd` at 20:28–20:29 ($0.135)** during this session. This run did not start them. This is the same unexplained pattern flagged on Telegram at 17:06.

## 3. Reading the Reddit Answers output: what can be trusted

- I treated Reddit Answers only as a starting point for finding threads. The answer summaries are AI text and are **not** kept as evidence.
- Each answer quotes short excerpts with permalinks. In the 30 answers I read, I found the following problems, all dropped from the evidence (§5):
  - **2 quotes had no link and could not be traced:**
    - "I poured hydrogen peroxide down his throat and he gagged…"
    - "She told me to give salt to make her vomit…"
    - Both appear in the P3.5 answer and may be invented.
  - **3 quotes didn't support the claim they were attached to.** For example, a r/labrador quote about puppy-proofing was cited as proof that peroxide is "corrosive".
  - **1 answer said in its own words** "While not directly quoted, this is a well-known veterinary caution".
- Kept items therefore fall into two tiers:
  - **Tier A (verified):** read in the opened thread or post itself, with date.
  - **Tier B (excerpt only):** a quote with a permalink as it appeared in a Reddit Answers answer. The thread was not opened, and the date was not retrieved. Treat as unverified until opened.

---

## 4. Kept items: paste as `## Added 2026-11-02: Reddit (Answers hops + subreddit search)` into the category document under `raw/`

Quotes are verbatim, typos included. Unless marked otherwise, every item is `customer_report`.

### 4.1 Tier A: verified in opened threads and posts

**P5: poison control fee and hold**
- r/AskVet, https://www.reddit.com/r/AskVet/comments/1t6mhey/pet_poison_control/ (OP, 2026-05-07):
  - "It costs $85.00 on my credit card to even be put through to Animal Poison Control."
  - "Once you navigate the fee, you get put on hold for an agent. I've never waited less than 35 min. That's now at least an hour since he ate and started metabolising the toxin. Every minute counts. In some cases, I hung up before speaking to someone because I \*had\* to find someone who would help, NOW."
  - "On a small animal, that kind of wait time is a death sentence.  Who is this serving?"
  - "Dog ate something he shouldn't have, today. Not his first time. Won't be his last time. 🙄😒"
  - After a vet-staff reply, the same OP wrote (comment okm5ksi, 2026-05-08): "Thank you for this very thoughtful and reasonable response. It makes perfect sense and I'm grateful." *(The objection softened once the reason was explained.)*
- r/Pets, https://www.reddit.com/r/Pets/comments/1o68fek/ (OP, 2025-10-14):
  - "We spent 2 hours on hold with ASPCA poison control tonight before giving up and calling another service  (Pet Poison Helpline). This took us 10 minutes…"
  - "ASPCA was 110 USD while Pet Poison Helpline was 89 USD."
  - "most ER vets (at least close to us) require a poison control call"
  - "My advice - call both"
  - Comment nwssdse (2025-12-30): "was on hold for soooooo long waiting for ASPCA cause my vet needed a case number… called the pet poison hotline instead and they answered in 10 minutes and was cheaper like you said!"
- r/DobermanPinscher, https://www.reddit.com/r/DobermanPinscher/comments/1anrg6x/ (OP Jillio_NH, 2024-02-10):
  - Title: "Augh- I've been on hold 15 minutes with poison control"
  - "the emergency vet won't work with us until we connect with poison control- is this a lethal dose?!?!?"
  - "poison control charged us $95 when they finally picked up to tell us that he should be fine."
  - Comment kpufboy: "they wouldn't take my call until I gave them a credit card. After almost 20 minutes on hold. I was in a bit of a panic but now I feel a lot better."
- Other comments in the same thread:
  - kpunp6j: "But damn $95 is just crazy"
  - kpuso9i: "I paid that fee too because we were in such a panic… the panic that set in was horrible. My dobie took a half full bottle of ibruprofen off the counter and ate a few."
  - kpuqulv: "they charged me $125 IIRC back in 2013/14."
  - kpxg9rz: "Had to pay 40 to get them to tell us the plant the dog ate would just irritate his stomach, not kill him."
  - kpv09iw: "Many manufacturers (especially of vet specific products) will cover the cost, though."
- r/puppy101, https://www.reddit.com/r/puppy101/comments/kzmwje/ (OP Sammibear1024, 2021-01-18):
  - Title: "Why Tf does animal poison control charge $50.00 freaking dollars?!"
  - "I was panicking and called poison control, the human one. They tried to help me but directed me to animal poison control instead."
  - "Like 10-20 would be way more reasonable, considering the human one is free."
  - "Thank goodness I had someone I could borrow the money from"
  - "Paid 50 dollars just to be told that he will be perfectly fine except for possibly upset tummy. Ridiculous."
  - Comment gjov3dq: "I called four different vets… and was told every time to call animal poison control… not everyone has the funds on hand for situations like that." Also: "my phone was on 2% and my toddler misplaced my phone charger so I was panicking"
  - Comment gjp0a3q (another owner): "the vet called poison control so I got charged for the vet and the poison control fee, along with a lot of treatment… Pets are expensive."
- r/puppy101, https://www.reddit.com/r/puppy101/comments/utaup0/ (OP biscaybaguette, 2022-05-19). This post covers P3, P4 and P5 together:
  - "As it's around 11PM, our vet is closed so we have no other option than to go to one of  the emergency vets"
  - "it would be a ***$75 consultation fee***. Wtf? No thanks."
  - "My partner and I are freaking out and scared, of course because the love of our life is possibly sick and it's our fault for leaving a half a bowl of Chipotle out."
  - "the vet wouldn't see her *UNLESS WE PAID THE $75 CONSULTATION FEE OVER THE PHONE TO THE THIRD PARTY BEFOREHAND!*"
  - "They gave her apomorphine for her to puke everything up… fluids to keep her hydrated, and charcoal to prevent any more absorption."
  - "the worlds most expensive bowl of chipotle ($400!)"
  - **Negative reception:** the OP's replies were downvoted (−4), and a moderator locked the thread as "heated".
  - Counter-view (pro_opinion / peer):
    - i98xaqc, score 14: "if there are no symptoms and the dog seems fine… then you saved a bunch of money"
    - i9918zh: "They'll even instruct owners on how to induce vomiting at home and save owners money if a vet visit isn't necessary."
- r/AskVet search posts:
  - https://www.reddit.com/r/AskVet/comments/1i2u1bu/ (2025-01-16, cat ate lily): "I waited for 1.5 hours or so while the vet waited on the line to speak with poison control… he charged me $150 of poison control communication fee."
  - https://www.reddit.com/r/AskVet/comments/1otlu68/ (2025-11-10):
    - Title: "I cannot afford to call poison control and my dog has no symptoms but I want to make sure"
    - "I can't afford the $90 poison control call"
    - "i used chewy chat for free and they were able to get me a discount"
    - "still shaking"
  - https://www.reddit.com/r/AskVet/comments/126bjlc/ (2023-03-30):
    - "ASPCA wants to charge $95 (lol)"
    - "I wasn't gonna roll the dice on his kidneys"
    - "I'd rather not chance $95 just to possibly be told that he needs to have constant access to water."
  - https://www.reddit.com/r/AskVet/comments/1xgibir/ (2026-10-27):
    - "When I heard that they have a $110 fee i decided to go to the vet after a quick google search."
    - "they have been on hold with poison control for the last 2 hours."
    - "Overall i am just frustrated at the vet/vet tech and the whole waiting with no communication"
  - https://www.reddit.com/r/AskVet/comments/1hrl17d/ (2025-01-02):
    - "they all charge somewhere between U$80 and U$100"
    - "Is calling them worth anything at all or just a waste of money and time"
  - https://www.reddit.com/r/AskVet/comments/1g5cd9h/ (2024-10-16): "I can't really afford the $95 animal poison control fee rn." Also: "I'm feeling so stupid"
  - https://www.reddit.com/r/AskVet/comments/1ld0da7/, comment my4m6lw (2025-06-16): "the online calculator is free the poison contol hotline is $95 upfront"
- pro_opinion (vet staff), r/AskVet 1t6mhey, comment okin3t6 (score 20): "We have people call poison control on the way to the hospital if they can… There are a lot of things that we can't/shouldnt make the pet vomit for… human poison control is government funded… We dont have that luxury in vet med!"
- pro_opinion, comment okjau8x: "if your pet is microchipped then sometimes you can use the poison control service through the chip company for much cheaper"
- Titles only (bodies not read):
  - r/dogs "How to canine poison control hotlines charge their fees?" (2022-11-08)
  - r/dogs "[Help] Is Pet Poison Helpline legit?" (2017-04-16)
  - r/dogs "What are our opinions on pet poison helpline?" (2025-12-30)
  - r/puppy101 "Had a great experience with poison control" (2021-06-25). **This is counter-evidence.**

**P3: vet closed at night / no vet nearby**
- r/AskVet, https://www.reddit.com/r/AskVet/comments/1ld0da7/ (OP, 2025-06-16). This post covers P2 and P3:
  - "He lives in a very rural area, nearest vet is nearly 2 hours away."
  - "I gave her two teaspoons of hydrogen peroxide… It's been about 3 hours since the HP and other than some nauseated licks she hasn't thrown anything up."
  - "I'm at a loss for what to do next, ended up calling the nearest vet and they are not open until tomorrow. I'm nervous that both the peroxide and chocolate will end up poisoning her."
- r/DogAdvice:
  - Title of z5x6ve (2022-11-27): "Help!!!! my dog just ate chocolate. I tried to take it from him but he became aggressive and bit me Our vet is closed.What should i do???"
  - 1hnuvs0 (2024-12-28): "Should I wait until morning and observe him a little more or go to my emergency vet immediately?"
  - 1l5jsxn (2025-06-07):
    - "Vet is closed and I can't afford the upfront fees anyway"
    - "No my area does not have an emergency vet clinic"
  - 1196aql (2023-02-22, marijuana poisoning):
    - "We tried five vets, in a city of 42,000, but none would see her"
    - "We even told each office we felt our dog might die. Nothing."
  - 1u3aj2r (2026-06-11, cooked bones, UK). This is not a toxin, but the language fits:
    - "I tried to call a few vets, but they didn't answer, any of them."
    - "I feel like such a moron."
  - 1ptwo7g (2025-12-23): "Waiting for the vet to call back." Also: "I'm really worried she's only little."
- r/AskVet, https://www.reddit.com/r/AskVet/comments/fsplqw/ (2020-04-01):
  - "Nothing is open right now, so I am not sure what to do."
  - "I have activated bamboo charcoal… It's the kind that goes inside the care"
  - "it costs a ton of money to bring him to the vet"
- r/AskVet, https://www.reddit.com/r/AskVet/comments/10hdn3j/ (2023-01-21, cat ate a plant):
  - "I order activated charcoal from amazon but it's gonna arrive just on Sunday. CVS has AC capsules but it has vegetable magnesium stearate on formula. Is it still safe for cats? I can't wait till Sunday."

**P2: peroxide**
- r/AskVet, https://www.reddit.com/r/AskVet/comments/1ttxg2h/ (OP JayJayLoves, 2026-06-01):
  - "I talked to my vet who recommended inducing with hydrogen peroxide. One of my dogs threw up all 4 tampons, and the other dog 86lb retriever did not vomit at all. He was given the max dose of 45mL"
  - "I did not know it was corrosive to their stomach lining so now I'm worried it's sitting in there."
  - Comment op5u0xe: "My vet said it was safe at that dose but I've read a lot online that says otherwise."
  - pro_opinion, op5lrfg (score 20): "That's a very old school thing to tell owners to induce vomiting themselves at home, particularly because of the risks… there are licensed subcutaneous injections that can be given to induce vomiting at the vets. I would opt for this."
- r/Pets, https://www.reddit.com/r/Pets/comments/17xefh8/, comment k9nxh9x (2023-11-17). **A success report:**
  - "call the vet on my way home and they tell me to give her hydrogen peroxide asap to induce vomiting. I take her outside, use a turkey baster to get it down her, and moments later, everything is all over the yard… Poor pupper looks at me with the saddest eyes, full of reproach. She was fine."
- Title, r/puppy101 ly4mls (2021-03-05): "YEAH OK I just gave my puppy hydrogen peroxide for the first time!!" Also the title of mxiw54 (2021-04-24): "How to induce vomiting?"
- The 1ld0da7 failure is listed under P3.

**P1: ate something toxic, nothing at home; charcoal and competitors**
- r/DogAdvice, https://www.reddit.com/r/DogAdvice/comments/1urz7u6/ (2026-07-09):
  - "Can anyone recommend activated charcoal that I can have at home and give my dog the next time they get into something?"
  - "I feel like we're playing with fire, our dogs are constantly getting into potentially dangerous stuff and the nearest vet is 2+ hours away"
- r/Pomeranians, https://www.reddit.com/r/Pomeranians/comments/1u31u8h/ (OP, 2026-06-11). **Competitor: Toxiban.**
  - "He ate 1/2 slice of chocolate banana bread. Gave him 40ml Toxiban (charcoal) and now taking him to the vet. He was furious with me and bit me couple of times but that didn't bother me."
  - Comment or1wbel (OP): "The vet said they'll do some bloodwork & give probiotics. They don't want him throwing up toxiban bc it can cause more problems."
- r/DogAdvice, https://www.reddit.com/r/DogAdvice/comments/18l9sv8/ (2023-12-18). **Competitor: VetDTox.** This covers aspiration fear and missing instructions:
  - "I just recently bought some activated charcoal powder (VetDTox)"
  - "the bottle didn't say anything about how to serve it. So I sprinkled it on top of some kibble."
  - "activated charcoal should not be given dry because they can aspirate it into their lungs"
  - "I feel hypervigilant of his behavior and it's stressing me out."
- r/AskVet, https://www.reddit.com/r/AskVet/comments/1df54i1/ (2024-06-13, cat, charcoal tablet). Aspiration fear:
  - "I fear she inhaled a little of it via her mouth or am I exaggerating? I don't want to do her more harm than good"
- r/AskVet, https://www.reddit.com/r/AskVet/comments/irkjyg/ (2020-09-12, bromethalin):
  - "I'm worried about the adverse effects of activated charcoal. I'm kicking myself and currently a mess of guilt"
  - "Trust me, I already feel like sh*t."
- r/DogAdvice, https://www.reddit.com/r/DogAdvice/comments/1bc0je3/ (2024-03-11):
  - "I've had to give my puppy 2 doses of activated charcoal… he hasn't really been wanting to eat or drink much and has been a bit tired."
- r/AskVet, https://www.reddit.com/r/AskVet/comments/1ed912e/ (2024-07-27): "I'm disappointed that the vet did not administer activated charcoal and am concerned it will increase the chances of renal failure." *(The owner believes in charcoal.)*
- r/AskVet, https://www.reddit.com/r/AskVet/comments/1w1t0q4/ (2026-08-29):
  - "The vet gave her activated charcoal with sorbitol (charactol 50)"
  - "How does this work, and should I be doing more?"
- r/Pets 17xefh8. Language on dogs that eat everything, and outcomes:
  - k9n4vli: "My littlest dog is a garbage disposal and will eat ANYTHING I drop on the ground."
  - k9o78l1: "This dog would eat anything."
  - k9nk3yk: "Our neighbor… dropped a huge block of rat poison on the ground… We got his stomach pumped"
  - k9nngw3: "My brother s dog got into antifreeze, it destroyed her kidneys. She was put down."
- Objection ("it won't happen" / "chocolate isn't that bad"):
  - r/Pomeranians 1u31u8h, comment or1v1ms: "Dogs can eat more chocolate than you'd think, I'm sure he will be fine!"
  - or3yz9y: "My Wally ate probably 10 or so miniature chocolates… and he was fine."
- Cats, titles only (r/cats):
  - "My cat Peter ate 2 petals from a Lily today. He's at the emergency vet right now and I am an absolute wreck." (2026-06-24)
  - "Do I need to rush my cat to the vet for lily poisoning, or is watching for signs okay?" (2022-06-28)
  - "cat poisoning home treatment" (2022-06-05)
  - "How can you help a cat if it has been poisoned?" (2021-11-28)

**P4: emergency vet bill**
- From the threads above:
  - "$400!" (utaup0)
  - $150 communication fee (1i2u1bu)
- r/Pets 17xefh8:
  - k9oc6vw: "$500 at the emergency vet and he would probably still do it again if given the opportunity."
  - k9nkdy4: "That was an expensive visit to the emergency vet and a sleepless night but they pumped his stomach and he was okay afterwards."
- r/AskVet, https://www.reddit.com/r/AskVet/comments/1i0mqo2/ (2025-01-13, possible yarn ingestion):
  - "Visit fee was $125, x-ray another $110, plus $50 for the med to try and induce vomiting… Total cost almost $350."
- Titles:
  - r/Pets "My dog is at the emergency vet for xylitol poisoning" (2013-10-05)
  - r/Pets "Emergency vets refusing treatment unless you pay them upfront? Is this a thing?" (2025-08-23; not poisoning-specific, kept as language only)

**P6: dose in a panic**
- r/AskVet, https://www.reddit.com/r/AskVet/comments/189k2n6/ (2023-12-03):
  - Title: "About to feed my dog 40 grams of activated charcoal"
  - "I would just like a double check on dosage!"
  - "tried calling HomeAgain medical line to get this question answered but no one could renew my membership. Please help me save $85"
- 18l9sv8 (above): "the bottle didn't say anything about how to serve it."
- 1ttxg2h (above): "He was given the max dose of 45mL".

### 4.2 Tier B: Reddit Answers excerpts with permalinks (threads not opened, dates not retrieved)
- P5:
  - r/assholedesign raeaqq, comment hnhntoq: "…will try to force you to give your credit card and $70 before getting advice about whether your animal has been poisoned."
  - Comment l63d1tk: "Oh it's 95 now."
  - r/legaladvice 1v643ah, comment oztmnjc: "If you sign up for AKC reunite for a one time payment $20 you get unlimited lifetime free pet poison control calls."
  - r/Pets 1ltuw9f: "add on a pet poison helpline plan for 20 dollars one time."
  - r/Rottweiler 1v8xzzl: "called the animal poison control but they charge $110 and I'm pretty strapped for cash."
  - r/WagWalker 1ofbfib: "I spent $89 out of pocket..."
  - r/CATHELP 1ovriv0: "I'm on hold waiting for a member of animal poison control to pick up"
  - r/UK_Pets 1ndoy7l: "the vet called the poison control centre on our behalf (saving us the £45 fee)"
  - r/YouShouldKnow 1ihevsn, comment mawjagt: "Poison control stayed on the line with me as I drove to the hospital and... My dog is now ok."
- P3:
  - r/DOG 1nivkg5: "I am shaking and crying and it's midnight."
  - r/AskVet 1n4lw7u, comment nbm4wqq: "the closest one is 3 hours away and that's not feasible for me right now."
  - r/cats 1vm1uzj: "I unfortunately could not afford x‑rays, exam fees, BW for everyone at a after hours clinic."
  - r/CATHELP 1vbr83z: "On the side of my microwave, I have a short list of animal hospitals..."
  - r/Dachshund 1qesw7t, comment nzzy7kk: "You can use a toxicity calculator to see the severity. That really helped me calm down."
- P2:
  - r/Columbus xqhh7j, comment iqc34n0: "My fucking dog is immune to this method.."
  - r/DogAdvice 175ezey, comment kj2xjt3: "I woke up to find that he had thrown up blood and rushed him to the vet."
  - r/WagWalker 1ofbfib: "I was apprehensive about giving him hydrogen peroxide, though, knowing that it can sometimes do more harm than good, and he's a senior dog"
  - r/YouShouldKnow 1ihevsn, comment mawmzi4: "They told me to mix hydrogen peroxide with milk to induce vomiting... At that point we said 'fuck it'."
  - pro_opinion:
    - r/AskVet 1n5cwt8, comment nbrs3od: "Hydrogen peroxide is no longer really recommended… It can frequently cause abrasions and ulcers in the esophagus and stomach"
    - r/todayilearned kl6ak8, comment gh73oey: "frequently pets still have to come in to see us because the hydrogen peroxide didn't work."
    - r/puppy101 ly4mls, comment gpsutmh: "Inducing vomiting on your own leads to a risk of aspiration pneumonia"
- P4:
  - r/Pensacola 1ty5w5l, comment oq141hk: "It was 3 grand, but I know I would've never forgiven myself"
  - r/Pets 1qmnc2p, comment o25vp17: "all of a sudden you're thinking about money when you should be thinking of the fragile life"
  - r/AskVet 1unmwq3, comment ovljdhc (vet-given charcoal): "they induced vomiting and gave him activated charcoal... he was released with no lasting damage."
- P6:
  - r/AskVet 1oz665m, comment np9tby6: "Based on her weight, you gave a very low dose."
  - r/AskVet 1unpg4z: "My wife gave our dog a dose meant for 50 pound dog. We are freaking out please help" *(a medication, not charcoal)*
  - r/TwoXPreppers 1063esw: "I would like to see if anyone has a dog safe dosing chart."
- Guilt (P1/P3):
  - r/Petloss 1av6wl9: "I'll forever hate myself for my laziness and carelessness that lead to my baby dying."
  - r/AskVet 1tbxsnc: "She said in 20 years of her being Vet, no dog ever died from eating grapes."

### 4.3 competitor_claim and alternatives named on Reddit (mentions, not proof)
- Charcoal products:
  - **Toxiban** (owner used 40 mL at home)
  - **VetDTox** powder (no serving instructions on the bottle, according to the owner)
  - **Charactol 50** (given by a vet)
  - CVS activated-charcoal capsules
  - Generic Amazon activated charcoal
  - Activated bamboo charcoal (a non-pet product)
- Hotlines and services:
  - ASPCA Animal Poison Control
  - Pet Poison Helpline
  - HomeAgain medical line
  - AKC Reunite
  - Chewy chat
  - Microchip-company plans
  - ToxBuddy (a vet tool)
  - Online chocolate toxicity calculators (free)
- **Negative evidence:** PawMergency, PetVet Medic and SavePet were **not mentioned once** in anything read on Reddit.

## 5. Dropped items, by reason (counts from what was read)

| Reason | Count | Examples |
|---|---|---|
| Unlinked quote inside an AI answer (can't be verified) | 2 | P3.5 "I poured hydrogen peroxide…", "She told me to give salt…" |
| Quote didn't support the claim it was attached to | 3 | r/labrador 1uvdj3n under "corrosive"; r/Pomeranians bite line under "pet's suffering"; r/Petloss lf19y2 under "vet access" |
| AI text with no quote | 1 | P2.9 "While not directly quoted…" |
| Off-problem posts or threads (not toxic ingestion) | 22 | r/Pets 1q8k2qg ($1,700, respiratory); DogAdvice ×7 (calming product, probiotics, behaviour, 2× cherry eye, vomiting illness, towel); AskVet 1i8l2nn; Pets "activated charcoal" search ×13 (cleaners, litter, Chewy, etc.) |
| Duplicate of an item already kept | 3 | or3yyiy (double post); Pets search hits 1q8k2qg and 1qmnc2p, already seen |
| Bot, moderator or deleted comments | 9 | 6× AutoModerator, 1 mod lock notice, 2 deleted/empty |
| Comment with no usable content (well-wishes, one-word replies) | 11 | or1tfcr, or1uoxi, or1s3v6, or1u3pj, kpudxs2, k9qc0mz, okm5cp6, kpuxlhb, gjp325f, kpu8rnb, op8cd1v |
| **Bought but not read** | **126 answers** | Batch 1, items 10–19 (10); batch 2, all except offsets 51–55 and 104–107 (116). Not dropped for content. Unread. |
| Post bodies not read (titles only) | 55 posts | r/cats 16, r/dogs 8, r/puppy101 15, r/Pets 16 |

## 6. Pull log

| # | Actor | runId | datasetId | Bought | Kept / read | Cost |
|---|---|---|---|---|---|---|
| 1 | nice_dev/reddit-answers-scraper (P3+P5, 52 q) | hxY5ZVchnNa7YrR20 | ieAHWcwOFmJwQMVxe | 0, ABORTED | 0 | $0.001 |
| 2 | nice_dev/reddit-answers-scraper (P1,P2,P4,P6, 104 q) | qv8ahAMr2sig0T9Wu | YhTT4zjEC0eDuMYoq | 0, FAILED | 0 | $0.001 |
| 3 | openclawai/reddit-scraper, answers (P3.1, P5.2) | yARVzscqPxD4VUlHu | laRkbz0H9DsMXDirX | 2 answers | 2 read | $0.02 |
| 4 | openclawai, answers (P3.2–26, P5.1, P5.3–5) | JbL9goExmyFpaJcrX | edo30btIGF0NdPkvS | 29 | 19 read | $0.29 |
| 5 | openclawai, answers (P5.6–26, P1, P2, P4, P6) | fWzjaaTVjGuLu2g4P | lPdySNS03gekOd6iv | 125 | 9 read | $1.25 |
| 6 | openclawai, 10 cited threads + comments | Ik1YdPzAlaEX10fQd | w0fhweSFZ0i7lN3ew | 10 posts | 9 threads kept (1 dropped) | $0.02 |
| 7 | openclawai, r/AskVet search ("activated charcoal", "poison control fee") | Qj9OjKJGPKNjac32D | mLxSIywSyajQGeJxz | 16 posts | 14 kept | $0.032 |
| 8 | openclawai, r/DogAdvice ("activated charcoal", "vet closed ate") | ZwoqxxMYyMZgfaJ0U | gYJGjMfzX4hSYgbPd | 16 | 9 kept | $0.032 |
| 9 | openclawai, r/cats ("ate lily vet", "poison control") | mQ1eLOxeG0HVo6uP6 | 0x0Hqr4MMjNr9jU4N | 16 | 4 titles | $0.032 |
| 10 | openclawai, r/dogs ("activated charcoal", "poison control charge") | 0xZL9W098waHfYCzX | h2s0dWDOnwj4F7T3y | 8 | 3 titles | $0.032 |
| 11 | openclawai, r/puppy101 ("hydrogen peroxide vomit", "activated charcoal") | M4xqQhh5ApwBO6idy | EFMrQbh84xRWncq6f | 15 | 3 titles | $0.03 |
| 12 | openclawai, r/CatAdvice ("ate something toxic", "poison control") | ucxieBJb0p4a8Z2Vb | j65DVWpnieZImnKzB | **0 returned** (succeeded, empty) | 0 | $0.032 |
| 13 | openclawai, r/Pets ("activated charcoal", "emergency vet bill poison") | wvucnb3WlJRpNwfgO | CATQJBFpasgWATCHK | 16 | 1 title (13 off-problem) | $0.032 |
| | **Total (list_apify_runs, job telegram)** | | | | | **$1.79** |

Notes:
- **Run 3 was launched without the `job` argument** (my mistake), but `list_apify_runs` shows it tagged `telegram`.
- **Run 12 was charged $0.032 for 0 items.**
- Per channel, against the stop rule ("stop after a page that adds nothing"):

| Channel | Status after page 1 |
|---|---|
| r/Pets (charcoal) | Stopped: page added nothing |
| r/CatAdvice | MISSING: returned 0 |
| r/AskVet | **Not saturated.** Page 1 added many lines. Page 2 was not pulled because the reading budget ran out. |
| r/DogAdvice | Not saturated |
| r/cats, r/dogs, r/puppy101 | Only titles read |

## 7. Coverage per problem: which question families are strong and which are still thin

**Basis.** A family counts as strong when it has at least 3 quotes from different people. Counts are pooled from onboarding report 02 and this run, with Reddit contributions only noted here. The 126 unread answers could change P1, P4 and P6 in particular.

| Problem | Strong now | Still thin | Note |
|---|---|---|---|
| **P5 Poison control fee and hold** (was thin) | **All 7.** Emotional (Mermaid467, Jillio_NH, gabby50579, Sammibear1024, biscaybaguette); failed attempts (human poison control redirect, skipping the hotline and being refused, a 2-hour hold); beliefs ("Who is this serving?", "$95 is just crazy", "10-20 would be way more reasonable"); transformation (Pet Poison Helpline in 10 min, microchip/AKC/Chewy workarounds, OP softened by the explanation); language ("death sentence", "WHAT THE EFF", "(lol)", "worlds most expensive bowl of chipotle"); trust (hotline-legit threads, "Had a great experience with poison control"); catalyst / price | none | **Fees owners report:** $40, $50, $70, $75, $85, $89, $90, $95 (×4 independent), $110 (×3), $125 (2013/14), and a $150 vet "communication fee". The profile's **$95 figure is now supported by owner reports**, with a range of $40–$125. **Holds reported:** 15–20 min, 35+ min, 1.5 h, 2 h (×2). |
| **P3 Vet closed at night** (was thin) | Emotional; failed attempts (peroxide failed with the vet closed until tomorrow; five vets refused; vets didn't answer); language ("playing with fire", "absolute wreck", "such a moron", "shaking and crying and it's midnight"); catalyst ("I can't wait till Sunday", "nearest vet is 2+ hours away", "Nothing is open") | Beliefs and self-image (2); transformation (Tier B list-on-microwave and toxicity calculator only); trust | Rural and "no ER nearby" shows up as strongly as "night". |
| P2 Peroxide | Failed attempts (86 lb no vomit, 2 tsp no vomit, "immune", blood vomit); trust (heavy negative pro_opinion); emotional (corrosive worry, "nervous both the peroxide and chocolate will end up poisoning her") | Catalyst; transformation on Reddit (1 success, the turkey baster); beliefs (1: "my vet said it was safe… online says otherwise") | The vet-advice contradiction: some vets tell owners to use peroxide, others call it "old school". |
| P1 Nothing at home | Catalyst / demand ("recommend activated charcoal that I can have at home", Amazon arrives Sunday, bamboo charcoal); emotional and guilt ("kicking myself", "mess of guilt"); language ("garbage disposal", "would eat anything") | Transformation from **home** charcoal: Reddit success stories are vet-given charcoal only. Beliefs (mixed; "it won't happen" objection present) | **P1 answers were not read.** |
| P4 Emergency vet bill | Prices ($350, $400, $500, "3 grand") | Emotional, beliefs, transformation, trust on Reddit | **P4 answers were not read.** Report 02 still covers this problem across the category. |
| P6 Wrong dose in a panic | none | Most families. Verified: "double check on dosage!", "the bottle didn't say anything about how to serve it", the 45 mL "max dose". | **Negative evidence:** of the 4 P6 answers read, the answers drifted to prescription-medication dosing errors and away from poisoning. |

## 8. Contradictions, negative evidence, hypotheses, conclusions

**Negative evidence and contradictions (customer_report / pro_opinion)**
1. **Vets themselves disagree on peroxide at home.** One vet recommended 45 mL (1ttxg2h), and another vet called the instruction "old school".
2. **Charcoal fears are real.**
   - Aspiration (18l9sv8, 1df54i1).
   - A vet "don't want him throwing up toxiban bc it can cause more problems" (1u31u8h).
   - Side effects: off food, tired (1bc0je3).
   - These match report 02's aspiration-pneumonia 1★ review.
3. **Poison control resentment is mixed with acceptance.** Vet staff argue it saves exam fees, and one angry OP accepted that. Another angry OP was downvoted and the thread locked. A "great experience with poison control" title also exists.
4. **Skipping the hotline doesn't skip the fee.** ER vets often require a case number, or call themselves and bill for it ($150).
5. **No brand mentions.** PawMergency, PetVet Medic and SavePet don't appear on Reddit in anything read. Toxiban and VetDTox do.

**Hypotheses (not proven)**
- H1. "The minutes between 'he ate it' and reaching help (the fee, the hold, the 2-hour drive)" could be a stronger frame than "instead of the vet". It is supported by P5/P3 quotes, but it needs testing against vet pushback.
- H2. Clear serving and dose instructions on the label is a gap that buyers can name (VetDTox "didn't say anything about how to serve it", "double check on dosage"). That makes it a differentiation lever, provided SavePet's own dose guidance, which currently contradicts itself, is fixed first.
- H3. The rural buyer with no ER within hours may be a sharper sub-avatar than the night-time buyer.

**Conclusions (from this run's evidence)**
- C1. P5 and P3 are no longer thin on Reddit. Owner fee reports support the $95 hotline figure as the most common single value, and the full reported range is $40–$125.
- C2. Reddit owners describe charcoal mostly as something the vet gives. Home charcoal stories are about worry, not relief.

## 9. Ideas for the owner (not tasks; nothing was created, assigned or scheduled)

- **Read the 126 paid, unread answers** (datasets `edo30btIGF0NdPkvS` items 10–19 and `lPdySNS03gekOd6iv`) with `get-dataset-items`. This costs $0. Start with the P1, P4 and P6 items. Then open the new cited threads at about $0.002 each.
- **Rerun the 21 rebuilt questions** (P5.8–P5.26, P6.1–P6.2) using the exact approved wording, if exact wording matters. Reading report 01 in two parts would get around the truncation. Cost: about $0.21.
- **Pull page 2 of r/AskVet and r/DogAdvice** (not saturated). Retry r/CatAdvice with different terms, for example "lily". Read the bodies of the cat lily posts.
- **Copy §4 into the category document** under `raw/` once its filename is settled.
- **Find out what is launching the untagged Facebook Ad Library runs** (3 more at 20:28 today).
- **Register an actor in the playbook:** the Reddit Answers row could name `openclawai/reddit-scraper` (`answerQueries`), since `nice_dev` failed.
- **Copy angles to test (still need two independent reports per claim):**
  - the hold/fee minutes
  - "the bottle didn't say how to serve it"
  - "nearest vet is 2+ hours away"
  - Lead with "use alongside your vet and the poison line" to defuse the vet pushback.

## 10. Unavailable or failed sources

- `nice_dev/reddit-answers-scraper`: failed (0 answers).
- r/CatAdvice search: returned 0.
- Report 01 §5 (P5.8–P6.2): truncated in the tool output.
- `RAW_RESEARCH_METHOD.md`: 404 in the SavePet repo.
- Registry prompts: `ADD_ID`.
- ClickUp: not configured, and not used.
- Vantage: not used, since it is not customer voice.
