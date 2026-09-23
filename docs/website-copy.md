# Segmenta AI — Website Content Proposal
### Draft v1 for segmenta-ai.com

---

## 0. Positioning foundation

**Category:** Bid floor optimisation for mobile apps and games.

**The wedge:** Everyone else needs to live inside your game. We don't.

**One-line positioning:**
> Segmenta optimises your bid floors from your mediation data — not from inside your game.

**The three-sentence version (use in decks, PR, LinkedIn bio):**
> Segmenta AI turns your mediation platform's user-level ad revenue data into higher ad revenue. We group your players into eCPM value buckets, learn what each bucket is actually worth, and set bid floors accordingly — all through your mediation platform's own APIs. No SDK, no code, no app store release.

**Competitive frame:**

| | Segmenta | Metica (SmartFloors) | Nefta |
|---|---|---|---|
| Integration | Mediation API keys | SDK in your game | SDK / pre-mediation layer |
| Sits in the ad call | No | Yes — SDK loads & shows ads | Yes — pre-mediation |
| Time to live | Same day | Days to weeks + release cycle | Days to weeks + release cycle |
| Crash / ANR risk | None | Non-zero | Non-zero |
| Works on historic data | Yes | No | No |
| Mediation coverage | MAX first, AdMob & LevelPlay | MAX | Mediation-dependent |
| Decision granularity | Cohort / eCPM bucket / ad unit | Per player, per session | Per request |

> **Note for internal use, not for the site:** the last row is the honest trade-off. Don't hide it — own it. The FAQ handles it directly. Publishers who want per-impression realtime decisions will choose an SDK vendor; publishers who can't or won't ship an SDK are your entire market, and it's a large one.

---

## 1. Homepage

### 1.1 Hero

**Headline options — pick one, A/B the rest:**

1. **Higher ad revenue. Zero lines of code.**
2. **Bid floor optimisation without the SDK.**
3. **We don't need to be in your game to make it more valuable.**
4. **Your mediation data already knows what your players are worth. We act on it.**
5. **The bid floor optimiser that never touches your build.**

*Recommended: #2 as the H1 (it names the category and the wedge in five words), with #1 as the paid-search headline.*

**Subhead:**
> Segmenta connects to MAX, AdMob and LevelPlay, groups your players into eCPM value buckets, and optimises bid floors through your mediation platform's own APIs. No SDK to integrate. No release to ship. No risk to your crash-free rate.

**Primary CTA:** Book a 20-minute revenue review
**Secondary CTA:** See how it works

**Trust strip (under the fold line):**
> Built on the AppLovin MAX User-Level Ad Revenue API · Read-only until you say otherwise · SOC-2 aligned infrastructure

---

### 1.2 Problem section

**Section header:** Bid floors are the last big lever nobody is pulling properly.

**Body:**
> In-app bidding was supposed to make floors irrelevant. It didn't. Bid shading is everywhere, and most networks treat your floor as a signal about what the impression is worth. Set it too low and you leave money on every high-value impression. Set it too high and you lose fill on the users who were never going to pay much anyway.
>
> The right answer is different for every player. The problem is that finding it has always meant putting somebody else's code in your game.

**Three-column pain points:**

| | | |
|---|---|---|
| **One floor for everyone** | **Optimisation you can't ship** | **Insight you can't act on** |
| Your whale and your never-payer see the same floor, in the same country group, at the same price. | The vendor with the answer needs an SDK, a QA cycle, and a store submission. By the time it's live, the quarter's gone. | Your mediation dashboard tells you your average eCPM. It doesn't tell you which players generate it. |

---

### 1.3 How it works

**Section header:** Three steps. None of them are in your codebase.

**Step 1 — Connect**
> Paste in your MAX API key. Segmenta starts ingesting impression-level ad revenue data — including your history, if you have it. Setup takes about ten minutes and touches nothing in your game.

**Step 2 — Segment**
> Every user is placed into an eCPM value bucket based on what advertisers actually pay to reach them. Segmenta then enriches each bucket: IAP conversion rate, average first purchase price, hours to conversion, ad revenue share, LTV. You see, for the first time, which players are carrying your ad revenue and which are carrying your IAP revenue — and how little those two groups overlap.

**Step 3 — Optimise**
> Segmenta recommends bid floors per bucket and per ad unit, then pushes them live through the MAX Ad Unit Management API as a controlled A/B test. You approve every change, or let Segmenta run on autopilot. Results are measured inside MAX, against your own baseline, with no attribution argument to have.

