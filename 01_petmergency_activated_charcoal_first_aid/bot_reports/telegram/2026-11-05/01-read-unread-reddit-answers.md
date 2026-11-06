# PetMergency (SavePet): reading the 126 unread Reddit Answers outputs (Tier B buyer language only)

- **Run:** telegram / 01-read-unread-reddit-answers. The file path is dated 2026-11-05 as instructed. The work actually ran on 2026-11-06, about 22:00–22:45 UTC, by the cloud research agent.
- **Repo / folder:** `exobvious/savepet-research` / `01_petmergency_activated_charcoal_first_aid/`. The brand is SavePet. "SavePets" and "PawMergency" on the product page are mistakes.
- **Status: DONE.** All 126 answers that were paid for on 2026-11-02 and never read have now been read:
  - dataset `edo30btIGF0NdPkvS`, items 10–19
  - dataset `lPdySNS03gekOd6iv`, all 116 items not read before
- **Apify spend for this step: $0.00.** No actor was started. Only `get-dataset-items` reads were used. See §8.
- **One file written:** this report.
- **No ClickUp tasks created.** ClickUp is not configured, and creating tasks is against the rules anyway. Ideas are in §6 and §7 only.
- **Evidence rules applied.** The Reddit Answers summaries are AI text and are **not evidence**.
  - The only things kept are short excerpts that sit inside a Reddit permalink in those answers. They are copied verbatim, typos included.
  - Every kept item is **Tier B**: excerpt only, thread not opened, date unknown. Treat each one as unverified until its thread is opened.

---

## 1. What was read, and dataset problems

**Read first**

| Source | Result |
|---|---|
| `gateway_status` | apify, vantage and supermemory are up. **Scaler is disconnected** (refresh token invalid). Scaler was not needed: this step runs no course prompt. ClickUp: false. The gateway's default repo is `exobvious/research`, so every read and the publish passed `repo: exobvious/savepet-research`. |
| `get_playbook` (sha 02e8ca8) | Every registry row still says `ADD_ID`. **No Supermemory space is named** for the course method or for evidence, so Supermemory was not used. No course prompt was run or rebuilt. |
| Telegram report 02 (sha f66bec6) | Read in full: which 30 answers were read, the dataset IDs, the Tier A/B rules, and the kept items in §4 (used to drop repeats). |
| Telegram report 01 (sha fdc0043) | **Truncated again** in the tool output, from partway through §5 (P5.8) to P6.2, as on 11-02. Repo search returned no hits. The questions inside the dataset showed the wording actually run, so nothing below depends on the missing lines. |
| `product_truth.md` (a2a4a93), `PRODUCT_DECISION.md` (3f08d1e) | Six problems. Page claims are seller claims. Profile numbers are hypotheses. |
| Telegram report 03, avatar check (sha 1355382) | **Truncated** in the tool output after point W5. A re-read gave the same cut, and repo search returned 0 hits. I could see **49 of the 66 points** (B1–B8, C1–C5, P1–P6, E1–E5, F1–F5, R1–R5, H1–H5, S1–S5, W1–W5). The other 17 (W6 onward, objections and so on) **could not be read**. §5 updates only visible points, plus the profile's objections, which appear in Appendix A of that report. |

**Datasets.** Both IDs worked, so `list_apify_runs` was not needed to find them.

| Dataset | Items | Read now | Map (dataset order is not question order) |
|---|---|---|---|
| `edo30btIGF0NdPkvS` | 29 | items 10–19 | 10 = P3.13, 11 = P3.14, 12 = P3.12, 13 = P3.15, 14 = P3.16, 15 = P3.17, 16 = P3.18, 17 = P3.19, 18 = P3.20, 19 = P3.21 |
| `lPdySNS03gekOd6iv` | 125 | 0–50, 56–103, 108–124 (116 items) | 0–20 = P5 (P5.6–P5.26, mixed order). 21–45 and 47 = P1. 46 and 48–72 = P2. 73–98 = P4. 99–124 = P6. Already read on 11-02: 51–55 (P2.5–P2.9) and 104–107 (P6.7, P6.6, P6.8, P6.9). |

**Dataset problems found**

1. **Three answers came back empty:**
   - P1.12 (offset 30)
   - P2.19 metaphors (offset 63)
   - P4.26 emotional state (offset 96)
2. **Two answers were refused by Reddit Answers** ("Reddit doesn't provide responses to some prompts, including those that are potentially unsafe…"):
   - P2.2 (offset 46)
   - P2.23 (offset 67)
3. **Read order changed.** The tool returns each page twice (content plus structuredContent), which overflowed the output. I re-read in pages of 4–6 items with `fields=query,markdown`.
   - The P1, P4 and P6 pages were read first, then P2, P3 and P5, as asked.
   - Exception: edo items 10–14 (P3) were read first, in the test page.
   - In the P6.17 page (offset 115), a few middle lines were cut from both copies. The visible lines around the gap were medication-schedule material (CatAdvice 1v0coi5), not poisoning.
4. **The 21 questions that report 02 rebuilt** (P5.8–P5.26, P6.1–P6.2) appear in the dataset in their rebuilt wording. Wording versus the approved list can't be checked, because report 01 is still truncated.
5. **The same quote appears under different permalinks** in different answers, 5 times. Two kept items are flagged with both links (P2-20, P2-21). The other three were dropped (§3).

---

## 2. Kept items, ready to paste

Paste the block below into the category document under `raw/`. **Every item is Tier B** (excerpt only, thread not opened, date unknown). Unless marked otherwise, items are `customer_report`. Other tags used:

- `customer_report (caretaker)`: a dog walker or pet sitter.
- `pro_opinion`: a vet-staff or peer advice comment. Unverified.
- `[context not stated]`: the excerpt doesn't show that the case was a poisoning.

Nothing here repeats an item kept on 11-02. Where a comment kept on 11-02 shows new words here, only the new words are given, marked "(new words)".

