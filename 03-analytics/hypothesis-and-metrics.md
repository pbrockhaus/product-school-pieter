# Hypothesis & Success Metrics (Module 3)

## Pre-work · Hypothesis check
- **Role , who you are solving for (from M2):** The Tech Enthusiast: an early adopter and existing Riverty BNPL user who buys high-value electronics, typically €200 to €800 per order.
- **Goal , what this user is ultimately trying to achieve:** To spread the cost of big purchases without being blocked mid-checkout.
- **Friction / moment of misery , the specific pain blocking their goal:** BNPL limit constraints: at checkout the basket exceeds their available Riverty limit, often with little explanation, so the purchase they planned to spread suddenly can’t go through.
- **Current workaround , the external tool or manual process they rely on (M2):** They check their open balance in the Riverty app and work out the gap themselves. Then they either split the basket (what fits on Riverty, the rest on Klarna, PayPal Pay Later or debit), switch the whole basket to a revolving credit card or a competitor’s instalment product, or abandon and wait for repayments to free up the limit. Afterwards they track the split obligations by hand across two or three apps with different due dates.
- **Problem Hook , your one-sentence framing of the business crisis (M1):** Riverty customers who rely on us to spread their payments lose that option the moment they shop outside our merchant network or exceed their limit, so they turn to a competitor’s card, and every purchase made there is lifetime value we hand away.
- **Value Proposition , the outcome your initiative promised to deliver (M1):** Riverty’s payment flexibility anywhere cards are accepted, managed in the app customers already use. It is urgent now because no competitor yet offers a credit card with integrated single-app BNPL built on an existing customer relationship (Klarna, the closest, needs constant app engagement), and the scheme funding window from Visa and Mastercard is open.

## Read the evidence in your case
- **Where does your case say people stall or leave? Does that match the friction you wrote in Module 2?:** The biggest losses come before anyone uses the card. 484 of 1,200 invitees (40.3%) never apply, and 155 of 586 approved people (26.5%) never activate. After activating, people go quiet: the Month 1 cohort falls from 77.6% active to 51.0% by its third month. At the till, 8.7% of in-store attempts are declined with no reason shown (T-101), and N-06 went back to their debit card after one decline. This does not match my Module 2 friction (the BNPL limit blocking a big basket). The pack has no limit data, the average purchase is about €55, and most exits happen before a limit could matter. The friction the pack evidences is an unexplained decline at the point of use, followed by a fallback to debit. Metric needed to test the limit friction: decline reason codes (share caused by insufficient limit).
- **What got better or worse in the case, and does that support the workaround your persona uses?:** Better: card volume grew from €15,206.91 in Month 1 to €61,085.73 in Month 4. Spend per active card rose from €200.09 to €233.15, and instalments from 15.2% to 17.4% of purchases. In-store declines fell from 12.1% to 6.4% by Month 3.

Worse: in Month 4, active cards fell from 278 to 262, the overall decline rate rose from 2.6% to 3.5%, and in-store declines climbed back to 8.7%. Every cohort loses activity: Month 2 drops from 82.0% to 57.1% and Month 3 from 84.5% to 64.0%. In-store share stayed flat at 15.4% to 17.7%.

Mixed signals: the Month 1 cohort ticks back up to 55.1%, and volume kept growing while active cards fell, so spend is concentrating in fewer users.

Support for the workaround: only partly. Falling activity and rising declines fit people paying elsewhere. Rising declines alongside rising spend per card would also fit limits starting to bind. But the pack shows neither where inactive users pay nor why cards are declined, and it has no big baskets. Metrics needed: decline reason codes, and what inactive users pay with instead.
- **Which user in the case is carrying the pain, and is that the person your Module 2 persona describes?:** **3 · Which users feel it**

Light BNPL users carry the most visible pain:
- They are the least likely to activate: 62.0% of approved, against 82.6% for heavy users.
- They buy least: 2.46 purchases and €125.13 a month.
- They make the highest share of purchases in store (24.5%), where declines run at 8.7%.

Heavy users look healthiest:
- 5.82 purchases a month
- €320.88 monthly spend
- 25.4% of purchases on instalments.

No age band or relation group stands out. Activation ranges from 71.4% to 81.2% across ages, and employees and friends or family spend about the same (€222.17 against €215.69).

This is not my Module 2 persona. The Tech Enthusiast maps closest to heavy users, who show the least pain. And no segment has big baskets: the average purchase is about €51 to €55 in every BNPL group.

One mixed signal: heavy users' high spend and instalment share make them the most likely to hit a limit, if limits bind at all. The segments file can't show that.

Metrics needed:
- decline rate by segment
- limit utilisation by segment.

