# The Grove

> _As You Serve, You Deserve._

The partner-facing dashboard for **TriBe (Trifecta Benefits)**, a Medicare and ACA insurance distribution agency launching June 2026.

The Grove turns a one-time lead-vendor relationship into a true partnership. It gives independent lead generators — starting with launch partner AJ — a transparent, real-time view of every member they've helped enroll and exactly when they'll be paid for it.

Mobile-first. Brand-forward. Built on the principle that a partner who can see their downstream income in detail will refer better leads, stay longer, and grow with us.

---

## Who it's for

The Grove serves **lead generation partners** — independent operators who run their own marketing, ads, intake forms, and qualification, then route warm prospects to TriBe's licensed agents to close. They are sophisticated, performance-driven operators who already know their numbers. They are not insurance agents. They are not licensed. They are partners on the front end of a long revenue stream.

Today that's AJ, who funnels leads through Go High Level into TriBe's licensed agents (Mark and Michael). Tomorrow it's a roster of similar partners, each with their own GHL subaccount, their own lead pipeline, their own income at stake.

The Grove is **not for**:

- TriBe's licensed agents (they use **MediCopilot** during calls and an internal CRM after)
- Members themselves (who deal with TriBe through the licensed agent and the carrier directly)
- TriBe's operations team (who use a separate operator console)

This focus shapes everything about what The Grove does and doesn't show.

---

## The three-tier income model

TriBe and its lead partners share revenue across three structured tiers. A given enrolled member belongs to exactly one tier, set at the moment the lead is sourced. The Grove makes all three tiers visible and traceable.

### Tier 1 — Short Stream

TriBe buys the lead at a flat **$50 fee, paid once**. The member is written under TriBe. Partner is paid up-front; the relationship ends there.

### Tier 2 — Mid Stream

Partner provides the lead at no upfront cost. If the lead enrolls, the partner receives the **full monthly carrier commission for 12 months** from the enrollment date. Member is written under TriBe. Aligns partner income with conversion quality and gives them a year of recurring revenue per enrolled member.

### Tier 3 — Long Stream

A separate jointly-owned LLC — **Best Plans LLC** (currently 50/50 owned by Shawn and AJ, formed via LegalZoom and active) — holds these enrollments as the agency of record. Mark writes the policy as the licensed agent under Best Plans. Partner receives **50% of carrier commissions indefinitely**. Structured separately so the book of business stays clean and sellable, and so future Trifecta acquisition is a clean option.

The Grove visualizes each tier as a distinct **Stream of Service** with its own visual treatment — Tier 1 still and transactional, Tier 2 a steady flowing stream, Tier 3 a slow-compounding river — and tracks each stream's progress against doubling milestones (0 → 500 → 1,000 → 2,000 members served).

---

## What The Grove actually does

The Grove is built around a single core question that every lead partner asks every day:

> **"How am I doing, and when am I getting paid?"**

The product answers that across four primary surfaces.

### Home (the Grove screen)

The landing experience. Hero metric is **members served**, not dollars — a deliberate choice that frames the partner's contribution in lives helped rather than commissions earned, with a circular progress ring tracking toward the next doubling milestone. The mantra _"As You Serve, You Deserve"_ lives here.

Below the hero: snapshot cards for each of the three Streams of Service showing current member counts, progress to next double, and visual movement that distinguishes the tiers. Beneath that: a **From TriBe** pane for active workflows (purchase requests, invoices to send, status updates) and a **Rooted in Truth** pane that surfaces the philosophical anchor of the partnership (Kahneman/Deaton research on log-income and life satisfaction, properly cited).

### Ledger

The cash-flow planner. Every payment event the partner is owed — past, current, and projected — surfaced as its own row, grouped chronologically (Today, Tomorrow, This Week, Next Week, Later in Month, then by month). Each row shows the lead identifier, tier badge, amount, source (TriBe vs Best Plans LLC), and date.

Three at-a-glance metrics live at the top: **Next Payout**, **Next 30 Days**, **Year to Date**. Filter pills toggle between tiers. A search bar finds any lead by ID, plan, or county.

Tap any row → a slide-up sheet shows the full payment timeline for that single member, with checkmarks on past payments, a coral marker on the next upcoming, and projection out 12 months (Tier 2) or 60 months (Tier 3). Earnings to date, expected remaining, and lifetime projection are all surfaced in one panel.

This is the most-used screen and the heart of why the partner stays engaged.

### Streams _(planned)_

Per-tier deep-dive. Income curves over time, projection vs. actuals, conversion rates, retention by tier. The analytics layer that lets a partner reason about which kind of lead generates the best long-term economics.

### Profile _(planned)_

Partner identity, contact info, payout method (masked), tax form (W-9), notification preferences, support. Built so it can extend later when partners need to be licensed in their own right.

---

## What The Grove deliberately does not show

The Grove operates under one immutable rule: **no protected health information, ever, anywhere on this surface.**