```markdown
## Added 2026-11-05: Reddit Answers (unread 126)
All items Tier B: excerpt quoted inside a Reddit Answers answer, permalink as given there, thread not opened, date unknown. Verbatim, typos kept.

### P1: ate something toxic, nothing at home
**Keeping charcoal / a kit at home (demand and catalyst)**
P1-1. "Eventually I just kept activated charcoal at hand just in case she ingested something." https://www.reddit.com/r/DogAdvice/comments/1hji198/took_my_dog_to_the_emergency_vet_at_5am_and_still/
P1-2. "Considering all of my meds would be fatal for her I try my best to be extra careful." (same post)
P1-3. "I now keep activated charcoal & hydrogen peroxide on hand for emergencies." https://www.reddit.com/r/DogAdvice/comments/158xlnj/comment/jtcoor7/
P1-4. "I would now have charcoal on hand in case he decides to scruff down some pills again." https://www.reddit.com/r/DobermanPinscher/comments/1anrg6x/comment/kpujlk8/ (thread opened on 11-02; this comment was not kept then)
P1-5. "keeping activated charcoal with my pet supplies." https://www.reddit.com/r/LifeProTips/comments/507912/lpt_you_can_save_money_and_potential_worry_after/
P1-6. customer_report (caretaker): "I carry a 1st aid kit in my car. It includes Hydrogen Peroxide with a baby medicine syringe to get it down the dog or if vomiting is not recommended I carry activated charcoal." https://www.reddit.com/r/WagWalker/comments/1ofbfib/comment/nldsw67/
P1-7. "I’ve sorted out a decent first aid kit for the family but then it hit me I’ve got nothing set aside for the dog." https://www.reddit.com/r/UKPreppers/comments/1o904o0/do_you_keep_extra_meds_for_pets/
P1-8. "I wanted to make a list of what NOT to feed a dog to put up on the fridge for my family to reference." https://www.reddit.com/r/DOG/comments/1jj733g/poison_dog_food_guide/
P1-9. "moving forward we definitely don’t feel comfortable using mice bait in the home." https://www.reddit.com/r/dogs/comments/vzpb01/comment/ig9qxhy/

**What they tried that didn't help**
P1-10. "My parents said to give her milk and I did i don't want to do I'm very worry" https://www.reddit.com/r/Pets/comments/1is1hx4/i_need_help_i_think_my_dog_ate_poison_and_dont/ (title slug: "i need help i think my dog ate poison and dont…")
P1-11. pro_opinion (vet staff, anecdote): "Finally she told us she had given him blended milk and garlic to settle his stomach. Poor guy didn’t make it." https://www.reddit.com/r/veterinaryprofession/comments/1rurzfk/home_remedies/

**Fear, guilt, self-blame (language)**
P1-12. "I know I’m such a dumbass but I need help idk how many she ate but there were quite a few and she ate the wrapper and all I’m so worried and feel like a terrible dog mom :(" https://www.reddit.com/r/DogAdvice/comments/1rcuag3/hey_guys_im_severely_worried/
P1-13. (new words) "I am shaking and crying and it’s midnight and I freaking hate myself." https://www.reddit.com/r/DOG/comments/1nivkg5/followed_my_vets_advice_and_now_im_finding_out_i/
P1-14. "I can't afford another $4,000 surgery and I'm terrified he's going to eat something that kills him before I can stop it." https://www.reddit.com/r/DogAdvice/comments/1quc75f/my_dog_eats_everything_dangerous_despite_training/ — FLAG: the same post contains "playing jackpot city", which may be casino spam. Verify before use.
P1-15. "I just don’t want to lose her. 💔🙏🏻" https://www.reddit.com/r/Indiedogs/comments/1vtuqff/dog_has_ingested_something_poisonous/
P1-16. customer_report (caretaker): "The internet was telling me that grapes can be toxic even in very small quantities and I was just at a loss." / "I was kind of panicking and not really thinking straight." https://www.reddit.com/r/WagWalker/comments/1ofbfib/what_would_you_do_if_a_dog_ingests_something/
P1-17. "I have no money so I hung up and called the emergency hospital. They said I could come in but doesn’t recommend because it’s currently a lightning storm and I’m sixteen." https://www.reddit.com/r/PetAdvice/comments/1vid717/i_think_i_accidentally_killed_my_dog/
P1-18. customer_report (friend's dog): "I specifically told her I knew the danger and totally dropped the ball." https://www.reddit.com/r/breakingmom/comments/wrxfn4/im_a_dirtbag_who_poisoned_my_friends_dog/ and "Thank you, yes it was an accident of course but I could have prevented it in so many ways." https://www.reddit.com/r/breakingmom/comments/wrxfn4/comment/ikv2sme/
P1-19. "I have grappled with the last month with dark ideas thinking I may have accidentally poisoned him with rogaine." https://www.reddit.com/r/Petloss/comments/1f2x053/a_month_later_i_called_the_vet_for_closure/
P1-20. "I’m feeling a little less frantic now." / "SUCH A RELIEF." https://www.reddit.com/r/Rottweiler/comments/1v8xzzl/my_dog_ate_around_a_quarter_or_maybe_a_little/
P1-21. "I was ready to cry because I thought my dog for sure going to die. She checked her blood work and said everything looks fine for now, gave her a vitamin k injection and gave me tablets to take home for a month." https://www.reddit.com/r/Pets/comments/1wxag3e/i_think_my_dog_might_have_ate_tomcat_poison/
P1-22. "I got nervous after googling it and decided to take her to the ER vet." https://www.reddit.com/r/CatAdvice/comments/1x4enbv/am_i_an_idiot_for_taking_my_cat_to_the_er_vet/ (cat; title slug "am i an idiot…")
P1-23. "I also hate when they say "this warrants a vet trip" without specifying if the vet trip needs to be within the hour, or within the day." and "I was very anxious because all I'd read said it was a big emergency and the vet didn't seem to think so." https://www.reddit.com/r/redditonwiki/comments/1uzruee/comment/oyb6yaj/
P1-24. "Every God dang website I've come across says that everything is toxic to my dog, even if they're referencing a substance that has to be ingested by the half ton to be deadly." https://www.reddit.com/r/unpopularopinion/comments/fkhuus/pet_health_advice_should_not_always_consist_of/

**Outcomes (vet-treated, not home charcoal)**
P1-25. "When they finally take her back they find out she’s been internally bleeding, needs two plasma transfusions, and tell me she wouldn’t have made it through the night." / "So two plasma transfusions later, 7 follow up vet appointments, and lots of Vitamin K we think we are in the clear." https://www.reddit.com/r/dogs/comments/vzpb01/my_dogs_behavior_changed_after_being_poisoned/
P1-26. "My 40 lb dog survived eating 20 pieces of xylitol gum. It was touch and go for the first 24 hours." https://www.reddit.com/r/DogAdvice/comments/1qgvw0y/comment/o0go60n/
P1-27. "Took him to the emergency vet, they induced vomiting, gave him fluids and antacids, and watched him overnight." https://www.reddit.com/r/AskReddit/comments/1q4qlj1/comment/nxuhyf3/
P1-28. "I month later she’s still not doing that well, it has been a year now and she’s ok as far as being a regular dog but nothing close to her intelligence" https://www.reddit.com/r/AskVet/comments/18lphw7/poisoned_how_long_do_i_have_left_with_her/

**Objection: "it won't happen / he'll be fine"**
P1-29. "He also got into MOUSE POISON and ate a pellet and never got sick, I swear this dog is indestructible." and "I grew up with the notion that even the tiniest bit of chocolate would kill a dog. Last year my boyfriends northern dog got into an entire double-stacked box of assorted chocolates, ate them all and didn't bat an eye." https://www.reddit.com/r/Pets/comments/s40foh/comment/hso6qm3/
P1-30. "My old pitbull ate a plate of 8 lava cakes once. I was pissed, he was completely fine, we no longer have barstools next to the counters" https://www.reddit.com/r/Rottweiler/comments/1v8xzzl/comment/p09vx5y/
P1-31. "My dog once found and ate the carcass of a rabbit in my yard and was totally fine." https://www.reddit.com/r/RoverPetSitting/comments/1v6m0zs/comment/ozrt28r/
P1-32. (peer reassurance) "if it’s anything that’ll make her sick, she’ll throw it up." https://www.reddit.com/r/puppy101/comments/1lsoj3y/comment/n1k6bov/ and "I expect your dog will be ok." https://www.reddit.com/r/Rottweiler/comments/1v8xzzl/comment/p09uhuy/
P1-33. "I truly thought the inhaler was safe because he had never shown any interest before." https://www.reddit.com/r/petsitting/comments/1vdu8go/warning_story_relayed_to_me_about_leaving_things/
P1-34. "These traps are labeled pet & kid safe. No pets & kids can easily access the bait but the rodents can exit the traps with chunks/almost a full block of bait." https://www.reddit.com/r/AnimalAdvice/comments/1w3q0az/these_traps_are_not_pet_proof_emergency_treatment/

**Hurtful or blaming lines (peer)**
P1-35. "Go to the vet anyways. Would you rather your dog die?" https://www.reddit.com/r/Pets/comments/1is1hx4/comment/mdcyl5w/
P1-36. Linked part only: "get” a dog, you take on that responsibility." https://www.reddit.com/r/DogAdvice/comments/1hji198/comment/m37pa8e/ (the preceding words, "Get your shit together. The second you decide to", sat outside the link in the answer)
P1-37. "What dog owner in their right mind would grow grapes on their property in an area their pet can get to?" https://www.reddit.com/r/PetAdvice/comments/1vrrqw6/comment/p4g6p4s/
P1-38. "If you handle poisons, chemicals, or hazardous/toxic materials, then be a fucking responsible adult and put them away properly." and "If I hadn't taken her and she had eaten the poison, she would bleed out internally in a few days" https://www.reddit.com/r/pitbulls/comments/1wuaak3/psa_lock_hazardous_things_up_and_away_from_animals/
P1-39. "Many of you chose to ignore that and borderline berate me. Fuck you :)" https://www.reddit.com/r/DogAdvice/comments/1vy8r82/not_sure_what_to_do/ [context not stated]

**Language for "dogs that eat everything"**
P1-40. "He was like a vacuum!" https://www.reddit.com/r/puppy101/comments/16jn9ib/comment/k0qu1lb/ ; "Sydney had the original cast-iron stomach." https://www.reddit.com/r/puppy101/comments/16jn9ib/comment/k0qxqwa/ [context not stated]
P1-41. "They ate a whole bag of rat poison like it was a bag of Doritos" https://www.reddit.com/r/animation/comments/1rjw27o/comment/o8gpmzy/ (a friend's dogs)
P1-42. "Dogs will get into anything when determined enough." https://www.reddit.com/r/breakingmom/comments/wrxfn4/comment/ikvpjel/
P1-43. "Why is my puppy trying to eat everything? She wants to try to attack deer? Like where is your self preservation?" https://www.reddit.com/r/puppy101/comments/jqkjv0/comment/gbo8m75/

**Trust and vet pushback: pro_opinion (unverified)**
P1-44. "If your dog ate actual poison, pet poison control is only going to direct you to go to the vet. There's no home remedy for a poisoned dog." https://www.reddit.com/r/Pets/comments/1is1hx4/comment/mdczwjg/
P1-45. "decontamination AKA "Vom-it, Bind-it, Dilute-it" AKA make him vomit, bind the toxin with activated charcoal/carbon, and dilute it with high load IV fluids." https://www.reddit.com/r/Rottweiler/comments/1v8xzzl/comment/p0boa29/
P1-46. "Be careful with activated charcoal. You can overdose your pet on it. I have seen a dog die from this." https://www.reddit.com/r/LifeProTips/comments/507912/comment/d7232qu/
P1-47. "Not deciding they’re an expert and giving activated charcoal or using hydrogen peroxide UNLESS advised by a medical professional." https://www.reddit.com/r/AnimalAdvice/comments/1w3q0az/comment/p73t58v/
P1-48. "Emergency vet ASAP; this can't be treated at home." https://www.reddit.com/r/AskVet/comments/1c17ad1/comment/kz1htz2/
P1-49. Linked part only: "home observation” never go together!!!" https://www.reddit.com/r/AskVet/comments/1oiwwhx/comment/nlyut6b/ (the words "ER!! Fyi, for future reference “toxicity” and" sat outside the link)
P1-50. "there are a lot of toxins that START with GI issues and then can cause kidney / liver issues - just because we’re not vomiting any more doesn’t necessarily mean we’re OK." https://www.reddit.com/r/AskVet/comments/1p4w9tn/comment/nqh5fc7/
P1-51. "Human meds are one of the top reasons pets end up in emergency hospitals. Even one pill can be life-threatening." https://www.reddit.com/r/Pets/comments/1o3cpub/we_see_this_almost_every_day_in_the_er_human_meds/
P1-52. (peer, on using ChatGPT to identify plants or pills) "EXREMELY bad at iding things, so its completely unsafe to use." https://www.reddit.com/r/puppy101/comments/1lsoj3y/comment/n1kiw0m/
P1-53. Vet judging the owner: "They immediately accused me of leaving out Thc for my dog to consume, despite my insistence that her flea collar had disappeared" https://www.reddit.com/r/AskVet/comments/1h4xkvc/emergency_vet_suggested_euthanasia_and_that_i/ ; "it seemed like they preferred to ignore my input on what was possibly happening to my dog" https://www.reddit.com/r/AskVet/comments/1h4xkvc/comment/m035nwe/

### P4: emergency vet bill
**Bills tied to an ingestion**
P4-1. "My 80lb German Sheppard ate a full container of Ice Cubes black cherry gum... 2500 dollars later and I took him home the next day." https://www.reddit.com/r/Pets/comments/17xefh8/comment/k9ojuej/ (thread opened on 11-02; this comment was not kept then)
P4-2. "Over two thousand spent from my bf’s 401k and we will have zero moneys by the end of treatment." https://www.reddit.com/r/legaladvice/comments/1v643ah/landlord_didnt_complete_inspection_and_my_cat_ate/ (cat; the substance is not shown in the excerpt)
P4-3. "Emergency vet is $900 and ours is waaay cheaper, however opens in 2 hours." https://www.reddit.com/r/DogAdvice/comments/1o5jhd5/please_help_emergency_situation/
P4-4. "The exam fee is $175, they recommended inducing vomiting for an extra $130, which did not work." / "I'm so broken, but my girlfriend is even more broken." https://www.reddit.com/r/Pets/comments/1xlef2m/i_dont_know_what_to_do/ (the answer calls it a kitten that ate fabric, so a foreign body, not a toxin)
P4-5. "...I was relieved to be stuck with a $500 bill rather than a potential $8,000 one if he needed major surgery." https://www.reddit.com/r/Dogowners/comments/1tuey5y/what_you_should_do_if_your_dog_eats_a_tampon_psa/ (tampon)
P4-6. "I wish I took her to the vet the day before but I knew that if this was something bad enough then they would just keep her and put her down and my mom would be going into debt to have them tell us god knows what." https://www.reddit.com/r/Advice/comments/1r71k56/i_think_my_dogs_are_being_poisoned/
P4-7. "obviously im so relieved shes okay but 500$ 😮‍💨" https://www.reddit.com/r/cats/comments/1ttu57o/500_vet_bill_and_she_was_fine/ [context not stated]
P4-8. "Paid 4K for emergency services for my cat. They couldn’t find anything wrong and eventually was fine." https://www.reddit.com/r/cats/comments/1ttu57o/comment/op4xxjm/ [context not stated]
P4-9. "They had required that we pay for an estimate of services before the admission and treatment and the total came out to $2400 dollars." https://www.reddit.com/r/AskVet/comments/ol79rm/we_paid_a_significant_amount_of_money_for/ [context not stated; the dog died]

**Walk-in and after-hours fees**
P4-10. "it’s highway robbery when they charge you 700 just to walk in the door!" https://www.reddit.com/r/rant/comments/1bgntw6/comment/kynrnlw/
P4-11. "they could bring the cat by the 'after hours' clinic - starting with an admission fee of $500." https://www.reddit.com/r/unpopularopinion/comments/exc1od/if_people_value_pet_lives_so_much_vet_clinics/

**Bill language from non-poisoning cases (language only; leave these out of poisoning bill ranges)**
P4-12. "That visit alone cost $2,000, which I put on CareCredit because there was no other option." / "What breaks me is that the alternative that’s been quietly mentioned is euthanasia if surgery isn’t possible." / "I just feel desperate, scared, and out of options." / "Payment can be figured out later, I'll bleed out my personal credit card if need be" / "I have signed up for pet insurance so this doesn't happen again" https://www.reddit.com/r/Pets/comments/1qx77vm/unable_to_pay_emergency_vet_bill/
P4-13. "This is her baby and now she is seemingly going to have to suffer and probably pass away because we’re too broke to pay for treatment." https://www.reddit.com/r/Pets/comments/1xlef2m/i_dont_know_what_to_do/
P4-14. "My SIL and her family have a small dog... They refused to treat the dog without payment upfront." https://www.reddit.com/r/Pets/comments/1my7v5p/emergency_vets_refusing_treatment_unless_you_pay/
P4-15. "absolutely wouldn't be able to afford $1500+ on a sudden unplanned bill." https://www.reddit.com/r/PetPeeves/comments/1ijl060/people_that_say_if_you_cant_afford_thousands_on/ (title slug: "people that say if you cant afford thousands on…")
P4-16. "I know the dread of an emergency vet bill hangs over my head and I'm not even financially destitue right now." / "I sure as shit don’t have an extra thousand just sitting around." https://www.reddit.com/r/PetPeeves/comments/1ijl060/comment/mbfakzy/
P4-17. "I know that if something like this happens again, I won’t be able to afford it." https://www.reddit.com/r/Pets/comments/1bekyem/my_dog_is_at_the_emergency_vet_im_heartbroken_and/
P4-18. "My wife thinks I overreacted, and wasted $135." https://www.reddit.com/r/DogAdvice/comments/1vxswtz/did_i_overreact_by_going_to_urgent_vet/ (limp, not poisoning)
P4-19. Hurtful lines: "If you can't afford it you shouldn't have the animal." https://www.reddit.com/r/unpopularopinion/comments/fkhuus/pet_health_advice_should_not_always_consist_of/ ; "Pets are a luxury." https://www.reddit.com/r/Pets/comments/1o7lkf1/comment/njoqgci/

**Insurance pays after the fact (avatar point S5)**
P4-20. "Pet insurance, or in my experience with lemonade still requires you to pay for the procedures then they reimburse you after the fact" https://www.reddit.com/r/dogs/comments/1wsh2xe/comment/pclc684/
P4-21. "Our Figo won’t pay unless we prove we paid the bill in full first." https://www.reddit.com/r/Pets/comments/1o7lkf1/comment/nn721es/
P4-22. "Even with insurance you have to be able to pay upfront before they reimburse you." https://www.reddit.com/r/Pets/comments/1vs0u9a/handling_pet_vet_bills/
P4-23. "I did have to pay first then get reimbursed from Pets Best." https://www.reddit.com/r/petinsurancereviews/comments/1te23ss/comment/pd4kd47/
P4-24. "Unfortunately no insurance will cover treatments for an already sick kitty, just like you can’t get home insurance after the earthquake." https://www.reddit.com/r/PetAdvice/comments/1lfo0f8/comment/mypsin9/
P4-25. Counter-evidence: "It saved me over $20,000 in one year with my dog." https://www.reddit.com/r/Pets/comments/1xlef2m/comment/19rzwran8jneo/ ; "Pet insurance. It’s expensive, but it’s saved us a few times now." https://www.reddit.com/r/Pets/comments/1o7lkf1/comment/njoht1h/ ; "The peace of mind with pet insurance is knowing a lifesaving surgery or emergency intervention is possible and won’t destroy my savings." https://www.reddit.com/r/petinsurancereviews/comments/1si97ym/comment/ofik0er/
P4-26. customer_report (caretaker): "I have insurance for this so I never have to hesitate about taking a client in for emergency care." https://www.reddit.com/r/WagWalker/comments/1ofbfib/comment/nl8e69j/
P4-27. "Pet insurance plus I put 80 bucks a month into what I call my Dog Colleage Fund account." https://www.reddit.com/r/dogs/comments/1wsh2xe/comment/pcldjwr/

**Credit and upfront payment: peer / pro_opinion**
P4-28. "I hate to recommend them, since they're predatorial, but CareCredit might be your only option right now" https://www.reddit.com/r/Pets/comments/1xlef2m/comment/19rzwran8jneo/ ; "Not everyone qualifies for care credit." https://www.reddit.com/r/Pets/comments/1my7v5p/comment/naceeeq/
P4-29. pro_opinion: "It’s a thing because people couldn’t pay after the pet was treated, and reneged on paying payments, so emergency vets started requiring payment before treatment." https://www.reddit.com/r/Pets/comments/1my7v5p/comment/naa4ttf/
P4-30. "One thing my cousin (veterinarian) told me when I rescued my first dog is to have a couple thousand on hand to drop in an emergency." https://www.reddit.com/r/Pets/comments/1vs0u9a/comment/p4hno9s/

### P6: wrong dose in a panic
**Peroxide amounts given at home**
P6-1. "In a panic I gave her ~40 ml peroxide and it worked in maybe 5-10 minutes." (see P2-20 for the two permalinks)
P6-2. "Since we live two hours from the closest emergency vet, I called them, and they advised me to give 2 tbsp of 3% hydrogen peroxide to induce vomiting." https://www.reddit.com/r/AskVet/comments/1s7cy6j/gave_peroxide_to_induce_vomiting_scared_about/
P6-3. "I know it was stupid, but I induced vomiting with peroxide. It was 3% and it was a little under a teaspoon. I gave it to her and it did nothing. It still has done nothing and it’s 9 at night." https://www.reddit.com/r/AskVet/comments/1oz665m/please_help_hydrogen_peroxide/ ; pro_opinion reply: "To induce vomiting, she would have needed almost double what you gave her." https://www.reddit.com/r/AskVet/comments/1oz665m/comment/np9tby6/
P6-4. Peer dosing rules of thumb: "a few capfuls (depending on dog weight) and they will throw it right up." https://www.reddit.com/r/Columbus/comments/xqhh7j/comment/iqbmz3s/ ; "3% hydrogen peroxide look up how much to give based on weight. That will make her throw it up." https://www.reddit.com/r/DogHealth/comments/1xf2953/comment/19rmzf91jzd9c/ ; "you need to follow body weight guidelines for it so you don’t give too much." https://www.reddit.com/r/labrador/comments/1uvdj3n/comment/oxakzsi/
P6-5. "But he was not throwing up, my mom was on the phone with the vet and they said that she shouldn’t give him any more hydrogen peroxide after we had already given him a second dose." / "But then we couldn't get him to drink it. We were trying to pour it down his throat and use a spoon and it just didn't work." / "I somehow had a medicine syringe in my purse because my dog has epilepsy" https://www.reddit.com/r/Yorkies/comments/1tb4ru7/what_to_do_and_how_to_protect_your_dog_from/
P6-6. Paying the hotline to learn the dose: "They changed me $95 before they would tell me how much hydrogen peroxide to give him to make him vomit." https://www.reddit.com/r/DobermanPinscher/comments/1anrg6x/comment/kpuxhv0/

**Label and instruction confusion (medicines, not charcoal)**
P6-7. "The exact wording on the bottle says, "Give 1ml (cc)/ 10lbs of body weight. Repeat in 2 weeks." "Give 4ml by mouth for 3 days. Repeat in 2 weeks."" https://www.reddit.com/r/DogAdvice/comments/1tnmnde/instructions_unclear/
P6-8. customer_report (caretaker): "Whenever there is medication I always ask them to write out instructions for me, I know there is no way I’m remembering what exactly is needed 😅😅" https://www.reddit.com/r/RoverPetSitting/comments/y35g8u/comment/is6uljl/
P6-9. "This is why my dogs medicines are pre-packed ... I don't want our doggo getting the wrong amount." https://www.reddit.com/r/dogs/comments/y3xiql/comment/isb1eyb/

**Wrong-dose and wrong-pill accidents at home (medicines)**
P6-10. "My 57 lb 13 year old pittie got a double dosage (200 mg) of carprofen tonight when my husband fed him accidentally after I already did." / "I’m so anxious but the nurse didn’t really say much on the phone." https://www.reddit.com/r/pitbulls/comments/1t4umzd/accidental_extra_dosage/ ; "Called the vet whose assistant actually howled with laughter and said give him bread!" https://www.reddit.com/r/pitbulls/comments/1t4umzd/comment/ok6mhz0/
P6-11. "I accidentally gave my 90lb lab Pyrenees mix enalpril that was meant for my 35lb border collie blue heeler." https://www.reddit.com/r/AskVet/comments/1hop7g1/i_gave_the_wrong_dog_medicine/
P6-12. "I’m so sorry but I feel stupid right now so please help and don’t fight me or anything." https://www.reddit.com/r/AskVet/comments/1kalnay/accidentally_gave_too_much_dosage/
P6-13. "A couple nights ago, I was doling out medications for my two cocker spaniels and accidentally gave the wrong meds to one of my dogs." https://www.reddit.com/r/dogs/comments/uihbsp/the_other_day_i_did_something_so_stupid_and_found/
P6-14. customer_report (caretaker): "I misread the message) so dog had double their normal dose." https://www.reddit.com/r/RoverPetSitting/comments/14j5oi7/comment/jpk73hq/
P6-15. "She is vision impaired and gave him Aleve instead. He deserved better but he died horribly from internal bleeding and kidney failure." https://www.reddit.com/r/offmychest/comments/1t52gvb/my_mother_accidentally_poisoned_our_dog/
P6-16. Chewy as a resource: "A vet tech on chewy said 'checking my doses, it is still under the high side. She should be ok but you should skip the morning dose'" https://www.reddit.com/r/AskVet/comments/1xjxn0t/accidentally_gave_dog_2_vetoryl_doses_in_1_day/
P6-17. peer: "Bigger dogs handle higher doses of poisons that might kill smaller dogs." https://www.reddit.com/r/Pets/comments/s40foh/comment/hsod7w3/ ; "It is good to know about the lethal doses of common items that your dog might ingest." https://www.reddit.com/r/DobermanPinscher/comments/1anrg6x/comment/kput3oj/
P6-18. Vet-supplied home emergency medicine (an analogy, not charcoal): "When my baby had his first seizure the vet gave us a vial of rectal diazepam only for emergency use if he has another seizure." https://www.reddit.com/r/EpilepsyDogs/comments/1odqzx6/comment/nkwu4ns/

### P2: peroxide
**Vets and hotlines that advised peroxide**
P2-1. "I called the emergency vet for advice since it is a Sunday evening. She suggested inducing vomiting with 3% hydrogen peroxide" / "I can't sleep although she appears to be fine because I'm worried I did the wrong thing." / "I have a habit of googling things and getting super anxious (bad habit, I know)" / "I also read that it can cause some pretty serious GI issues and there was a study where it caused ulcers in all 6 dogs who received it." https://www.reddit.com/r/AskVet/comments/kuwbzx/emergency_vet_recommended_to_induce_vomiting_with/
P2-2. "everything I'm reading about the side effects of peroxide (ulcers, "massive internal bleeding," etc.) has me really scared." https://www.reddit.com/r/AskVet/comments/1s7cy6j/gave_peroxide_to_induce_vomiting_scared_about/ (the 2 tbsp line is P6-2)
P2-3. "The vet told me I could induce vomiting at home with peroxide if I had to but only if I couldn’t make it to the vet since it can cause irritation." https://www.reddit.com/r/puppy101/comments/1uvh106/past_week_with_human_baby_and_8_month_old_lab_has/
P2-4. "Emergency vet told me in a pinch I could use peroxide to induce vomiting but it could cause irritation." / "She threw up the spoon, but now I'm paranoid she's going to get ulcers." / "My husband works 30 mins away and we only have 1 car." / "it feels like she's always finding shit to get into any time she has an ounce of freedom." https://www.reddit.com/r/labrador/comments/1uvdj3n/well_i_had_to_use_peroxide_on_my_rock_fiend/ (a silicone spoon, so a foreign body)
P2-5. "My ACD mix drank some of my coffee once and I called pet poison helpline. They actually advised hydrogen peroxide to induce vomiting." https://www.reddit.com/r/AustralianCattleDog/comments/1syofph/comment/oj0sju6/
P2-6. "My dog ate 5 of those once and the vet told me to give him peroxide to induce vomiting." https://www.reddit.com/r/DobermanPinscher/comments/1anrg6x/comment/kpwn7lg/
P2-7. "I just called poison control when I thought my dog ate slug bait. They just said give her hydrogen peroxide with a turkey baster and wait 30 minutes to see if she barfs." https://www.reddit.com/r/LifeProTips/comments/507912/comment/d71yo1s/ (another answer quotes the same comment as ending "Cost me nothing.")

**It failed, or caused new worry**
P2-8. "I feel so guilty about poisoning my dog, and didn't know there was an injection that is much safer." / "He threw up once (no washers) and felt uncomfortable the rest of the night." https://www.reddit.com/r/DogAdvice/comments/175ezey/comment/kj2xjt3/ (new words from a comment kept on 11-02)
P2-9. "Did this with my pup. Ended up having to go to the vet anyway because she wouldn't stop throwing up." https://www.reddit.com/r/DogAdvice/comments/175ezey/comment/k4fn9mb/
P2-10. "She still hadn't vomited so we became a bit worried." / "After a few hours she vomited again, and then in the middle of the night, again." https://www.reddit.com/r/PetAdvice/comments/1aim1jv/hydrogen_peroxide_and_vomiting/
P2-11. "a teaspoon of hydrogen peroxide and hasn’t thrown up. Will he be ok if he doesn’t throw it up?" https://www.reddit.com/r/AskVet/comments/14qy8fj/my_8_pound_dog_had_a_teaspoon_of_hydrogen/
P2-12. "So far no puking!" https://www.reddit.com/r/AskVet/comments/1fwkg08/please_help_hydrogen_peroxide_not_making_my_dog/
P2-13. "Blood was not present in vomit till 12 hours later" https://www.reddit.com/r/AskVet/comments/1n5cwt8/comment/nbrv2vp/
P2-14. "It’s been almost a week and she’s acting totally normal, however she is sometimes randomly throwing up, mostly mucus." / "Things are financially tight, but I will take her to the vet if that is needed." https://www.reddit.com/r/AskVet/comments/1quy26w/hydrogen_peroxide/
P2-15. (new words) "So more concerned the other dog didn’t throw up and now the peroxide is sitting there." https://www.reddit.com/r/AskVet/comments/1ttxg2h/comment/op5u0xe/
P2-16. "The emergency vet is very expensive and i’ve barely got enough to take her, and I had a friend suggest hydrogen peroxide, but I’ve also read that that should only be administered 1-2 hours after the toxin has been ingested." https://www.reddit.com/r/DogAdvice/comments/1u4ejxz/should_i_go_to_the_emergency_vet/
P2-17. "Peroxide generally is only preferred if you can’t make it to the vet which… I can’t. It can cause ulcers though." / "My 8 month old lab, she eats everything 😭" https://www.reddit.com/r/breakingmom/comments/1uveqgp/comment/oxalqma/ ; "I just feel like I'm failing as a SAHM right now" https://www.reddit.com/r/breakingmom/comments/1uveqgp/comment/oxakolx/
P2-18. "Called the emergency vet frantically after and they basically said to give her a bland diet and monitor her the next few days." https://www.reddit.com/r/AskVet/comments/1uvdcqw/had_to_induce_vomiting_with_peroxide_at_home_what/
P2-19. "How do you make them vomit? Thanks" https://www.reddit.com/r/dogs/comments/vzpb01/comment/igal9v5/
P2-20. "In a panic I gave her ~40 ml peroxide and it worked in maybe 5-10 minutes." Two permalinks in two answers: https://www.reddit.com/r/AskVet/comments/1uvdcqw/had_to_induce_vomiting_with_peroxide_at_home_what/ and https://www.reddit.com/r/DogAdvice/comments/1uvd7ho/had_to_give_dog_peroxide_it_worked_but_now_im/
P2-21. "Looking for any reassurance of people giving their dogs peroxide to throw up and the dog being fine after." (the same two permalinks as P2-20)
P2-22. "My anxiety disorder could’ve never endured this!" https://www.reddit.com/r/puppy101/comments/ly4mls/comment/gpqtwud/

**It worked, and peers say keep peroxide in the house**
P2-23. "A spoon of hydrogen peroxide will work a vet told me this after my dog ate some medication, it worked immediately" https://www.reddit.com/r/WagWalker/comments/1ofbfib/comment/nlct5ck/
P2-24. "A tablespoon of salt to the back of the throat once coughed up an entire raw pork tenderloin. Same dog ate a bucket of chocolate a year later, same trick. He’s fine, just stupid." https://www.reddit.com/r/WagWalker/comments/1ofbfib/comment/nl7vxx3/ ; caretaker counterpoint: "Any method for inducing vomit can pose a health risk to a dog (especially salt)" https://www.reddit.com/r/WagWalker/comments/1ofbfib/comment/nl80egt/
P2-25. "Thank heaven for hydrogen peroxide lol" https://www.reddit.com/r/labrador/comments/11oo0x9/comment/jbu901k/
P2-26. "For future reference hydrogen peroxide will induce vomiting quite quickly if you aren’t near a vet etc. always check with a vet before doing this but I used this several times with my lab over his life." https://www.reddit.com/r/washingtondc/comments/1usph1y/comment/owplz08/
P2-27. "Keep peroxide in your house so they throw up when they eat something." https://www.reddit.com/r/CavaPoo/comments/1teo31s/comment/om59s6v/
P2-28. "Get a vets to walk you through it. I’ve had to do 2x over the years." / "Good knowledge to have, especially if you’re traveling or it’s an odd hour." https://www.reddit.com/r/bernesemountaindogs/comments/1tkinuj/comment/onb0yg2/

**Against home peroxide: pro_opinion (unverified)**
P2-29. "Not really ideal to use peroxide to induce vomiting unless you also want to risk chemical burns/ulceration down the oesophagus and stomach." https://www.reddit.com/r/AskVet/comments/1qismq8/comment/o0treoa/
P2-30. "Peroxide is ulcerative and burns all tissue it touches from mouth to stomach." / "It tastes terrible and causes lots of froth, and both as it goes down and comes up, significantly increases the risk of aspiration(choking)." https://www.reddit.com/r/AskVetAnimals/comments/1wed7l7/comment/p9cr807/
P2-31. "Hydrogen peroxide is no longer recommended for inducing vomiting because it can damage the esophagus. Going to the ER instead where they administer an injectable emetic is much, much safer." https://www.reddit.com/r/DogAdvice/comments/175ezey/comment/k4f730a/
P2-32. "My clinic now only advises giving it in a true life or death situation (owner lives hours from nearest vet clinic, etc.)" https://www.reddit.com/r/AskVet/comments/1n5cwt8/comment/nbrsv2a/ ; "Hydrogen peroxide is irritating to the mucosal lining of the esophagus, which is why we try to limit the use of it." https://www.reddit.com/r/AskVet/comments/1n5cwt8/comment/nbrvhsr/
P2-33. "Medium to high chance of aspiration (choking), especially given how bad it tastes, the salivation that it causes, and then the vomiting itself." / "It's much safer to have us give the injection at the vet. They go from 100% feeling fine to heaving and vomiting usually within 1-3 minutes of administration." https://www.reddit.com/r/Goldendoodles/comments/1f2n4i3/to_the_op_whose_dog_ate_1_grape/
P2-34. Cats: "I’m shocked your vet said to administer hydrogen peroxide, it is strongly NOT recommended for use in cats as they are prone to developing hemorrhagic gastroenteritis from it." https://www.reddit.com/r/AskVet/comments/1u3wsa0/comment/or8jg7s/
P2-35. "Please do NOT recommend owners give their pets hydrogen peroxide without direct supervision of a licensed vet." https://www.reddit.com/r/DogHealth/comments/1xf2953/comment/19rn3jhab1bs0/ ; "It is VERY possible aspirate this way, I advise you take her to the vet if she’s acting lethargic in anyway" https://www.reddit.com/r/DogAdvice/comments/1qsmiow/comment/o2wn5v8/ ; "In the future please never do that without calling the vet first, it can be extremely dangerous." https://www.reddit.com/r/DogAdvice/comments/1uvd7ho/comment/oxa7cpe/
P2-36. Timing: "Don’t feed peroxide or salt, it might make it worse." / "It had been a couple of hours now and vomiting is not going to be as effective anyway." https://www.reddit.com/r/DogAdvice/comments/1wafc6u/comment/p8hr7k0/ ; "the window to vomit up a toxin is limited to 2 hours." https://www.reddit.com/r/DogAdvice/comments/1u4ejxz/comment/orcm5ai/ ; "by the time you see symptoms it's too late to just make them vomit it out." https://www.reddit.com/r/Dogowners/comments/1tuey5y/what_you_should_do_if_your_dog_eats_a_tampon_psa/
P2-37. "(DO NOT INDUCE VOMITING IN PETS) That includes gagging, salt, olive oil, etc. Induced vomiting needs to be done in a medical setting and can make things worse when done at home." https://www.reddit.com/r/Pets/comments/1qmnc2p/comment/o1qwp2t/
P2-38. "the online misinformation makes me insane." https://www.reddit.com/r/veterinaryprofession/comments/1rurzfk/comment/oantkrs/

### P3: vet closed at night / far away
P3-1. "We are driving 2 towns over to seek help from an ER who had agreed to remain open on the evening of 4th of July." https://www.reddit.com/r/AskVet/comments/1unmwq3/emergency_help_puppy_ate_whole_block_of_rat_poison/
P3-2. "I plan to make an appointment at 8am Monday... I don’t know what to do." https://www.reddit.com/r/AskVet/comments/1n4lw7u/help_vet_closed_until_monday/ ; peer: "Does your normal clinic have an on call vet? Many do even when closed if there are no emergency clinics nearby." https://www.reddit.com/r/AskVet/comments/1n4lw7u/comment/nbmaqtd/
P3-3. "I called a 24-hour emergency vet, who advised me to monitor her at home..." https://www.reddit.com/r/AskVet/comments/1x4dasl/possible_chocolate_poisoning_in_my_12_lb_dog/
P3-4. "My vet laughed me off... I stormed out and took my dog to emergency vet" / "They imidiatly did blood work and flushed her stomach out and they are keeping her there until next morning." / "she said no because its not needed." https://www.reddit.com/r/AskVet/comments/1tbxsnc/should_i_find_a_new_vet/ ; "I felt guilty but now I feel angry at her." https://www.reddit.com/r/AskVet/comments/1tbxsnc/comment/olk3360/ ; "she told me she wont do anything between the door." https://www.reddit.com/r/AskVet/comments/1tbxsnc/comment/olks812/
P3-5. "I'm calling the vet when they open but I’m wondering if I should just drive over and be there with her when they open." https://www.reddit.com/r/AskAVeterinarian/comments/1t94f55/my_vet_doesnt_open_for_a_half_hour_does_this_look/
P3-6. "Emergency vet! ... I was on my way. Poor guy I should have left 12 hours ago." https://www.reddit.com/r/CATHELP/comments/140sr99/comment/jmxfvfb/
P3-7. "She suffered for hours longer than she needed to, because I didn’t realize how bad it was when I opted to wait for her own vet to open in the morning..." https://www.reddit.com/r/Petloss/comments/1u2mpcy/she_died_badly_before_the_vet_could_administer/ [context not stated]
P3-8. "It's 3:15 in the fucking morning. My face hurts from crying. My cat also still doesn't seem all there." https://www.reddit.com/r/Vent/comments/1wxcrya/well_i_just_had_a_terrible_night/ [context not stated]
P3-9. "They tried to take him to the vet but was closed around 4-5am." https://www.reddit.com/r/DogAdvice/comments/1w7k10u/need_to_not_feel_guilty/ [context not stated]
P3-10. "It's scary and disheartening to know that there might not be a vet available if anything happens to one of my dogs." https://www.reddit.com/r/dogs/comments/uihbsp/the_other_day_i_did_something_so_stupid_and_found/
P3-11. peer: "Emergency vets are like going to the emergency room, I’ve had to wait hours before just to be seen." https://www.reddit.com/r/AmITheDevil/comments/1skgofu/comment/og7p4ql/
P3-12. customer_report (caretaker): "She remained completely normal for the next 24 hours... Then, approximately 24 hours later, she started urinating blood." / "He believed she would be fine and that we should monitor her closely for the rest of the day." https://www.reddit.com/r/RoverPetSitting/comments/1wyts39/hi_all_i_need_your_advice_my_worst_fear_happened/
P3-13. "I noticed she was lethargic and couldn’t keep her head up when I was holding her." https://www.reddit.com/r/puppy101/comments/wq7e5c/puppy_went_to_emergency_vet_after_ingesting_drugs/
P3-14. Getting ready for nights: "write down where your closest emergency vet locations are that are actually open after hours/weekends" https://www.reddit.com/r/LifeProTips/comments/1wh7x2z/lpt_for_pet_owners_write_down_where_your_closest/ ; "now the emergency number is on a post-it by the door." https://www.reddit.com/r/LifeProTips/comments/1wh7x2z/comment/pa81mfr/ ; "We actually selected our vet based entirely on their after-hours support options." https://www.reddit.com/r/LifeProTips/comments/1wh7x2z/comment/pa07ja4/
(Rural or one-car access also appears in P6-2 and P2-4.)

### P5: poison control fee and hold
**Fees paid, and whether it was worth it**
P5-1. "I called poison controll and asked me for $110.00 for consulting. I cant afford that just for them to tell me to go to the vet." https://www.reddit.com/r/DogHealth/comments/1xf2953/my_lil_dog_is_2_she_weighs_about_89_lbs_she_ate_a/
P5-2. (new words) "I would have paid whatever, but the time they make you wait on hold, then the time to pay is horrible when every second counts." https://www.reddit.com/r/DobermanPinscher/comments/1anrg6x/comment/kpuxhv0/ (the $95 dose line is P6-6)
P5-3. "It cost 95 dollars to call the pet poison control." / "They told me just to monitor her for three days but most likely she would be fine and super dehydrated." https://www.reddit.com/r/goldenretrievers/comments/1fk1awz/in_case_you_are_wondering_it_cost_95_dollars_to/ ; "Cost $25 for a phone consultation. I took it out of Piper’s allowance." https://www.reddit.com/r/goldenretrievers/comments/1fk1awz/comment/lnselg9/
P5-4. "It did cost me $100 to call, but that’s still half the price of the emergency visit." / "I called my normal vet who advised that they would have just called the same poison control number to get more details." https://www.reddit.com/r/AustralianCattleDog/comments/1tixm3c/aspca_poison_control_hotline/
P5-5. "Yes its around $100 us I believe. BUT its invaluable." / "They give you a case number and you can call back with follow up concerns, AND if you need to go into a vet they’ll call ahead and give your vet the treatment plan." https://www.reddit.com/r/toddlers/comments/1xhdog6/comment/19rt92bdo3fur/ (posted in r/toddlers; the pet context is not visible in the excerpt)
P5-6. "They make you pay ~$90 one time fee but it’s 100% worth it." / "This part is super important because literally every minute counts." https://www.reddit.com/r/dogs/comments/17f45nl/what_to_do_if_your_dog_eats_something_poisonous/
P5-7. "Well worth the $70 at the time." https://www.reddit.com/r/YouShouldKnow/comments/1ihevsn/comment/mb237ye/ ; "He ate well above a lethal dose but has no kidney damage due to the immediate expert advice I got from poison control." / "My local Blue Pearl Hospital would not begin stabilizing measures without a case number. They were in touch with poison control throughout treatment." https://www.reddit.com/r/YouShouldKnow/comments/1ihevsn/comment/mawjagt/ (new words; another line was kept on 11-02) ; "The quick timing on all our parts saved my babies." https://www.reddit.com/r/YouShouldKnow/comments/1ihevsn/comment/max4czs/
P5-8. "My dog ate rat poison hidden in my garage twice. We called poison control, they asked questions about the brand, amount, breed, weight of the dog, etc and calculated how much she could have before it was toxic to her." https://www.reddit.com/r/Pets/comments/1is1hx4/comment/mdd2t1e/
P5-9. "They told me she was ok to monitor and gave me stuff to look out for." https://www.reddit.com/r/DogAdvice/comments/158xlnj/dog_ate_two_raisons_animal_poison_control/ ; "It was worth the call to have peace of mind and to not drive her to the ER if she didn’t need it and take up resources/have a very long wait." https://www.reddit.com/r/DogAdvice/comments/158xlnj/comment/jtcq5l7/ ; "ASPCA has a poison control hotline you can use for a donation. They can check dog’s body weight against amount ingested & give you a good action plan." https://www.reddit.com/r/DogAdvice/comments/158xlnj/comment/jtcoor7/
P5-10. "they ended up telling me it was subtoxic for his weight and that he will most likely just have upset stomach." https://www.reddit.com/r/DogAdvice/comments/1t5zvxp/do_you_trust_poison_control/ (title slug "do you trust poison control")
P5-11. "My cat ate the dogs Apoquel a couple months ago and the ER vet told us that we absolutely have to call Poison Control before we come in. Not optional." and "In my case we didn’t need to go, which saved us a ton of money in the end." https://www.reddit.com/r/Pets/comments/1qmnc2p/comment/o1teq0a/ ; "Poison control saved me from going to the ER when my dog ate an entire packet of my daily vitamins." https://www.reddit.com/r/Pets/comments/1qmnc2p/comment/o1x892z/
P5-12. "I'd recommend ASPCA poison control hotline in case of any ingestions. They are super legit and helpful." https://www.reddit.com/r/DogAdvice/comments/175ezey/comment/k4gn955/
P5-13. Cat: "They told me to monitor her and: - Take away access to food and water for an hour - Offer water after an hour" https://www.reddit.com/r/CATHELP/comments/1ovriv0/comment/nolifls/

**Holds, resentment, double charges**
P5-14. customer_report (caretaker): "You can also call the animal poison line but chances are you'll just end up on perma hold and pay $75 to be told to bring your dog to the vet." https://www.reddit.com/r/WagWalker/comments/1ofbfib/comment/nldsw67/
P5-15. "all they did was read the same article i read and told me to go to the hospital" https://www.reddit.com/r/cats/comments/1ttu57o/500_vet_bill_and_she_was_fine/ ; "I was literally comparing pet insurance quotes planning on getting one this week but ill have to wait till next month" (same post)
P5-16. "Just a warning, in my experience they are severely understaffed and hold times are often 2 hours or more." https://www.reddit.com/r/dogs/comments/yp69di/comment/ivhpx74/
P5-17. (new line from the 11-02 Tier A thread, Tier B here) "There has to be a way get a poisoned animal in front of a vet NOW, instead of waiting three times longer to get, and pay for! Poison Control's opinion." https://www.reddit.com/r/AskVet/comments/1t6mhey/pet_poison_control/
P5-18. (new lines) "Had it been a real emergency, we would have been long past the point of being able to help." / "Pet Poison Helpline had a helpful 'estimated wait time' while ASPCA did not." https://www.reddit.com/r/Pets/comments/1o68fek/ysk_that_aspca_poison_control_can_take_up_to_2/
P5-19. (new words) "This is without considering low income individuals who may not be able to afford this price gouging" https://www.reddit.com/r/assholedesign/comments/raeaqq/comment/hnhntoq/
P5-20. (new words) "It’s ridiculous in my opinion. If they have to charge a fee, they should charge a more affordable one." https://www.reddit.com/r/puppy101/comments/kzmwje/why_tf_does_animal_poison_control_charge_5000/ ; "Usually the emergency vet will give you general answers for free if you get a helpful vet tech when you call." https://www.reddit.com/r/puppy101/comments/kzmwje/comment/gjou4bz/
P5-21. (new words) "I'm furious. We just drove 20 mins in the opposite direction of town to be told that they required us to pay $75 to someone over the phone for them to tell us to go to the vet" https://www.reddit.com/r/puppy101/comments/utaup0/refuse_to_help_my_puppy_unless_we_call_a_third/ ; "I'm sure they get a lot of panicked people willing to pay, though." https://www.reddit.com/r/puppy101/comments/utaup0/comment/i98p6ff/
P5-22. "I did pay for poison control and the vet still charged me for additional" https://www.reddit.com/r/AskVet/comments/1i2u1bu/comment/m7tjk50/ ; peer: "Did you give the vet your case number? If a case number wasn't given, they have to call and pay the charge again unfortunately." https://www.reddit.com/r/AskVet/comments/1i2u1bu/comment/m7itxlr/ ; pro_opinion: "If my staff has to call poison control we do charge for it." https://www.reddit.com/r/AskVet/comments/1i2u1bu/comment/m7hgs0w/
P5-23. "Does anybody know a poison control hotline that isn’t free or the cheapest one available???" https://www.reddit.com/r/Pets/comments/1qmnc2p/emergency/ ; peer: "If they have to call poison hotline, they will likely put it on the bill." https://www.reddit.com/r/Pets/comments/1qmnc2p/comment/o1oyke7/ ; "some emergency vets may put the $ you spend at Poison control towards your pet’s treatment" https://www.reddit.com/r/Pets/comments/1qmnc2p/comment/o1wf2xm/ ; "They will make you call regardless to make a case #" https://www.reddit.com/r/Pets/comments/1qmnc2p/comment/o1n4svd/

**Free or cheaper routes (these contradict the fee story)**
P5-24. "if your pet's microchip is registered with Home Again ... you can call the ASPCA Animal Poison Control Hotline for free." https://www.reddit.com/r/LifeProTips/comments/507912/comment/d71teot/ ; "They have never charged for calling and very helpful." https://www.reddit.com/r/LifeProTips/comments/507912/comment/d71ymkc/
P5-25. "You can call regular poison control for free & they will help you with your pet!" https://www.reddit.com/r/YouShouldKnow/comments/1ihevsn/comment/maxgm3i/ ; "If you sign up for AKC reunite, which doesn't cost much, it comes with free lifetime Poison helpline access." https://www.reddit.com/r/YouShouldKnow/comments/1ihevsn/comment/mazt2zc/
P5-26. YSK post: "The cost is $95 and they can help any animals, not just dogs and cats!" / "Some emergency vets will not see your animal without an open case with animal poison control. Save time by opening up a case on the way to the hospital." https://www.reddit.com/r/YouShouldKnow/comments/1ihevsn/ysk_there_is_an_animal_poison_control_hotline_run/

**Why the fee exists: peer / pro_opinion**
P5-27. "Pet Poison Control (a private company entirely separate from poison control for humans) does require payment (via credit card)." https://www.reddit.com/r/legaladvice/comments/1v643ah/comment/ozqsrh5/ ; "The human one’s are state and federally funded, where the pet one isn’t and requires owners to pay in order to keep it operational." https://www.reddit.com/r/legaladvice/comments/1v643ah/comment/ozto9gi/ ; "The cost is because you are consulting with a veterinarian." https://www.reddit.com/r/DobermanPinscher/comments/1anrg6x/comment/kpwi415/
P5-28. pro_opinion: "As vets/techs we can not do anything for a toxicity case without contacting poison control." https://www.reddit.com/r/AskVet/comments/1xgibir/comment/19rppiz2hj4pw/ ; "I work in er and we would have you call poison control regardless." https://www.reddit.com/r/AskVet/comments/1gjr1zp/comment/lvfb90g/ ; "Poison Control is 100% useful. Yes, your pet likely needs in-person care if the ingestion turns out to be serious. But our #1 resource is Poison Control." https://www.reddit.com/r/AskVet/comments/1hrl17d/comment/m4ykpqr/ ; "And they may be able to tell you that the dosage was not problematic saving you the ER exam fee which is typically higher than the poison control fee." https://www.reddit.com/r/AskVet/comments/1hrl17d/comment/m4ylmx1/

### competitor_claim and alternatives named (mentions only)
- Hotlines and services: ASPCA Animal Poison Control, Pet Poison Helpline, human poison control, HomeAgain, AKC Reunite, Chewy vet tech
- Payment and insurance: CareCredit, ScratchPay; Lemonade, Figo, Pets Best (insurers)
- Clinic: Blue Pearl (ER chain)
- Home "kit" items peers mention: hydrogen peroxide (most often), salt, milk, a baby medicine syringe, activated charcoal (generic, no brand)
- **Negative evidence:** none of the 126 answers mentions SavePet, PawMergency, PetVet Medic, Toxiban or VetDTox.
```

