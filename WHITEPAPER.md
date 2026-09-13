# un_named_project — White Paper

**A Kenya-first trust protocol for the people who feed, build and move this country.**

Version 1.0 · September 2026

---

## The main goal, in one paragraph

Kenya does not have a food problem. It has a **coordination and trust problem** that looks like a food problem. We import maize while land in Nyanza and Western lies dormant. A farmer in Kisumu gets a fraction of what a Nairobi household pays. A chama's money is one treasurer's honesty away from disappearing. A mama mboga with fifteen years of honest trade cannot borrow against a single day of it, because none of it is written down anywhere that anyone can check. Young people who want to work have energy, phones and time, and no credible way to turn those into income. This project builds the missing layer: an open protocol where trades are protected, group money obeys its own rules, reputation is earned from real events and cannot be bought, and a person's money answers to their own key — plus one app, built on top of it, that a Kenyan can live their day in. The goal is not a marketplace. The goal is that **coordination becomes cheap and trust becomes provable**, so that the land gets farmed, the harvest reaches the city at a fair price, the group's money stays the group's, and the youth doing the work get paid and get a record of it.

---

## 1. The problems we are solving

### 1.1 We import what we could grow

In 2025 Kenya imported **468,109 tonnes of maize**, up 51% on the year, while domestic production grew only 2.2% to 45.8 million bags; nearly all of it came from Tanzania, Uganda and Zambia. [^1] The national food import bill reached **KES 288 billion** in 2025, and the first quarter of 2026 was the highest ever recorded at KES 81.6 billion. [^2] By February 2026, **3.5 million Kenyans** needed humanitarian food assistance, up from 2.2 million a year earlier. [^3]

Now the other half of the picture. Kenya has an estimated **27.4 million hectares of cultivable land, of which only 6.1 million are cultivated** — about 21 million hectares uncultivated. More than 70% of the land in Western, Nyanza and Central is arable, and in the high-potential areas of Nyanza roughly **36% of land is idle or underutilised**. [^4]

Put those two facts side by side and the problem is obvious: the country that is short of maize is sitting on the land to grow it. The land is not missing. What is missing is the *reason* and the *means* to farm it: someone who owns two acres in Siaya does not know what to plant, when, for whom, at what price, with whose money, and with whom to share the tractor. That is not an agronomy problem. It is a coordination problem, and coordination is what software is for.

### 1.2 Middlemen capture the value

A farmer in Kisumu growing mangoes or maize has no direct line to a Nairobi buyer. They sell at the farm gate to whoever comes, at whatever price is offered, because they cannot verify the buyer and the buyer cannot verify them. The margin between the two ends is routinely **40–60%**, and it is invisible — nobody prints it. The farmer earns too little to keep farming; the household in Nairobi pays too much; the information about what is actually in demand never reaches the person who could grow it.

### 1.3 Group money runs on one person's honesty

Kenya has roughly **300,000 chamas managing around KES 300 billion**; one in three working adults belongs to one. [^5] Almost all of that money is governed by an exercise book and a treasurer. When it works, it is the most effective financial institution in the country. When it fails, there is no recourse, no record, and no way for the next group to know.

### 1.4 Reputation does not travel

A trader with years of honest deliveries starts from zero on every new platform and in every new town. A young person who has done a hundred verified deliveries has nothing to show a lender. The most valuable thing a Kenyan small business owns — its track record — exists nowhere it can be proven.

### 1.5 Young people have energy and no ladder

Youth aged 15–34 are **35% of the population**; about **17% of them are in neither education, employment nor training**, and more than a million enter the labour market every year. [^6] They are the delivery riders, the quality checkers, the people who would drive a shared tractor, run a node, verify a stall, organise a neighbourhood's farming — if there were a credible, paid way to do it and a record of having done it.

### 1.6 Daily life is fragmented and every app hoards trust

Paying, ordering food, finding transport, booking a room, finding work, borrowing: each lives in a different app, each with its own idea of who you are, none of which talks to the others, and each of which holds your money and your history hostage to its own survival. And every one of them rebuilds the same trust machinery, closed, badly, and incompatible with the next.

---

## 2. Who this is for, and what each of them gets

