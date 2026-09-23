# Segmenta AI — Privacy Content
### Draft for review. Not legal advice — have a qualified adviser check this before publishing.

---

## Part 1 — Micro-copy for under the Join form

This is the line people actually read. Keep it to one sentence and make it specific about what happens next.

**Recommended:**

> We'll use these details to contact you about Segmenta and nothing else. No newsletter, no list sales. See our [Privacy Policy](/privacy).

**Alternatives, depending on how formal you want to be:**

1. *Plain:*
   > We use what you enter here to get in touch about Segmenta. Nothing else. [Privacy Policy](/privacy)

2. *Explicit about the legal basis (useful if your buyers are EU enterprises):*
   > We process these details under legitimate interest to respond to your enquiry, and delete them if nothing comes of it. [Privacy Policy](/privacy)

3. *With an opt-in checkbox, if you also want to send product updates:*
   > ☐ Send me occasional product updates. Unticked, we'll only contact you about this enquiry. [Privacy Policy](/privacy)

**On the checkbox:** only add it if you genuinely intend to send updates. An unticked box that nothing depends on is friction for no gain. Never pre-tick it — a pre-ticked consent box is invalid under UK and EU GDPR, and it's the single most common mistake on B2B forms.

---

## Part 2 — Cookie / analytics notice

**If you run no analytics and no third-party scripts** (achievable — this site is one static page):

> This site sets no cookies and runs no analytics. Nothing about your visit is tracked.

That is a genuine differentiator for a company whose whole pitch is "we don't put code in your app." It's worth engineering for.

**If you do add analytics**, use a privacy-preserving tool (Plausible, Fathom, self-hosted Umami) that doesn't require a consent banner, and say so:

> We use [tool] for basic visitor counts. It sets no cookies and collects no personal data, so there's no banner to dismiss.

**If you end up needing marketing pixels** (LinkedIn Insight Tag, Meta pixel, Google Ads), you will need a proper consent banner with reject-as-easy-as-accept. Weigh that against the fact that your first hundred customers will come from conversations, not retargeting.

---

## Part 3 — Privacy Policy page

Replace everything in `[square brackets]` before publishing.

---

# Privacy Policy

**Last updated:** [date]

This policy explains what Segmenta does with personal data. It covers two quite different situations, and we've separated them because the difference matters:

1. **Data about you** — if you visit this site, fill in our form, or become a customer. Here we decide what happens to the data, so we're the *controller*.
2. **Data we process for our customers** — the mediation data a publisher connects to Segmenta. Here the publisher decides what happens, and we only act on their instructions, so we're a *processor*.

## Who we are

Segmenta AI is [full legal entity name], a company registered in [jurisdiction] under number [company number], at [registered address].

For any privacy question, email [privacy@segmenta-ai.com].

---

## Part A — When we are the controller

### What we collect

**When you fill in the Join form:** your name, work email address, company name, and the two answers you give about your app's scale and mediation setup.

**When you email us:** whatever you put in the message, and your email address.

**When you become a customer:** the contact details of the people at your company who use Segmenta, and billing details if applicable.

**When you visit this site:** [Nothing. We set no cookies and run no analytics. / Aggregate visit counts via [tool], which sets no cookies and does not identify you.]

We do not buy contact lists, and we do not enrich what you give us with data from third-party providers.

### Why we use it, and on what basis

| What we do | Why | Legal basis |
|---|---|---|
| Reply to your enquiry and arrange a conversation | You asked us to | Legitimate interest |
| Send product updates | You ticked the box | Consent — withdraw any time |
| Run and support your account | To deliver what you're paying for | Contract |
| Keep accounting and tax records | We're required to | Legal obligation |

You can object to processing based on legitimate interest at any time, and withdraw consent at any time, by emailing us.

### How long we keep it