**Count of what was pasted:** 53 P1 entries, 30 P4, 18 P6, 38 P2, 14 P3 and 28 P5, so **181 entries**. Several entries hold more than one excerpt from the same thread.

---

## 3. Drop counts by reason

The counts come from coding every excerpt as I read it, about 975 linked excerpts in total. They are tallies made by hand while reading, so treat them as close but not machine-exact.

| Reason | Count | Examples |
|---|---|---|
| **Quote with no link** (possibly invented) | **7** | Five in P3.19, the "metaphors" answer, all with no link: "Felt like I was driving him to the ER blindfolded because nothing was open." / "It felt like playing Russian roulette waiting for the morning vet to open." / "It was like watching a timer count down while I prayed he'd be okay." / "I was gutted and felt completely helpless while waiting for help." / "Rushing to the ER felt like running against a clock." One in P3.20: "My dog licked something off the floor and now he's acting weird, it's 2am and the clinic is closed." One in P2.3: a vet-ER commenter's sentence that sat outside its link. |
| **Quote doesn't support the claim, or permalink inconsistent** | **39** | P6.2 cites 5 r/AdrenalInsufficiency comments about **human** steroid dosing as if they were about "vets" and pets. P6.19 cites 4 r/BenignExistence lines about a **human** taking anxiety meds as "panic dosing" metaphors. P4.9 attaches 2 unrelated r/Pets 1q8k2qg lines to claims about "first aid kits". P1.18 claims "many Redditors keep activated charcoal at home" but backs it with rat-poison quotes (2). "$95 is just crazy" is cited to kpufboy, but report 02 has it as kpunp6j. "saved me an ER Trip." is cited to m4ylmx1, but that comment says something else. "Emergency vet told me in a pinch…" is cited to two different threads. |
| **Answer admits a line is not a direct quote** | **0** | Not found in this batch. |
| **AI claim with no quote at all** | **1** | P1.24: "Brand Information is Limited…" |
| **Off-problem** (not toxic ingestion, or not this buyer) | **202** | Most of P6 drifted to prescription-medicine errors, anxiety meds, vet dispensing mistakes and even human conditions (89 off-problem in P6 alone). Most of P4 drifted to surgeries, illness and economic euthanasia (59). Other examples: foreign bodies such as toys, a penny, a thumbtack and a battery; pet-loss grief; Petfree and scam threads. |
| **Repeat** (of an item kept on 11-02, or already kept in this batch) | **263** | P5 alone had 121 repeats. Its answers re-cite the 11-02 Tier A threads: 1t6mhey, 1o68fek, 1anrg6x, kzmwje, utaup0, 1i2u1bu and raeaqq. |
| **No usable content** | **121** | Hotline phone numbers, "Go to the vet" with nothing else, well-wishes, fragments, condolences. |
| **Jokes / off-topic humour** | **31** | "sin-eater", "Kuzco's poison", "ding a ling", "bunny Brazilians", "Doxycycline". |
| **Suspected spam** | **1** | "playing jackpot city" in r/DogAdvice 1quc75f. The other quote from that post was kept, flagged as P1-14. |
| **Answers with no content** | **5 answers** | 3 empty (P1.12, P2.19, P4.26) and 2 refused (P2.2, P2.23). |
| Passed first read but **merged or trimmed at write-up** | 311 passed → 181 entries | Lines from the same comment were merged into one entry. Weak or generic lines were trimmed. |