| Who | What they get |
|---|---|
| **Farmers** | Direct buyers, a protected payment that cannot be reversed by the buyer once delivery is proven, a live market price for what they grow, and a public track record that becomes credit |
| **Traders and aggregators** | The same protection buying as selling; the ability to buy from many small farms as one lot; reputation that follows them between towns |
| **Buyers** (households, hotels, restaurants, schools, exporters) | Verified supply, money that only leaves escrow on delivery, prices that reflect the real market, and a dispute path that does not depend on shouting |
| **Mama mboga and SMEs** | A storefront, hash-committed payment details nobody can silently swap, automatic books from settled sales, and the ability to raise capital against those books |
| **Chamas and welfare groups** | Rules written once and enforced by code: quorum before any shilling leaves, dissolution that pays everyone by the agreed formula, meetings and attendance recorded |
| **Families with dormant land** | A way to pool adjacent parcels, farm them as one operation, split the harvest by an agreed formula, and sell as a large farm |
| **Young Kenyans** | Paid, recorded work: field verification, delivery, aggregation, running nodes and indexers, organising neighbourhood projects — each job an on-chain fact they own |
| **People running the network** | Node and indexer operators, dispute arbiters, bonded verifiers and approved app builders each earn from the protocol's fee and verification streams, in the open |
| **Every Kenyan** | One app for the day — buy, sell, pay, eat, move, sleep, work — whose trust layer is public, whose money layer is theirs, and whose privacy is structural |

---

## 3. Dormant land: farming together as one large farm

Here is the scenario the protocol is built for. Five families in a location in Siaya each own between one and three acres. Individually none of them can afford a tractor, bulk inputs, a lorry to Kisumu, or the time to find a buyer. Individually each is too small for any serious buyer to bother with. So the land sits, and Kenya imports maize.

On the protocol those five families are a **community group** with a farming schema:

1. They write the rules once — who contributes what land, labour and money; how the harvest is shared (by acreage, by labour, by capital, or a mix); what quorum decides spending; how the group dissolves. Those rules are hashed and committed on-chain, and **every member joins by presenting the same hash** — you signed what you read.
2. The group has a **treasury** that only quorum can move. Inputs are bought from it; a tractor day is paid from it; nobody's brother-in-law can "borrow" from it.
3. The group's produce is listed **as one farm** — twenty acres of maize, not five scraps — which is the size a Nairobi miller, a school or an exporter actually buys.
4. Every sale settles through escrow into the group's treasury; the **share formula pays each family automatically** from the split. The exercise book is replaced by an event log anyone in the group can audit.
5. The group's record of settled sales becomes its **collateral**: next season it can open a funding pool for seed and fertiliser, and investors are repaid from the harvest sales by the same skim that repays everyone else.

Nothing in the protocol knows this is a farm. It is a group, a schema, a treasury, some listings and some attestations. The same machinery runs a boda co-operative, a women's welfare group or a youth construction crew. That is the point.

Add the ward-level intelligence the app carries — thirty-year rainfall and temperature normals, soil, and which crops fit which ward, drawn from the country's own data — and "what should we plant, and when?" stops being a guess for the families in Siaya.

---

## 4. Farm produce as a living market

Prices on the protocol are not set by us. **Sellers price; the platform informs.** What the platform does is make the real market visible for the first time:

- Every settled trade emits its price, quantity and coarse location. From those events the indexer computes **live medians per territory** — "maize, Kisumu, this week, from N settled sales" — the way a stock ticker is built from real fills, not from anyone's opinion.
- Prices move with demand. When a school term starts and Nairobi's demand for maize rises, the median in Nairobi rises and every farmer in Nyanza sees it, in KES per kilo, on their phone. When Kisumu is flush after harvest and Nairobi is short, the spread between the two towns is *visible*, and a trader with a lorry can act on it — which is exactly the arbitrage that closes the gap and moves food to where it is needed.
- The Ministry's own market data already shows spreads of 10–25% between the same bag of maize in different towns in the same week, and farm-gate prices moving over 40% in seven months. [^7] Today only the middleman sees that. Tomorrow the farmer does.
- Buyers can make **offers** below list; sellers accept with a signature; the trade commits at the negotiated price with both signatures verified on-chain. Bids, asks, fills — a market, not a noticeboard.

To be concrete with an illustrative example: if maize sells at KES 200 per kilo in Kisumu and KES 500 in Nairobi because of demand, transport and trend, the protocol does not "fix" that — it publishes it, lets a Kisumu farmer list against the Nairobi price, and lets a young trader in between earn the honest margin for moving it. Prices that reflect reality, seen by everyone, is how a market stops being a trap.