Members appear as their **GHL Contact ID** (the stable identifier that flows from the partner's lead-gen system through every downstream surface) plus a non-identifying friendly label — typically state and plan tier, never a name. The partner already knows who their leads are because they originated them; The Grove never has to display that mapping back. This is by design: it keeps the Grove on the cheap, no-HIPAA-exposure side of the architecture and protects member privacy by default.

**The Grove never shows:**

- Member full names, phone numbers, email addresses
- Member dates of birth or Medicare ID numbers
- Policy numbers, exchange subscriber IDs, or member responsibility amounts
- Anything else considered PHI under HIPAA

**The Grove does show:**

- Lead IDs (the partner's own identifiers, traceable on their side)
- Plan names and on/off-exchange status
- Effective dates, term dates, paid-through dates
- Monthly premium amounts (for partner economics, not member protection)
- County and state (territorial, not address)
- Enrollment status

This separation is foundational, not cosmetic. It's why The Grove can run on cheap public infrastructure (Vercel, Cloudflare) while everything that does touch PHI runs on a separate compliance-grade Google Cloud foundation. **The boundary is whether a screen ever displays a member's name. Grove never does.**

---

## Brand and visual identity

The Grove's design language is **"Digital Forest Floor"** — dark editorial photography of a twilight meadow, glassmorphism panes that float over a moody background, italic-serif headlines (Lora Italic) acting as the protagonist voice, sans-serif (Montserrat) for structure, and a restrained palette.

### Palette

| Token            | Hex       | Use                              |
| ---------------- | --------- | -------------------------------- |
| Deep Teal        | `#007B7F` | Primary actions                  |
| Coral Sunset     | `#F47C6E` | Accents, hero numbers            |
| Frosted White    | `#F5F5F5` | Foreground                       |
| Void             | `#06080A` | Ground                           |

### The metaphor

Every plant in the meadow is one real person served. Not a building, not a sanctuary, not a corporate visualization. **A lit wildflower in twilight.** The hero number on the home screen represents members served — currently 247 in the prototype data — each one represented by a real plant lit somewhere in the dark field.

### The mantra

**"As You Serve, You Deserve,"** grounded in Kahneman & Deaton's 2010 PNAS research showing life satisfaction increases linearly with the log of income — meaning each doubling matters as much as the last. This is why the milestone structure is geometric (500, 1,000, 2,000) rather than linear.

### Typography signature

Italic serif for the meaningful, weighty moments (_"You Deserve."_); tracked sans-caps micro-labels at `0.18em` letter-spacing for structure (`STREAMS OF SERVICE`); generous negative space and breathing room throughout.

The result is a partner dashboard that reads more like a thoughtful editorial magazine than a SaaS dashboard. That's intentional. It signals that the partner is a **co-founder of the relationship**, not a vendor in a queue.

---

## Where the data comes from

The Grove sits at the end of a data pipeline:

1. **Lead origination.** Partner generates a prospect through their own marketing and routes them to a GHL subaccount. Each prospect gets a **GHL Contact ID** at this moment — that ID becomes the lead's permanent identifier across every surface.
2. **Agent contact.** The lead is routed to a TriBe-licensed agent (Mark or Michael), who uses **MediCopilot** as their call coach during the conversation. Compliance disclosures are captured. If the prospect enrolls, the carrier's enrollment system is updated.
3. **Carrier reconciliation.** Daily/weekly, broker portal CSVs from carriers (Ambetter, Oscar, etc.) export enrollment status, paid-through dates, premiums, and commission detail. These flow into TriBe's operator console.
4. **Tier assignment.** Each enrolled member is tagged with its tier (1, 2, or 3) based on which lead source produced them.
5. **Grove rendering.** The operator console exposes only the **non-PHI subset** — lead ID, tier, plan name, effective dates, premium, county, state, status — to The Grove. The Grove computes payment schedules from rules (tier rules, street-level commission rates, payment timing) and renders the partner-facing surfaces.

In the prototype today, all of this is mocked. In v1, the broker CSVs are imported manually and the operator parses them. In v2+, this is automated end-to-end.

---

## Where we are

| Surface / capability                | Status                                      |
| ----------------------------------- | ------------------------------------------- |
| Visual design language              | Complete and locked                         |
| Home screen prototype               | Built                                       |
| Ledger payment-schedule prototype   | Built                                       |
| Streams deep-dive page              | Not yet built                               |
| Profile page                        | Not yet built                               |
| Real GHL integration                | Not yet built (currently mocked)            |
| Real CSV ingestion                  | Not yet built (currently mocked)            |
| Real auth and partner accounts      | Not yet built                               |
| Production hosting                  | Not yet provisioned (Vercel target)         |

---

## Why this matters

The standard lead-vendor relationship is transactional and brittle. Vendor sells lead, gets paid, moves on. There's no shared incentive in member outcomes, no transparency into long-term economics, no reason for the vendor to invest in higher-quality lead flow over time.

The Grove is the product expression of a different relationship — one where the partner sees, in detail, that their leads have become real members in real plans paying real premiums, and that money is flowing back to them on a known schedule for a known duration. The dashboard is the **visible manifestation** of an income arrangement that, on paper alone, would just be three pages of contract language nobody reads.

Built well, The Grove makes a partnership feel like a partnership. That's the wedge. And it's the thing TriBe can offer that bigger, more established agencies — who treat lead vendors as commodity inputs — structurally cannot.

---

## Architecture at a glance

- **Grove (this repo)** — partner dashboard. Vercel + Cloudflare. **No PHI. Ever.**
- **Operator console** — internal admin surface for TriBe ops. Compliance-grade GCP. Holds PHI.
- **MediCopilot** — agent-side call coach. Separate surface.
- **Source of truth** — GHL Contact ID flows from lead origination through every downstream system.

---

## Tech stack _(target)_

- Next.js (App Router) on Vercel
- Tailwind for styling, with design tokens mirroring the Digital Forest Floor palette
- Mock data layer today; real GHL + carrier-CSV integrations to follow in v1/v2
- Cloudflare in front for edge + DNS

---

## Repo status

Bootstrapping. README first, prototypes to follow. See `Where we are` above for the live build state.

---

_The Grove is part of the TriBe (Trifecta Benefits) product family. PHI lives elsewhere by design._