---

## 4. Coverage after this read: well covered vs still thin

"Strong" means 3 or more quotes from different people. Counts combine the 11-02 kept items (Tier A and B) with this batch (Tier B).

| Problem | Now well covered | Still thin | Notes |
|---|---|---|---|
| **P1 nothing at home** | **Emotional** (P1-12…P1-17), **beliefs and blame** (P1-18, P1-37, P1-38), **objection "he'll be fine"** (P1-29…P1-32), **trust / vet pushback** (P1-44…P1-51), **catalyst / "keep charcoal at home"**: now 5 people (P1-1, P1-3, P1-4, P1-5, P1-6) plus P1-7 | **Transformation:** still **no story of home charcoal working**; every outcome is vet-given. **Proof** (P1.22) is outcome talk only. P1.12 (self-image) came back empty. | The answers lean heavily on "no home remedy" pro_opinion. |
| **P4 emergency vet bill** | **Prices and emotion** (but mostly not poisoning), **insurance pays after** (P4-20…P4-24, 5 people), **credit / upfront payment** | **Poisoning-specific bills** (only P4-1, P4-2, P4-3, P4-4, P4-5 and P4-6 relate to an ingestion). **Transformation, proof, real vs fake** (P4.23 gave scam stories). P4.26 came back empty. | Reddit Answers mostly pulled general vet-bill threads. |
| **P6 wrong dose in a panic** | **Peroxide amounts and uncertainty** (P6-1…P6-6), **medicine-error fear** (P6-10…P6-15, medicine not charcoal) | **Beliefs, language, metaphors and transformation are essentially empty.** P6.19's quotes were all mismatched; P6.20 was all jokes. Nothing about dosing **charcoal** at all. | The P6 question wording pulls medication threads. A charcoal-specific rewording is needed (§7, C3). |
| **P2 peroxide** | **Emotional**, **failed attempts**, **trust** (heavy pro_opinion), **catalyst** (P6-2, P2-1 Sunday), **who advised it** (vet or hotline: P2-1, P2-3, P2-4, P2-5, P2-6, P2-7) | **Language** (P2.19 empty; P2.20 mostly practical). **Real vs fake** (P2.23 refused). P2.2 refused. | Cats: only pro_opinion (P2-34). |
| **P3 vet closed at night** | **Transformation is no longer thin**: writing down after-hours vets, post-its, picking a vet by its after-hours support (P3-14). **Waiting until morning** (P3-2, P3-5, P3-7). **Distance** (P3-1, P6-2, P2-4). | **Language and metaphors:** the P3.19 metaphors were fabricated and P3.20 was jokes, so still thin. **Beliefs and self-image.** | |
| **P5 poison control fee and hold** | Saturated. New: "worth it" voices (P5-4…P5-12), free routes (P5-24, P5-25), double charges (P5-22) | none | Fees reported now run from $25 to $110 ($25, $70, $75, ~$90, $95, ~$100, $110), plus "never charged" and free routes through microchips or human poison control. |