- **Enquiries that go nowhere:** deleted within [12] months of last contact.
- **Enquiries that become conversations:** kept while the conversation is live, then [24] months.
- **Customer records:** for the life of the contract, then [6] years for accounting.

### Who else sees it

We use a small number of service providers, and only these:

- [Email provider — e.g. Google Workspace] — hosting our email
- [Form/CRM provider] — receiving and storing form submissions
- [Hosting provider] — serving this website
- [Add any others]

Each is bound by a data processing agreement. We do not sell personal data, share it with advertisers, or use it for anything other than the purposes above.

### Where it goes

Our providers are located in [the UK / the EEA / the United States]. Where data leaves the UK or EEA we rely on [UK International Data Transfer Agreement / EU Standard Contractual Clauses / adequacy decisions].

### Your rights

Under UK and EU data protection law you can ask us to: give you a copy of your data, correct it, delete it, restrict what we do with it, hand it to another provider, or stop processing it. Email [privacy@segmenta-ai.com] and we'll respond within one month.

If you're unhappy with how we've handled it, you can complain to the [Information Commissioner's Office (ico.org.uk)] or your local supervisory authority.

---

## Part B — When we are the processor

This part is about the data a publisher connects to Segmenta. If you're a player in a game that uses Segmenta, the game's publisher — not us — is responsible for your data, and their privacy policy governs it.

### What Segmenta receives

Segmenta reads impression-level advertising data from the mediation platform a publisher has connected. That data consists of:

- Mediation-assigned identifiers — the pseudonymous IDs the mediator uses for users
- Ad revenue values, ad unit identifiers, timestamps
- Country and platform (iOS or Android)

### What Segmenta does not receive

Segmenta does not receive names, email addresses, phone numbers, precise location, device advertising identifiers, or any direct identifier. We do not attempt to re-identify anyone, and we do not build cross-publisher profiles: each publisher's data is analysed only for that publisher.

### What we do with it

We group users into value buckets, calculate aggregate statistics per bucket, and recommend bid floors. We do not use one customer's data to improve another customer's results, and we do not use it to train models offered to anyone else.

### Where it lives

Data is held [in our infrastructure in [region] / in the customer's own cloud environment, at their choice]. Access is limited to named Segmenta staff who need it, every query is logged, and connections are read-only unless the customer explicitly grants write access to their ad unit configuration.

### On instruction and deletion

We process this data only on the customer's documented instructions, under a data processing agreement. When a customer disconnects, we stop processing immediately and delete their data within [30] days. There is nothing to remove from their app, because Segmenta was never installed in it.

### Sub-processors

Our current sub-processors for customer data are: [list — e.g. cloud host, warehouse provider]. We'll give customers notice before adding another.

### Security

[Describe honestly what you actually do. Encryption in transit and at rest, role-based access, audit logging, credential handling. Do not claim a certification you don't hold.]

---

## Changes to this policy

We'll post any changes here and update the date at the top. If a change materially affects how we handle your data, we'll tell customers directly.

**Questions:** [privacy@segmenta-ai.com]

---

## Notes on things you need to decide

1. **Legal entity and registration.** The policy is unenforceable and non-compliant without a named entity and address.
2. **ICO registration.** If you're UK-established and processing personal data, you likely need to register with the ICO and pay the data protection fee. Check — it's inexpensive and the omission is noticed in vendor reviews.
3. **Is bucket data personal data?** Pseudonymous mediation IDs are still personal data under GDPR. The policy above treats them as such, which is the defensible position. Don't be tempted by the "it's just anonymous analytics" framing — it doesn't survive scrutiny and it will cost you an enterprise deal.
4. **A DPA template.** Every publisher above a certain size will ask for one before connecting an API key. Having it ready shortens the sales cycle noticeably.
5. **Retention numbers.** I've put placeholders in brackets. Pick numbers you'll actually honour rather than numbers that sound careful.
6. **Sub-processor list.** Keep it current. Customers with a DPA are entitled to notice of changes.