Below a small threshold (a few hundred shillings) trades settle off-chain and are batched, so a bunch of sukuma is free to sell and still counts toward the seller's history.

---

## 5. How money is kept safe during a trade

Three rules, all enforced by code, none by us:

1. **A person's money sits in their own vault** under their own phone key. The backend can relay a payment the person signed; it can initiate none. There is no company key that can move user money.
2. **Money in flight sits in escrow** under a state machine: *Committed → Fulfilled → Settled*, or *Disputed → Resolved*, or *Refunded* on timeout. The buyer's money leaves their vault only on their signature; it reaches the seller only after the seller proves fulfilment and the buyer confirms (or a window passes); it goes back to the buyer if nothing was delivered by the deadline.
3. **The split is printed.** At settlement the contract emits exactly three numbers — protocol fee, funding-pool repayment, seller net — and the app must show them. The fee is **capped at 2% in the contract itself**; no vote, no update and no company can raise it above that. The buyer sees the total; the seller sees the split; nobody sees a hidden spread.

For the farmer: you cannot be paid in a cheque that bounces. For the buyer: you cannot pay for a lorry that never arrives. For the trader in between: both of your legs are protected the same way. If something goes wrong, a dispute locks the money and a quorum of arbiters — governance-appointed, with the chat transcript hash as evidence — splits it. Every one of these steps is a public event.

---

## 6. A mama mboga raising capital the way the stock market does

Today a stall owner who wants a second fridge borrows from a shylock or does without. On the protocol:

1. Her settled sales are already her **books** — automatic, derived from events, impossible to inflate.
2. She opens a **funding pool**: "KES 5,000 for a fridge, units of KES 500, repay 1.25×, from 10% of each sale, over 180 days." The terms are hashed and committed. To open one she must carry a verification attestation — a bonded field verifier (a young person from her own area, paid to do it) has confirmed the stall exists.
3. Her **raise cap** is set by her history: a first raise is small; each pool repaid in full unlocks a larger one. Progressive trust, like a credit line, from data no one can fake.
4. Neighbours, customers, a chama, or an investor across the country **buy units**. When the target is met the money disburses to her vault. If the target is missed by the deadline, everyone is refunded automatically.
5. From then on **every sale she settles routes a capped skim into the pool** until investors have their 1.25×, then it stops. They claim pro-rata. If she defaults past the term, that is recorded — visible to the next lender, as it should be.

This is chama capital with the exercise book replaced by code and the borrower's reputation made portable. Investors are not promised a return; they are promised **the rule** — and every shilling in and out is an event they can audit. For projects, disbursement can be released in tranches against milestones a verifier attests ("fridge installed"), so the money follows the work.

---

## 7. Youth: jobs, and empowerment projects in the hoods

We are targeting young Kenyans first — the energetic, phone-first generation in the estates and the informal settlements, who are either unemployed or under-employed and who already do most of the physical work of the informal economy without any record of it. The protocol creates paid roles that only exist because trust is being made provable:

- **Field verifiers.** Bonded through the attestation registry, paid per verification (they keep the majority of the fee), slashable for lies. Verifying a stall, a farm, a delivery, a milestone. This is the first job the network creates, and it is a job for someone who knows the area.
- **Delivery and logistics.** Orders on the marketplace need moving; boda riders and small lorries join as actors with a delivery schema, and every completed delivery is a settled agreement on their record.
- **Aggregators and organisers.** The person who gets the five families in Siaya to form the group, who organises the harvest, who lists it as one lot — that coordination is paid work, and the group can pay it from its treasury by quorum.
- **Node and indexer operators.** The protocol runs on a public chain; the read models that turn events into books are open-source and anyone can run one. As the network grows, running infrastructure for a county — and being paid for it from the protocol fee — is a technical job that a young Kenyan with a laptop can hold.
- **Builders.** The engine is open. A team in Eldoret can build a livestock app on the same primitives and register it as a namespace.

**Empowerment projects in hoods and slums** — a youth group in Kiambiu that wants to run a car wash, a kitchen, a recycling point, a community farm on a vacant plot — use the same machinery as the families in Siaya: a group with committed rules, a treasury behind quorum, a funding pool for capital, milestone tranches released against verified progress, and settled sales that build the group's record. **Credibility is the product.** Nobody has to take the group's word for anything: the rules are hashed, the money is on-chain, attendance at meetings is recorded, the verifier who signed off is bonded, and the audit page is public. A donor, a county government or an investor can see exactly what happened to every shilling — which is what has been missing every time a youth project asked for money.