---

## 5. Updates to the avatar-profile check

Only the 49 visible points can be updated. The last 17 points of report 03 were truncated and remain "status unknown here". All evidence below is Tier B, so per report 03's rule, Tier B **alone never makes a point "supported"**. Where Tier B is the only new support, the verdict says "partly".

| Point | Was | Now | Quote that moves it |
|---|---|---|---|
| **S5** Insurance "is money AFTER" | Not yet tested | **Supported in part (Tier B only, 5 people), with counter-evidence** | P4-20 "still requires you to pay for the procedures then they reimburse you after the fact". P4-21 "Our Figo won’t pay unless we prove we paid the bill in full first". P4-22, P4-23. P4-24 "just like you can’t get home insurance after the earthquake". **Counter:** P4-25 "It saved me over $20,000 in one year". |
| **R1** Partner thinks she's "too dramatic" | Not yet tested | **Partly (one Tier B, not poisoning, and the roles are reversed)** | P4-18 "My wife thinks I overreacted, and wasted $135." (a limp) |
| **F2** "Too late" discovery overnight | Not yet tested (closest only) | **Partly (Tier B; poisoning not confirmed)** | P3-7 "She suffered for hours longer than she needed to, because I … opted to wait for her own vet to open in the morning". P3-6 "Poor guy I should have left 12 hours ago." |
| **F3 / R3** Shame in front of the vet | Self-blame supported; vet judging you for *lacking* charcoal contradicted | **Vet judgment exists, but about causing the poisoning or overreacting, never about lacking a kit.** The "why didn't you have anything at home" form stays contradicted. | P1-53 "They immediately accused me of leaving out Thc". P3-4 "My vet laughed me off". P6-10 "assistant actually howled with laughter and said give him bread!" |
| **H3** ER vet: "if you had given charcoal at home…" | Contradicted | **Contradicted more strongly** (pro_opinion, Tier B) | P1-46 "Be careful with activated charcoal. You can overdose your pet on it. I have seen a dog die from this." P1-47 "…UNLESS advised by a medical professional." P1-44 "There's no home remedy for a poisoned dog." |
| **H5** Stranger: "every responsible owner should have charcoal" | Only affiliate content | **Partly**: peers say it about **peroxide** more than charcoal | P2-27 "Keep peroxide in your house so they throw up when they eat something." P6-4 "Keep hydrogen peroxide on hand… a few capfuls". The charcoal mentions are self-reports (P1-1, P1-3, P1-4), not advice to others. |
| **B8** Reactive preparer (one near-miss leads to buying) | Supported in part | **Stronger.** Near-miss leading to "now I keep charcoal" appears 3 times (Tier B). The proactive buyer also exists. | P1-4 "I would now have charcoal on hand in case he decides to scruff down some pills again." P1-1, P1-3. Proactive: P1-7 "it hit me I’ve got nothing set aside for the dog." |
| **S2** Peroxide is "completely unsafe for cats" | Owner voice not yet tested | **Partly (pro_opinion only), with a contradiction** | P2-34 "strongly NOT recommended for use in cats as they are prone to developing hemorrhagic gastroenteritis". The same comment shows an owner's vet **did** tell them to give it to a cat. |
| **S2 / W1** Peroxide fear vs wanting to induce | Supported in part, with contradiction | **The contradiction grows.** Vets and Pet Poison Helpline tell owners to use peroxide (P2-1, P2-3, P2-4, P2-5, P2-6, P2-7, P6-2), while vet staff call it ulcerative (P2-29…P2-33). | Fear: P2-2 "has me really scared"; P2-4 "paranoid she's going to get ulcers". |
| **P4 / F4** "$2,000 bill"; "$2,500–3,000" | Cost pain supported; $2,000 contradicted as typical (one Tier A at 2 grand) | **$2,000 or more is now reported twice more for ingestions (Tier B).** Typical bills stay lower. Entry fees are a new dimension. | P4-1 "2500 dollars later" (xylitol gum). P4-2 "Over two thousand spent from my bf’s 401k" (cat). Lower bills: P4-4 ($175 + $130), P4-5 ($500), P4-7 ($500). Entry fees: P4-10 "700 just to walk in the door", P4-11 "$500", P4-3 "$900". |
| **S3** ASPCA fee "$95" | Supported, with a fee caveat | **Supported. The range widens, and free routes contradict the fee.** | P5-3 "It cost 95 dollars", P6-6 "$95", P5-26 "$95". P5-1 "$110.00". P5-4 "$100". P5-3 "$25". Free: P5-24 "for free" via HomeAgain; "They have never charged". P5-25 human poison control "for free". This contradicts the kzmwje redirect kept on 11-02. |
| **W2** No measuring or maths in a panic | Supported | **Stronger (Tier B).** Owners pay for, or guess, the amount. | P6-6 "They changed me $95 before they would tell me how much hydrogen peroxide to give him". P6-1 "In a panic I gave her ~40 ml". P6-3 "a little under a teaspoon… it did nothing" vs "would have needed almost double". P6-7 label confusion. |
| **C5** "First 60 critical minutes" | Supported as a belief; not tested clinically | **The belief is supported again. Peer and pro statements give a 2-hour window**, which conflicts with the 1-hour framing and with the page's 1, 4 and 6 hours. | P5-6 "literally every minute counts". P2-36 "the window to vomit up a toxin is limited to 2 hours". |
| **E5** Protective rage | Not yet tested | **Partly.** The anger is aimed at careless other people, not an intruder frame. | P1-38 "be a fucking responsible adult and put them away properly." |
| **B6** Income $120k / spends liberally | Contradicted for the people who have the problem | **Contradicted more strongly** | P1-10 (title) "don't have money to go to the vet". P1-17 "I have no money". P5-1 "I cant afford that". P2-14 "Things are financially tight". |
| Objection #3 "My pet has never gotten into anything" | (profile objection; report 03 status not visible) | **Supported as an objection owners voice** | P1-29 "I swear this dog is indestructible". P1-30 "he was completely fine". P1-33 "I truly thought the inhaler was safe". |
| **F5 / R2** Kids | Not yet tested | **Still not tested.** The only "kid" lines were a bite case and "failing as a SAHM" (P2-17), neither of which is the profile's scene. | n/a |
| **E4** "38%" and **B7** "82%" | Not yet tested | **Still not tested** (no numbers exist in Reddit text) | n/a |