**Micro-copy under the three steps:**
> If you don't like what you see, you disconnect an API key. There's nothing to remove from your game, because we were never in it.

---

### 1.4 Why no SDK (the money section)

**Section header:** "No SDK" isn't a limitation. It's the product.

**Four cards:**

**Live in a day, not a quarter.**
> No integration ticket. No engineer pulled off the roadmap. No QA pass. No app store review. No waiting for organic adoption of a new build before your optimisation reaches enough users to learn anything.

**Zero risk to the thing you actually care about.**
> Third-party SDKs are the leading cause of ANRs and cold-start regressions in mobile games. A monetisation gain that costs you 0.3% on your crash-free rate isn't a gain. Segmenta adds no bytes, no threads and no network calls to your app.

**We optimise your history, not just your future.**
> Because we read your mediation data rather than generate it, Segmenta can analyse impressions that already happened. You get your first eCPM bucket analysis from data you already own — before you've agreed to change anything.

**We never touch the auction.**
> Segmenta isn't in your waterfall, isn't a demand partner, and doesn't take a position in your ad calls. Your MAX setup stays your MAX setup. We change the numbers in it, not the plumbing under it.

---

### 1.5 Insights section

**Section header:** Your eCPM buckets, fully explained.

**Body:**
> Segmenta breaks your userbase into value buckets — $1–5, $6–10, $11–25, and up — with bucket ranges you define per app and per ad unit type, because a hyper-casual puzzle game and a mid-core RPG don't have the same distribution.

**For each bucket, you get:**

- Users and share of userbase
- IAP conversion rate
- Average first purchase price
- Share of total IAP revenue
- Share of total ad revenue
- Average hours to first IAP
- Hours to the 90th percentile of first purchases
- IAPs per payer
- IAP LTV
- Average first IAP value

**Closing line:**
> Split by iOS and Android, filterable by country, ad unit and cohort. This is the analysis most publishers have never run — because the data lives in a callback nobody warehouses.

---

### 1.6 Results / social proof

*Placeholder structure — populate as soon as you have a pilot.*

**Section header:** What publishers see.

> **[+X%] ad ARPDAU** — [Studio name], [game genre], [n] MAU
> "[One-sentence quote about how little work it was.]" — [Name, Title]

**If you have no case studies yet, replace with:**

**Section header:** Early access

> Segmenta is currently onboarding a small group of publishers running AppLovin MAX. Early partners get the full eCPM bucket analysis on their historic data at no cost, and shape the roadmap. We're taking on [n] more studios this quarter.

---

### 1.7 Final CTA

**Header:** Find out what your buckets look like.

**Body:**
> Connect a read-only MAX API key and we'll send you a full eCPM bucket breakdown of your last 90 days. No integration, no commitment, and you'll know within a week whether there's revenue on the table.

**CTA:** Get your free bucket analysis

---

## 2. Product page — Segmenta Floors

**H1:** Bid floors that know who they're pricing for.

**Intro:**
> Segmenta Floors sets the price of your ad inventory based on what your players are demonstrably worth — then holds the ratio of ad requests to filled opportunities inside a range you set, so you never trade fill for eCPM by accident.

**Sub-sections:**

**Bucket-level pricing**
> Users in your top eCPM buckets are consistently underpriced by a single global floor. Segmenta identifies the buckets where advertisers are already bidding well above your floor and raises the price on that inventory specifically — leaving your low-value inventory priced to fill.

**Routed through MAX, not around it**
> Where user-level floors aren't exposed by the mediation platform, Segmenta routes cohorts to dedicated ad units and controls the floor on those units via the MAX Ad Unit Management API. Your existing ad units and country groups are left untouched.

**Always an A/B test**
> Every floor change ships as an A/B test inside MAX. Segmenta monitors fill rate, impressions per DAU, eCPM and ad ARPDAU, and promotes the variant only when the uplift holds. Regressions roll back automatically.

**Guardrails you control**
> Set a minimum acceptable fill rate, a maximum floor, a maximum number of ad units Segmenta may create, and a change frequency. Or require manual approval on every recommendation. Segmenta will not do anything to your account you haven't authorised.

**CTA:** See a sample optimisation plan

---

## 3. Product page — Segmenta Insights

**H1:** The player segmentation that lives in your bid callback.

