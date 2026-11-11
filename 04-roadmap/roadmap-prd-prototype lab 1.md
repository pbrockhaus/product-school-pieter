# Roadmap, PRD & Prototype (Module 4)

## Your strategic anchors
- **Persona (M2), who are you solving for?:** An existing Riverty BNPL user with an activated card who tries to use it for small everyday purchases in store, and wants to pay later wherever they shop (N-01, N-04).
- **Primary success metric (M3), your leading indicator:** In-store decline rate. The baseline is 8.7% in Month 4 (7.9% across the pilot, 48 of 604 attempts), and the target is below 4% (my assumption).
- **Moment of misery (M2), the specific friction blocking the goal:** Declined at the till with no reason shown, so they go back to their debit card. N-06: “The card was declined at a bakery and the app did not say why. I went back to my debit card the same week.” (T-101)
- **Guardrail metric (M3), what must not drop or break:** On-time repayment rate of card holders. Cutting declines must not raise missed payments. The baseline is not in the data pack, so it needs to come from Risk.

## Scan the backlog & set a human baseline
- **My instinctive “quick wins” before touching the AI (2 to 3 feature IDs + why):** B1, decline reason and retry hint in the app. It targets the moment of misery directly (N-06, T-101). If the processor already returns decline codes, this is mostly app messaging, but that’s an assumption I’d check with engineering. One caveat: showing a reason doesn’t stop a decline. It mainly stops people giving up, so it may move retention more than the in-store decline rate itself.

B2, add to phone wallet straight from the approval screen. 143 of 431 activated cards (33.2%) never reached the wallet (T-102), and in-store tapping needs it. It’s one extra step in an existing flow, so effort should be low.

## Audit, override & decide
- **Where did you override the AI? (feature + old vs. new score + why):** B2, add to phone wallet from the approval screen: Value 3 → 4, Effort stays 2. The AI scored it down because it raises in-store attempts rather than lowering the decline rate. My M3 funnel data shows that 143 of 431 activated cards (33.2%) never reached the wallet (T-102). For a persona defined by paying in store, that is the biggest leak in the funnel: a third of card holders never get to the till at all. It also feeds my second metric, new cohorts’ activity one month after activation (target above 69.2%). It can’t be a 5 because it doesn’t directly cut declines, but it is the precondition for every in-store gain. The 4 also makes it a Quick Win whether the builder counts 3 or 4 as “high”, so the call no longer depends on the threshold.

I kept B1 at Value 4, Effort 2. The AI’s reasoning matched mine: it removes the moment of misery (N-06, T-101), but a reason on screen doesn’t stop the decline. B3 (2/4) and B8 (2/5) also stay, since both pains are real (T-103, T-104, N-07) but neither happens at the till.
- **Did the AI over-value a Sales/Eng request your M2 interviews don’t support?:** Not among the features it scored. It was strict with B3 and B8, the two most “platform” features, and put both in Time Sinker. The risk I’m watching for in B4 to B7 is anything that raises limits or targets bigger purchases. That was my original Tech Enthusiast story, and the evidence contradicts it. Interviewees describe everyday purchases (N-01, N-04, the bakery in N-06). Only 0.9% of purchases were over €200, and none of those was declined. A limit change would also need credit policy approval (N-11) and would put the repayment guardrail at risk.
- **Did it underweight something your M3 cohort/funnel data strongly supports?:** Yes, B2 (see above). The AI read the primary metric too narrowly and missed that wallet set-up is where a third of activated users drop out before their first in-store attempt.

## Generate your interactive roadmap
- **My “Now” lane (this sprint), the 2 to 3 quick wins I’ll build first:** only Fix in-store declines at pharmacy, fuel and grocery terminals with the processor
- **What I cut, and the “no” I’m protecting the scope from:** lots of  topics
- **Prototype/roadmap screenshot link (paste into your deliverables):** will go into repo