---

## 6. New cited threads worth opening later (not opened; about $0.002 per thread, comments free)

| # | Permalink | Why |
|---|---|---|
| 1 | https://www.reddit.com/r/DogAdvice/comments/1hji198/ | Owner who started keeping charcoal after an ER visit at 5am (P1-1). The only home-charcoal habit story. |
| 2 | https://www.reddit.com/r/DogAdvice/comments/158xlnj/ | Raisins: the poison control experience, "I now keep activated charcoal & hydrogen peroxide", and "for a donation" (P1-3, P5-9). |
| 3 | https://www.reddit.com/r/LifeProTips/comments/507912/ | Home charcoal, a charcoal overdose warning, a free HomeAgain route and "never charged", all in one thread (old). Covers P1 objections and P5. |
| 4 | https://www.reddit.com/r/DogHealth/comments/1xf2953/ | "$110.00… I cant afford that", peer dosing by weight, and a vet-staff "Please do NOT" (P5-1, P6-4, P2-35). |
| 5 | https://www.reddit.com/r/AskVet/comments/1s7cy6j/ | Two hours from the ER; the vet advised 2 tbsp over the phone; ulcer fear. Covers P3, P2 and P6. |
| 6 | https://www.reddit.com/r/AskVet/comments/1oz665m/ | Under a teaspoon did nothing; "almost double" reply (P6-3). |
| 7 | https://www.reddit.com/r/AustralianCattleDog/comments/1tixm3c/ | "$100… half the price of the emergency visit" (P5-4). |
| 8 | https://www.reddit.com/r/Pets/comments/1is1hx4/ | Dog ate poison, no money, gave milk; "no home remedy" replies (P1-10, P1-44). |
| 9 | https://www.reddit.com/r/Pets/comments/1qmnc2p/ | Cat ingestion; poison control "not optional"; "saved us a ton of money"; asks for the cheapest hotline (P5-11, P5-23). |
| 10 | https://www.reddit.com/r/DogAdvice/comments/1t5zvxp/ | Titled "do you trust poison control". Trust family for P5. |
| 11 | https://www.reddit.com/r/Yorkies/comments/1tb4ru7/ | Couldn't get peroxide down; second dose; syringe in purse. P2/P6 administration failure (P6-5). |
| 12 | https://www.reddit.com/r/UKPreppers/comments/1o904o0/ | "nothing set aside for the dog". Proactive buyer, UK (P1-7). |
| 13 | https://www.reddit.com/r/DogAdvice/comments/1rcuag3/ | "such a dumbass… terrible dog mom" (P1-12). |
| 14 | https://www.reddit.com/r/AskVet/comments/kuwbzx/ | ER vet on a Sunday recommended peroxide; owner anxious afterwards (P2-1). |
| 15 | https://www.reddit.com/r/legaladvice/comments/1v643ah/ | "Over two thousand… 401k". Confirms whether this was a poisoning bill (P4-2). |
| 16 | https://www.reddit.com/r/DogAdvice/comments/1tnmnde/ | "instructions unclear": label dose confusion (P6-7). |
| 17 | https://www.reddit.com/r/AskVet/comments/1h4xkvc/ | ER accused the owner of THC exposure. Shame / vet-judgment point (P1-53). |
| 18 | https://www.reddit.com/r/DogAdvice/comments/1quc75f/ | Check for spam before using P1-14. |