The reference app already carries the full administrative map — every county, constituency, ward and sublocation, and more than ten thousand named settlements including informal ones like Kiambiu, with their leaders, schools, clinics, roads and climate. A project in a slum is a project *somewhere real*, at an address the protocol knows, which is the precondition for it being credible.

---

## 8. One app for the day

Kenyans should not need nine apps to live a Tuesday. The reference app is built the way WeChat is built in China — one place to do the things a day requires — but with the trust layer public and the money layer the user's own:

| Need | On the protocol it is… |
|---|---|
| Buy food, sell produce | listings + escrow (the marketplace) |
| Order a meal from a local kitchen | a listing with a food schema + delivery agreement |
| Get across town, get a lorry for a harvest | a gig listing + a delivery schema + escrow |
| Find a room for the night in another town | a rental/hospitality schema + escrow with a check-in fulfilment |
| Pay anyone, get paid | the vault + signed intents, KES-denominated on stable rails |
| Save with your group | a community group with a treasury |
| Borrow, invest | funding pools |
| Work | verification, delivery and organiser jobs, each an on-chain record |
| Know your place | the map: your ward, your leaders and their records, what grows here |

Every row is the same handful of primitives with a different schema. Adding "hotel bookings" is a transaction, not a deployment.

---

## 9. Privacy and safety: what goes where

The chain is public and permanent, so it holds only what must be public and permanent. Everything personal stays off it.

| Lives on-chain (public, forever) | Lives with the app (private, deletable, under the Data Protection Act) | Shown to other users |
|---|---|---|
| actor ids (random 32-byte ids), signing keys | names, phone numbers, national ID, KYC documents | a handle you chose; "@wanjiku" not your ID |
| listing hashes, price, quantity, a ~5 km cell | photos, descriptions, your exact location | the listing, the photo, "near Kiambiu, Nairobi" — never a street |
| escrow states and the money split | chat, support tickets, notes | your trades count and dispute rate — as numbers, never as names |
| attestation claim hashes + who attested | the evidence itself | "verified by a bonded verifier under schema X" |
| group rules hash, treasury, votes | the rules text, meeting minutes | to members: everything; to the public: totals and rules, never the ledger |
| proposals, votes, rationale hashes | full rationale documents | the outcome and the reason |

**What nobody can do**, including us: move your money without your key; edit your reputation; sell your data (the chain does not hold it and the private store is one leak from ending the company); see your exact location; raise the fee above 2%; change a group's rules after you joined; take a group's money without its quorum.

**What happens when you lose your phone**: you request a key rotation from the new phone with evidence; a window runs; if the old phone is still in your hands you can veto from it (so a thief who files first still loses); when the window passes the new key takes over and your vault — money, history, reputation — answers to it. Recoverable, never seizable. Companies' keys work the same way with an extra root approval.

**Who you trade with** is a handle and a record, never an identity. Money contexts always show the person's main handle so a temporary alias cannot be used to trade under a borrowed reputation.

---

## 10. Security for people who are not "crypto people"

Most Kenyans — most humans — will never understand, and should never need to understand, private keys, seed phrases, gas or nonces. Every person who has been told to "write down these twelve words and never lose them" has been handed a liability, not a product. So the rule for the app is simple: **the phone does the cryptography; the person does what they already know how to do.**

### 10.1 What logging in looks like

- You install the app and confirm your **phone number** with the code you receive by SMS, exactly like M-Pesa or WhatsApp. You choose a **PIN**, and if your phone has a fingerprint or face sensor you turn that on.
- That is the whole of it. There is no wallet to create, no words to write down, no "connect wallet" button, and you will never see a token symbol — every amount in the app is in **shillings**.
- Underneath, at that moment, the phone quietly creates a signing key inside its **hardware security chip** (the same place Android and iPhone keep your fingerprint data). The key never leaves the chip; it cannot be copied out, not even by the app. When you tap "Pay KES 300 into escrow", the app shows you a plain-language sentence, you confirm with your PIN or fingerprint, and the chip signs. That signature is what the protocol trusts. You never touch it, name it, or back it up.
- The network's transaction fees ("gas") are paid by the app operator, not by you. You are never asked to hold anything but shillings.

This is the Binance idea — the company handles the hard parts so the user never sees them — with one deliberate difference, covered below.