## Step 2 · Craft your hypothesis
- **Qualitative evidence (from M2) , quote the specific friction / moment of misery for your persona:** There is no direct quote for my Module 2 friction. The BNPL limit friction (“the basket exceeds their available limit, so they split the purchase, abandon it, or use a different credit product”) comes from desk research, and its personas are marked as hypotheses. None of the 12 interview notes mentions limits or big baskets.

The closest observed moment of misery is N-06: “The card was declined at a bakery and the app did not say why. I went back to my debit card the same week.”

Before I fill in the rest of the table: are you keeping the Tech Enthusiast as a labelled hypothesis, or switching to the decline-and-fallback friction that N-06 and the data support? That choice changes every row.
- **Quantitative evidence (from M3) , name the metric or data point that confirms the pain; cite the number:** The in-store decline rate confirms the pain.

In card_transactions.csv, 48 of 604 in-store attempts were declined (7.9%), against 1.6% to 1.8% online.
In store is 18% of attempts but half of all declines (48 of 95).
Small everyday purchases are hit hardest: pharmacy and fuel 8.8%, groceries 8.9%.

What follows: cards go dormant. The Month 1 cohort falls from 77.6% active to 51.0% by its third month (cohort_activity.csv).
The data does not confirm the BNPL limit friction. Only 31 of 3,377 purchases (0.9%) are over €200, and none was declined.
- **Persona , role, goal, and the friction you confirmed in the reconciliation steps:** Role: an existing Riverty BNPL user with an activated card who tries it for small everyday purchases in store. Light users are most exposed, with 24.5% of their purchases in store.
Goal: to pay later wherever they shop, including the everyday shop (N-01, N-04).
Friction: declined at the till with no reason shown.
48 of 604 in-store attempts were declined (7.9%), against 1.6% to 1.8% online.
Pharmacy, fuel and groceries are hit hardest, at 8.8% to 8.9%.
After a decline, people go back to their debit card (N-06, T-101).
- **Problem you are solving , one sentence describing the specific friction this initiative removes:** Card holders are declined at the till on small everyday purchases with no explanation, so they go back to their debit card and the card goes dormant.
- **Strategic outcome , what behaviour change do you expect, and how does it map to retention / revenue / churn?:** Behaviour change: card holders keep using the card in store after their first weeks instead of falling back to debit.
Retention: more cards stay active. The baseline is the Month 1 cohort falling from 77.6% to 51.0% by its third month.
Revenue: more in-store purchases per active card. The baseline is an in-store share flat at 15.4% to 17.7%.
Churn: fewer cards abandoned after a first bad experience.
- **Primary success metric (initiative signal) , the leading indicator that tells you the gap is closing:** Metric: in-store decline rate.
Baseline: 8.7% in Month 4 (7.9% across the pilot).
Target: below 4% (assumption: about halfway to the online rate).
Metric to add: the share of card holders who use the card again within 14 days of a decline. This isn’t in the data pack, so it needs tracking from launch.
- **Guardrail metric (product signal) , the metric that must NOT drop; it protects your existing base:** Metric: on-time repayment rate of card holders. Cutting declines by loosening risk rules must not raise missed payments.
Baseline: not in the data pack. Ask Risk for it, and note N-10’s warning that an employee-heavy test group will flatter it.
- **Decision window , how much time or data before you scale, pivot, or kill? minimum threshold to proceed?:** Length: two full months after release.
Data needed: at least about 420 in-store attempts, which is what’s needed to see a drop from 8.7% to 4% reliably (my calculation). At the Month 4 rate of 206 attempts a month, that’s two months.
Scale if:
the in-store decline rate is below 4%,
the activity of new cohorts one month after activation is above the Month 2 cohort’s 69.2%,
and the guardrail holds.
Pivot if declines fall but cohort activity doesn’t improve. That would mean declines aren’t what drives dormancy, so look next at the wallet drop-off (143 of 431 activated cards never reached the wallet, T-102) or the split balance view (T-103).
Kill if the decline rate doesn’t move.
Scope limit: keep the fix to decline reasons, retry hints and technical or merchant-side causes. Any credit policy change goes back through approval and takes months (N-11), which would blow the window.
- **Draft your full hypothesis sentence , one to three sentences; quote the metric, name the persona, name the outcome:** Based on N-06’s unexplained decline at the till and an in-store decline rate of 7.9% (48 of 604 attempts, against 1.6% to 1.8% online), I believe that removing unexplained in-store declines for BNPL card holders who use the card for everyday shopping will keep them paying with the card instead of falling back to their debit card. This will be measured by the in-store decline rate falling from 8.7% to below 4%, with new cohorts’ activity one month after activation rising above 69.2%. I will protect card holders’ on-time repayment rate and will make a go/no-go decision after two full months, or at least 420 in-store attempts.