**Estimated cost:** 18 posts × ~$0.002 ≈ **$0.036**, comments free.

**$0 option first:** P1-4, P6-6, P5-2, P2-6 and P5-27 (comments in r/DobermanPinscher 1anrg6x) and P4-1 (comment in r/Pets 17xefh8) belong to threads already bought on 11-02, dataset `w0fhweSFZ0i7lN3ew`. Reading that dataset again costs nothing and could move them to Tier A. **Not done this step**, because the brief named only the two answer datasets.

---

## 7. Contradictions, hypotheses and conclusions (kept separate)

**Contradictions and negative evidence** (each is `customer_report` or `pro_opinion` as marked in §2)

1. **Who says to use peroxide.** ER vets, regular vets and Pet Poison Helpline told owners to give peroxide (P2-1, P2-3, P2-4, P2-5, P2-6, P2-7, P6-2). Vet staff elsewhere call it "ulcerative", "no longer recommended", or something to use only in a "true life or death situation" (P2-29…P2-33).
2. **Is the hotline worth the fee?**
   - Worth it: "100% worth it", "invaluable", "Well worth the $70", "saved us a ton of money", "half the price of the emergency visit".
   - Not worth it: "all they did was read the same article i read", "perma hold and pay $75 to be told to bring your dog to the vet".