**Intro:**
> Every impression your mediation platform serves comes back with a revenue value attached. Aggregate that across a user's lifetime and you have the single best available proxy for what the advertising market thinks that player is worth. Segmenta warehouses it, buckets it, and joins it to your monetisation data.

**Feature blocks:**

**Normalised across mediation platforms**
> MAX, AdMob and Unity LevelPlay data is normalised into one consistent schema, so cross-platform comparison is possible without a data engineering project.

**Query builder and chat**
> Build segments visually, or ask in plain language: *"Which buckets convert to IAP within 48 hours?"* Every query is logged and auditable.

**Dashboards worth opening**
> KPI overview, bucket distribution, revenue attribution by bucket, and cohort views split by platform, country and ad unit.

**Your data, your call on where it lives**
> Hosted by Segmenta, or deployed into your own cloud environment. PII is anonymised on ingest either way.

---

## 4. Roadmap page

**H1:** What's next.

**Intro:**
> Segmenta starts with floors because floors are where the immediate, no-integration revenue is. The same bucket data unlocks more — and for publishers who *do* want an in-game component, these are the next products.

**Cards:**

**Smart IAP Offers** *(In development)*
> The hardest question in offer design is what price to show someone the first time. Segmenta already knows the historic first-purchase price of their eCPM bucket. Offers priced at the point where comparable players actually convert, with dual-price upsells after the first purchase.

**Offerwall Timing** *(In development)*
> Use each bucket's IAP conversion rate and 90th-percentile time-to-purchase to decide *when* a player has effectively declared they'll never buy — and unlock an offerwall for them at that moment, not before. Measured against a holdout so you can see the churn cost, not just the revenue.

**Cross-platform benchmarking** *(Planned)*
> Anonymous, aggregated benchmarks so you can see whether your $51–100 bucket converts like everyone else's.

**Anomaly alerts** *(Planned)*
> Alerts for sudden eCPM shifts, fill collapses and bucket distribution drift.

**Honest framing line at the bottom of the page:**
> Offers and Offerwall will require a lightweight SDK. Floors and Insights never will. You can use one without the other.

---

## 5. Comparison page — "Segmenta vs SDK-based optimisers"

**H1:** Do you actually need an SDK to optimise bid floors?

**Intro:**
> Short answer: it depends on what you're optimising. Longer answer below, written as fairly as we can manage.

**When an SDK-based tool is the right call:**
> If you need a floor decision made per impression, in the moment, using in-session behavioural signals — device state, current session length, live progression — then that decision has to be made on-device. Metica and Nefta do this, and they do it properly. If your studio can absorb an integration and a release cycle, and your titles have the volume to justify per-request modelling, that's a legitimate path.

**When Segmenta is the right call:**
> - You can't get engineering time for a monetisation SDK this quarter
> - You've been burned by third-party SDK stability before
> - You run a portfolio and need something you can roll out across twenty titles without twenty integrations
> - You want to see the analysis before you commit to anything
> - You run more than one mediation platform and want one view across them
> - Your legal or platform team won't approve another data-collecting SDK in the build

**The comparison table** *(as in section 0)*

**Closing:**
> We think most publishers should start with the version that costs them nothing to try and can't break anything. If you outgrow it, you'll have a year of clean bucket data to hand the next vendor.

---

## 6. Security & compliance page

**H1:** Boring, in the way you want it to be.

- Read-only API access by default. Write access to ad unit management is granted explicitly, per app, and revocable in one click.
- JWT-based authentication, HTTPS everywhere, role-based access control across UI and API.
- Two roles: Admin (full create/edit/delete on users, publishers, apps and reports) and Viewer (read-only).
- Full audit log of every query executed and every change pushed to your mediation account.
- PII anonymised on ingest. Segmenta stores mediation-assigned user identifiers, not personal data.
- Hosted deployment or deployment into your own infrastructure.

---

## 7. Pricing page

*Structure only — you'll need to decide the model. Two credible options:*

**Option A — Revenue share on uplift**
> Segmenta is free until it makes you money. We take [X]% of measured incremental ad revenue, calculated against the A/B baseline running inside your own MAX account. If the test doesn't win, you don't pay.

*This is the strongest offer for a no-SDK product, because the A/B test inside MAX makes the measurement uncontestable. It's also what removes the last objection.*

**Option B — Flat platform fee by MAU tier**
> Insights: free up to [n] MAU. Floors: from $[X]/month per app.

**Recommended page copy either way:**
> No integration cost. No engineering cost. No minimum term for the first 90 days.

---

