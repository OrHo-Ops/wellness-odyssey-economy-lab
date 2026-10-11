# Location-Based Monetization and a Post-Launch Experiment

> **Everything on this page is a proposal.** Wellness Odyssey has no merchants, no sponsorship agreements and no revenue. No experiment has been run. Every commercial number below is a hypothetical placeholder, listed in [`assumptions.csv`](../assumptions.csv) with the status `hypothetical`.

## 1. The concept

Players already walk to earn progress. A location quest gives that walk a destination: start the quest, travel there, and claim a reward on arrival. If a local business sponsors the quest, the same mechanic becomes a way to bring interested people to its door.

| Who | What they get |
|---|---|
| Player | A destination worth walking to, extra Energy, and a collectible that only quests award |
| Business | Visits it can count, from people who chose to come |
| Game | B2B revenue that does not depend on selling currency or showing ads |

**Where this stands.** Location quests with verified arrival and a walking bonus exist in the game today, and they are not sponsored. Sponsorship is a concept, not a built feature. The pricing comparison, unit economics and experiment below are proposals.

## 2. Three commercial models

| | Fixed sponsorship fee | Cost per verified visit | Hybrid |
|---|---|---|---|
| **Revenue mechanism** | Flat monthly fee to feature a quest | Fee for each verified arrival | Smaller monthly fee plus a lower fee per arrival |
| **Business incentive** | Easy to budget, but pays the same whether ten people come or sixty | Pays only for results and carries no volume risk | Shares the risk; the fixed part signals commitment |
| **Measurement challenge** | Billing needs no measurement, but renewal still depends on showing visits | Every bill rests on visit verification, so a disputed or faked visit is a revenue problem | Same as per visit, with less money riding on each arrival |
| **Operational complexity** | Low: one invoice | High: verification, per-visit billing, budget caps, disputes | Highest: both systems |
| **Main risk** | Mispriced by design. Quiet locations overpay and leave; busy ones underpay | Revenue moves with player numbers, and the game carries servicing cost when volume is low | Hardest to explain and sell |

## 3. Illustrative unit economics

A one-month, single-city pilot. All inputs are hypothetical.

| Input | Value |
|---|---|
| Sponsored quests (one merchant each) | 20 |
| Monthly active players in the city | 5,000 |
| Eligible: location permission on and a sponsored quest within reach | 40% |
| Eligible players who start at least one sponsored quest | 25% |
| Sponsored quests started per participating player | 2 |
| Started quests that end in a verified arrival | 50% |
| **Verified visits** | **500 a month, 25 per quest** |
| Prices | Fixed $150 per quest · $2.00 per visit · Hybrid $50 + $1.25 per visit |
| Costs | $40 per quest for servicing · $0.25 per visit for verification and billing |

**Result at 25 visits per quest** (monthly, all 20 quests):

| Model | Revenue | Operating cost | Contribution | Margin | Merchant's cost per visit |
|---|---|---|---|---|---|
| Fixed fee | $3,000 | $925 | $2,075 | 69% | $6.00 |
| Per verified visit | $1,000 | $925 | $75 | 7.5% | $2.00 |
| Hybrid | $1,625 | $925 | $700 | 43% | $3.25 |

**The same pilot at other volumes.** Contribution, with the merchant's cost per visit in brackets:

| Visits per quest per month | Fixed fee | Per verified visit | Hybrid |
|---|---|---|---|
| 10 | $2,150 ($15.00) | −$450 ($2.00) | $400 ($6.25) |
| 25 | $2,075 ($6.00) | $75 ($2.00) | $700 ($3.25) |
| 60 | $1,900 ($2.50) | $1,300 ($2.00) | $1,400 ($2.08) |

What the table says:

- **The models differ in who carries volume risk.** The fixed fee looks best for the game at all three volumes, but only because the merchant absorbs the risk: at 10 visits it pays $15 per visitor and is unlikely to renew.
- **Per-visit pricing has a break-even volume.** Each visit contributes $1.75 ($2.00 − $0.25), so a quest needs about 23 visits a month to cover its $40 servicing cost. Below that the game pays to run it.
- **The hybrid never loses money on a quest** under these inputs and keeps the merchant's cost per visit within a moderate range.

**What a visit costs the game economy.** A quest arrival pays 150 Energy, plus a walking bonus: 26 more if about 1,300 steps, roughly 1 km, are walked on the way. That is about 3.5 spins, or 176 Progress Points under the illustrative reward table the simulation uses. In the simulation, two arrivals a week raise Energy income by 16% for the low-activity profile, 8% for moderate and 7% for high, and bring the median day the seventh region is completed forward by about 6, 2 and 2 days. For the low-activity profile both dates lie past day 28 and are projections. The reward is small enough not to distort pacing, and because it is flat it is worth proportionally more to players who walk less.

## 4. Strategic risks