### 10.2 What we handle for you

| You do | The app and the protocol do |
|---|---|
| confirm your number, choose a PIN | create a hardware-backed key on the phone; register you as an actor on the protocol |
| tap Buy and confirm with fingerprint | build the intent, sign it in the chip, relay it, pay the network fee, wait for the chain, show you the result |
| load your account from M-Pesa | convert at a displayed rate, deposit into *your* vault under *your* key |
| forget the details | keep the receipts: every trade, every group payment, every vote is an event you can always re-read, and the audit page proves the totals |

### 10.3 What happens when you lose your phone

Losing the phone does not lose the money, the history or the reputation — it loses one key, and the protocol was built to replace a key without anyone being able to steal an account.

1. On a new phone, install the app and confirm the **same phone number**. The app files a **recovery request** for you (it is a protocol transaction, but you just see "Recovering your account…").
2. A **waiting window** starts (a few days in the first version). During the window the request is visible on-chain and to you.
3. If the old phone is actually still in your hands — you found it, or it was never lost — you can **cancel the request from it** with one tap. This is the protection: a thief who grabs your number and files first *still loses*, because the real owner's phone can veto.
4. When the window passes with no veto, the new phone's key takes over. Your vault, your trades, your groups, your record — all of it now answers to the new phone. Nothing moved; only the key changed.
5. Forgot your PIN but still have the phone? PIN reset is an app-level flow (number confirmation plus a cooling-off period) that never exposes the key, because the key was never the PIN.

For companies and app operators the same recovery exists with one extra step: a root-level approval, because a company key can act for many people.

### 10.4 Where this is deliberately not like Binance

Binance is *custodial*: your balance is a row in their database, they hold the keys, and they can freeze, delay or — if they fail — lose your money. Here the simplicity is the same but the custody is not: **your money sits in your own vault under your own phone's key.** The company operates the app, pays the network fees, runs the recovery flow and answers the phone — but it holds no key that can move your money, and the audit page proves in public that the vault holds every shilling it says it does. If the company disappeared tomorrow, your vault, your history and the recovery path would still exist on the chain, and any other approved app could pick them up.

### 10.5 Safety limits that work without you understanding them

- **Daily limits** on your vault, set by you, so a stolen unlocked phone cannot drain an account in one go.
- **A pending window** on large outside payments — you can cancel a payment for a short time after sending it.
- **Every money moment shows you a sentence, not a hash**: "Pay KES 300 into escrow for 10 kg of maize from @otieno. It is released when you confirm delivery."
- **Handles, not identities**: the people you trade with see a handle you chose and a record of trades; never your name, number or exact location.
- **No support agent can move your money.** Support can help you recover a key, never spend one. That is not policy; it is the absence of a key that could.

### 10.6 Planned in this area

Biometric gating on every money action (fingerprint required, not just PIN); **trusted contacts** who can shorten the recovery window by vouching for you (a chama member, a family member — a social recovery layer on top of the time-locked one); and a simple "security check-up" screen that says, in Kiswahili and English, what is protected and how.

## 11. Decentralised: who runs it, and why it stays open

- **The chain.** The contracts run on a public Celo-family chain (testnet now, mainnet after audit). The validators are not us. Every state change is a public event.
- **The protocol.** Fifteen contracts, Apache-2.0 when published, governed by a stage ladder that only moves one way: company multisig → council → community. Parameters change by proposal, vote and timelock. Emergency pause exists and always carries a reason on record.
- **The engine.** The open Rust crate any approved app uses. It bootstraps from one address and resolves everything else on-chain, so no app depends on us for anything but the protocol itself.
- **The indexers.** Books, reputation and prices are derived from events by open code. Anyone can run one; if ours lies, yours will disagree, in public. The reference app publishes a live audit page that recomputes the money invariants against the chain on demand — vault, escrow and group balances must equal what the events say, or the app is wrong.
- **The apps.** Ours are closed and compete on their merits. A third party's app is a namespace: staked, scoped, approved by governance, paying dues into the community treasury, slashable.
- **The nodes.** Node, indexer and verification roles are paid from the protocol's fee and verification streams — small, capped, and visible. The plan is county-level operators, and the plan is that many of them are young Kenyans.

---

## 12. How the founding group earns, in the open