## 8. FAQ

**Do I really not have to integrate anything?**
> Correct. Segmenta reads your mediation platform's user-level ad revenue API and writes back through its ad unit management API. Both are server-to-server. Nothing changes in your app binary.

**How can you optimise per user without being in the app?**
> We don't optimise per user in real time — we optimise per value bucket, and we route buckets to ad units whose floors we control. For bid floor pricing this captures most of the available uplift, because the underlying signal (what a given player is worth to advertisers) is stable across sessions. Decisions that genuinely depend on in-session state, like interstitial cooldowns, need an SDK, and we're honest that we don't do those.

**Which mediation platforms do you support?**
> AppLovin MAX is fully supported and prioritised. Google AdMob and Unity LevelPlay are supported for ingestion and analytics, with floor optimisation following.

**Will you change things in my MAX account without asking?**
> Only if you turn on autopilot. Default is recommend-and-approve. Every action is logged.

**What if it doesn't work?**
> The A/B test tells you, in your own dashboard, in your own numbers. Then you revoke the API key. There is no removal project.

**Do you take a cut of my ad revenue as a demand partner?**
> No. We are not in your auction and we don't sell your inventory. [Add pricing model line.]

**Can I get the insights without the optimisation?**
> Yes. A lot of publishers start there.

**How much data do you need before recommendations are useful?**
> Roughly 30 days of impression-level history, or 14 days at higher volumes. If you have historic data available through the API, we can often produce a first analysis immediately.

---

## 9. Navigation & site structure

```
Home
Product
  ├── Floors — bid floor optimisation
  ├── Insights — eCPM segmentation
  └── Roadmap
Why no SDK
Compare
Pricing
Resources
  ├── Blog
  ├── Case studies
  └── Docs
Company
  ├── About
  └── Careers
[Book a demo]  ← persistent button, top right
```

---

## 10. SEO metadata

**Homepage title tag:**
`Segmenta AI — Bid Floor Optimisation Without an SDK | Mobile Apps & Games`

**Homepage meta description:**
`Increase ad revenue from your mobile game without integrating an SDK. Segmenta segments players into eCPM value buckets and optimises bid floors through your mediation platform's API. Live in a day.`

**Target keyword clusters:**
- Primary: *bid floor optimisation*, *bid floor optimization mobile games*, *AppLovin MAX bid floor*
- Secondary: *ad revenue optimisation without SDK*, *eCPM segmentation*, *user-level ad revenue API*, *MAX ad unit management API*
- Comparison: *Metica alternative*, *Nefta alternative*, *SDK-free ad monetisation*
- Long tail: *how to set bid floors in AppLovin MAX*, *what is a good bid floor for rewarded video*

**Recommended launch blog posts** *(these carry the positioning and the SEO):*
1. "Why your bid floor is a signal, not a price"
2. "We analysed [n]M impressions. Your top 10% of ad-value players generate [X]% of your ad revenue."
3. "You don't need an SDK to optimise bid floors — here's the maths"
4. "eCPM buckets: the segmentation model hiding in your bid callback"
5. "The real cost of a monetisation SDK" *(ANRs, cold start, release cycles — cite public data)*

---

## 11. Tone of voice notes

- **Speak to monetisation managers and heads of ad ops**, not to CEOs. They know what bid shading is. Don't explain it.
- **No "AI-powered" in the hero.** Every competitor says it. Your differentiator is operational, not algorithmic — lead with that. Keep the AI claims for where you can substantiate them.
- **Quantify or cut.** "Significant uplift" is noise. Either put a number on it or describe the mechanism instead.
- **Be openly honest about the limitation.** The comparison page that fairly describes when Metica is a better fit will win you more deals than the one that doesn't. This audience has been oversold to for a decade.
- **British or American spelling — pick one.** This draft uses British ("optimisation"). Given the buyer base skews US and Israeli, American may convert better.

---

## Open questions for you

1. **Pricing model** — rev-share on uplift is the strongest story for a no-SDK product. Is that commercially viable for you?
2. **Do you have a pilot publisher?** The site needs one number in it. Even "+11% on one title" beats a page of adjectives.
3. **Is the SDK dead or deferred?** If Offers and Offerwall are still coming, the roadmap page as written is right. If you've dropped them, cut section 4 entirely and go all-in on the no-SDK identity.
4. **AdMob and LevelPlay** — supported at launch, or MAX-only? The copy currently promises ingestion for all three. Don't ship that if it isn't true.