3. **Is the hotline free?** "They have never charged", free through HomeAgain, and "call regular poison control for free" (P5-24, P5-25) conflict with the human-poison-control redirect kept on 11-02 (kzmwje) and with $70–$110 fees.
4. **Home charcoal.**
   - Owners keep it: P1-1, P1-3, P1-4, P1-5, P1-6.
   - Pro voices warn against it: P1-46 "You can overdose your pet on it"; P1-47 "UNLESS advised by a medical professional".
   - No home-charcoal success story appeared in 126 answers.
5. **The timing window.** Peers and pros say about 2 hours (P2-36). The page says 1, 4 and 6 hours (report 05, competitor_claim). The profile says 60 minutes.
6. **Insurance.** It "saved me over $20,000", but you still pay upfront first (P4-20…P4-25).
7. **"No home remedy for a poisoned dog"** (P1-44) vs owners reporting home peroxide or salt worked (P2-23…P2-26).
8. **Reliability of Reddit Answers itself.**
   - 7 unlinked quotes, 5 of them in a single answer (P3.19) that reads as invented.
   - 39 mismatches, including human medical posts (r/AdrenalInsufficiency, r/BenignExistence) presented as pet-owner voice.
   - 5 permalink inconsistencies.
9. **Brand silence.** SavePet, PawMergency, PetVet Medic, Toxiban and VetDTox appear 0 times in these 126 answers.

**Hypotheses (not proven, for testing)**

- **H4.** Some owners pay the hotline mainly to learn **how much** to give: "They changed me $95 before they would tell me how much hydrogen peroxide to give him" (P6-6). A weight-based dose that is already printed could address that exact moment. Two cautions:
  - SavePet's own page dosing guidance contradicts itself (product_truth.md), so that has to be fixed first.
  - The pro_opinion pushback in H3 still applies.
- **H5.** Owners who keep a kit pair **peroxide + charcoal** and use charcoal "if vomiting is not recommended" (P1-6, P1-3). Positioning charcoal as the step that goes with the poison-control call, not a replacement for the vet, may meet less vet pushback.
- **H6.** On Reddit, **entry and walk-in fees** ($500, $700 "just to walk in the door", $900) and **"pay first, reimbursed later"** may be sharper money hooks than "$2,000". Poisoning-specific bills ranged from about $300 to $2,500.
- **H7.** The rural / one-car / "two hours from the closest emergency vet" owner shows up again (P6-2, P2-4, P2-32, P3-1). This supports H3 from 11-02 that this is a distinct sub-avatar.

**Conclusions (from this read)**

- **C3.** The P6 question family, as worded, does not reach charcoal or emergency-dosing talk. 89 of its excerpts were off-problem medication or human content. A rerun with charcoal- and weight-specific wording would be needed. That would be a paid step and needs the owner's OK.
- **C4.** Reddit Answers adds little that is new for P5 (121 repeats). The best new yield in this batch came from P1 (home-kit habits and objections) and P2 (who advises peroxide, and failures).
- **C5.** The "bought but unread" gap from 11-02 is closed: all 156 answers have now been read. Every new item is Tier B until its thread is opened (§6).

---

## 8. Apify spend for this step

- `list_apify_runs` at the start (2 h window) and at the end (3 h window, limit 200) shows **0 runs tagged `telegram`**. No `call-actor` was made in this step.
- Only `get-dataset-items` reads were used, so **Apify spend for this step: $0.00.**
- The window does show **runs this step did not start**: untagged runs of the Facebook Ad Library actor `XtaWFhbtfxyzqrFmd`.
  - 21 runs between 20:11 and 21:35 UTC, before this step began.
  - **22 more between 22:29 and 22:35 UTC, while this step was running.** I did not start these.
  - In total 43 runs, about $2.03 according to `list_apify_runs`.
  - This is the same unexplained pattern flagged on 11-02. Someone should check which job is launching them.

## Unavailable or failed sources

- **Scaler:** disconnected (OAuth refresh failed). Not needed for this read.
- **Supermemory:** the playbook names no space, so it was not used.
- **ClickUp:** not configured, and not used.
- **Report 01 §5 and report 03 after W5:** truncated in the tool output, and repo search returned no hits.
- **Reddit Answers:** 2 refusals and 3 empty answers (§1).