| Risk | Why it matters | Mitigation |
|---|---|---|
| **GPS spoofing and fraudulent visits** | With per-visit billing, every fake arrival becomes a charge to a merchant | Bill only visits that pass stronger verification than a location check alone; cap billable visits per player and per merchant; audit outliers. The game's own anti-fraud rules are deliberately not described here |
| **Privacy and consent** | Location is sensitive, and merchants will ask for data | Use location only while the player is looking at quests; give merchants counts, never individual trails; make sponsored offers opt-in |
| **Poorly targeted destinations** | An irrelevant quest wastes the slot and teaches players to ignore quests | Limit sponsored quests by distance and category; rank them by observed completion; rotate |
| **Excessive commercial pressure** | Too many sponsored slots turn a walking game into an ad feed | At most one labelled sponsored slot at a time; frequency caps; a hide option; no quest is ever required for progress |
| **Merchant ROI uncertainty** | A verified arrival is not a purchase | Start with pay-per-visit and budget caps; report redemptions where the merchant can record them; keep contracts short |
| **Accessibility and fairness** | Players who cannot travel, live far from sponsors or decline location sharing must not fall behind | Keep quest Energy small next to walking income (7–16% in the scenario above); arrival by any travel mode already counts; no progression gate |
| **Monetization undermining the health value** | If rewards favour driving to shops over walking, this stops being a health product | Keep the walking bonus so that walking there pays more than driving; make daily steps a guardrail in the experiment; refuse sponsors that conflict with the health positioning |

## 5. Recommendation: what to test first

**Test cost per verified visit first, with a monthly budget cap for each merchant. Plan to move to the hybrid once visit volumes are known.**

- The two largest unknowns are how many visits a quest produces and what a visit is worth to a merchant. Per-visit pricing puts a price on exactly that unit, so a merchant accepting the price is direct evidence of value. A fixed fee blends both unknowns into one number.
- A new channel with no track record cannot credibly ask for money up front. "Pay only for verified visits, up to a cap" is an offer a merchant can accept.
- Per-visit billing forces the verification and reporting to be built, and every other model needs them at renewal anyway.
- The cap limits fraud exposure while verification is still unproven.

This holds if visits can be verified well enough to bill on, and if merchants value a visit at or above the price. The unit economics also show why it is a test model and not the end state: below about 23 visits per quest per month it does not cover servicing cost, which is what the fixed part of the hybrid is for.

## 6. Proposed post-launch A/B experiment

**Question.** Does offering optional sponsored destination quests improve meaningful engagement without harming the core health-oriented experience?

| Element | Design |
|---|---|
| **Hypothesis** | Players who are offered sponsored quests have higher week-4 retention than players who see only regular quests, with no decline in daily steps or core-loop play |
| **Eligibility** | Players in the pilot city who have granted location permission, finished onboarding (first step sync and first spin), and have a sponsored location within quest range when they first open the quest screen during the test. The rule is fixed before assignment and applied identically to both groups. Staff and test accounts are excluded |
| **Randomization unit** | Player account, split 50/50 and assigned once at the first eligible quest-screen open. Stratified by prior-week steps and by new versus existing player |
| **Control group** | The current game: regular, non-sponsored quests only |
| **Treatment group** | The same quest screen with the same number of quest slots. At most one slot shows a sponsored quest, labelled as sponsored and dismissible. Its in-game reward equals a regular quest's, so the test measures sponsorship and not a larger reward |
| **Primary success metric** | Week-4 retention: the share of assigned players with at least one credited step sync on days 22–28 after assignment. Analysed by assignment, whether or not the player ever starts a sponsored quest |
| **Secondary metrics** | Quest participation and verified destination visits per player; D7 retention; active days per week; regions completed; walking-bonus Energy earned; a one-question satisfaction survey. Merchant side, described but not compared between groups: verified visits per quest, redemptions, merchant-reported sales and cost per visit |
| **Guardrail metrics** | Daily steps per active player; spins per active day; sponsored-quest hide and opt-out rate; location-permission revocations and uninstalls; fraud flags per 100 claims; complaints about advertising. A pre-agreed drop in any of them stops the test |
| **Data collection** | An assignment log (player, group, time, stratum); an exposure event when a sponsored quest is actually shown; the quest funnel by quest type (shown, started, verified arrival, claimed); daily step syncs and spins; hide, opt-out and permission changes; survey answers; merchant-side redemption records |
| **Main confounding factors** | Novelty in the first week; weather, season and holidays, since walking is seasonal; uneven quest density across neighbourhoods; the particular merchants in the pilot; unequal notification volume between groups; spillover between players who walk together; players with more than one account |

**Sample size and duration.** These cannot be computed yet, because no baseline exists. Four things have to be measured first: baseline week-4 retention in the pilot city, the weekly inflow of eligible players, the share of treatment players who are actually shown a sponsored quest, and the smallest retention change that would alter the decision. With those, the usual approximation for comparing two proportions (about 16·p(1−p)/δ² players per group for 80% power at the 5% level) gives the required duration. No effect size is assumed here.

**Decision rule, agreed before the test starts.**

- **Expand** if no guardrail is breached, week-4 retention in the treatment group is higher than or statistically indistinguishable from control within a pre-set margin, and verified visits per sponsored quest reach the break-even volume of the pricing model in use.
- **Iterate** on targeting, labelling and frequency if retention holds but hide and opt-out rates are high, or if visits fall short of break-even.
- **Stop** if retention or daily steps fall.