Total platform take on any escrowed trade is **capped at 2% in the contract**. The protocol fee (1–1.5%) goes to a treasury behind a governor with a 72-hour spending velocity limit; our own apps charge a visible app margin on top like anyone else's would. Later: a success fee on completed raises only, a displayed sliver on M-Pesa on/off-ramps, tiered namespace fees for other companies, a coordination cut on verification fees (verifiers keep the majority), SME tools subscriptions, and anonymised market-data products. **Never**: personal data, ranking, or interest on user money.

---

## 13. Where we are, and what comes next

**Built and verified today** (local chain): fifteen contracts with 146 tests; per-person vaults; escrow with the 2% ceiling and the funding-pool repayment slot; funding pools with progressive caps; community groups with committed terms, quorum treasuries, dissolution payout, investor tranches, and recorded meetings; key recovery; disputes; governance with stages and timelock; two governed treasuries; an open engine with an event indexer; a reference backend with the public audit page; a reference app with the marketplace, offers, vault wallet, chamas, QR onboarding, and the full national map with leaders, amenities, roads, and ward-level climate and crop intelligence.

**Next**: testnet broadcast and audit; a first-party marketplace pilot in one county with a verification crew of local youth; the M-Pesa ramp; then concurrent project pools and milestone tranches, juror incentives for disputes, county-level node operators, and the food, transport and hospitality schemas that make the one-app promise true.

---

## Sources

[^1]: Business Daily / USDA FAS GAIN, Kenya Grain and Feed Annual 2025 — maize imports 468,109 t (+51.4%), production 45.8 M bags (+2.2%); Tanzania, Uganda and Zambia ≈99% of import shipments; 50% duty outside the EAC. https://apps.fas.usda.gov/newgainapi/api/Report/DownloadReportByFileName?fileName=Grain+and+Feed+Annual_Nairobi_Kenya_KE2025-0006 · https://millingmea.com/kenya-explores-maize-imports-from-zambia-tanzania-to-stabilize-supply-to-millers/
[^2]: Daily Nation, "Kenya's food import bill rebounds to Sh288 billion"; Business Daily, "Kenya's food imports bill hits record Sh82bn in first quarter". https://nation.africa/kenya/business/kenya-s-food-import-bill-rebounds-to-sh288-billion-on-cost-pressure-5357776 · https://www.businessdailyafrica.com/bd/economy/kenya-s-food-imports-bill-hits-record-sh82bn-in-first-quarter-5483572
[^3]: Kenya Food Security Steering Group, February 2026 assessment (3.5 M in need, up from 2.2 M). https://tech-ish.com/2026/06/15/kenya-record-food-imports-shilling/
[^4]: IGAD Land Governance, "Land Ownership and Use in Kenya" — 27.4 M ha cultivable, 6.1 M cultivated; >70% arable in Western, Nyanza, Central; 36.3% idle/underutilised in high-potential Nyanza. https://land.igad.int/index.php/documents-1/countries/kenya/rural-development-3/801-land-ownership-and-use-in-kenya-policy-prescriptions-froman-inequality-perspective/file
[^5]: Capital Business, "How Kenya's Chamas Could Transform Healthcare Access" (≈300,000 groups, ≈KES 300 bn); Huduma Global on chama membership. https://www.capitalfm.co.ke/business/2025/09/how-kenyas-chamas-could-transform-healthcare-access/ · https://hudumaglobal.com/blog/understanding-chamas-kenya-investment-groups-merry-go-rounds-collective-saving
[^6]: NCPD Policy Brief No 2 of 2025 (youth NEET); Federation of Kenya Employers (youth 15–34 = 35% of population); KNBS Quarterly Labour Force Survey. https://ncpd.go.ke/wp-content/uploads/2026/02/Final-Policy-brief-on-Youth-NEET-Final.pdf · https://www.fke-kenya.org/policy-issues/youth-employment
[^7]: Ministry of Agriculture KAMIS wholesale prices (KES 2,200–4,500 per 90 kg bag by region; Kisumu vs Nairobi spreads); Agrisoko market intelligence (farm-gate KES 3,200 → 4,500 in seven months). https://kamis.kilimo.go.ke/ · https://www.agrisoko254.com/market-intelligence/maize · https://sokodirectory.com/2026/07/maize-prices-surge-as-90kg-bag-hits-6500-in-kisumu-and-other-towns/

*The maize prices in §4 (KES 200 vs 500 per kilo) are an illustrative example of a spread, not a quotation; real spreads in the sources are smaller and change direction with the season. The protocol's job is to make whichever spread exists visible.*
