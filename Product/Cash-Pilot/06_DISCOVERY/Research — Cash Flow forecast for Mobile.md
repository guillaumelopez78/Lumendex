# Research — Cash Flow forecast for Mobile

# Objectives

Determine which subset of the desktop cash flow forecast information is essential to display on mobile, for users who consult the tool briefly in low-attention contexts: in transit, in a car, or in front of a customer.

The desktop tool currently exposes the following information:

- Bank account selection
- Current balance
- Projected balance in 8 weeks
- Cash runway
- Cash flow forecast graph including: balance curve, cash in/cash out histograms by time period
- Per-period summary: cash in, cash out, net result, balance at end of period
- Transaction details

The mobile view must not replicate the desktop. Its sole purpose is to give the user a fast, reliable answer to the question `*"Is my cash position healthy right now?"*` and redirect them to desktop if they need deeper analysis.

The output of this research is a scoped content decision: which KPIs and/or graph elements to include in the mobile view for the first mobile feature release.

---

# Constraints

<aside>
📕

- **Read-only display.** The mobile view will show information only. No bank account switching, no date range selection, no transaction interaction.
</aside>

<aside>
🖥️

- **Desktop is the primary tool.** The cash flow forecast tool is intentionally desktop-first. Mobile must cover the "quick check" use case only — not offer a degraded version of the full experience.
</aside>

<aside>
⏳

- **Not a real-time tool.** The forecast is not designed for live monitoring. The mobile view must not imply otherwise (no live indicators, no push alerts).
</aside>

---

# Options / Possible Solutions

## Option A — Essential KPIs only

Display **two KPIs**:

- Projected balance in 8 weeks
- Cash runway

#### **Does it answer *"Am I safe in the near term?"*  : YES**

- Projected balance gives a concrete amount on a fixed horizon.
- Cash runway gives a time-based risk signal ("your cash runs out in X months").
- One screen. Two numbers. No scrolling.

#### **Risk:**

Some users may find two isolated numbers insufficient, too short.

---

## Option B — Simplified graph view

Display a **balance curve only** (no cash in/cash out histograms), with three KPIs beneath it, related to the time period that is selected:

- Cash in
- Cash out
- Balance at end of period

#### **Does it answer *"Am I safe in the near term?"*  : depends on the graph scale, time coverage**

#### **Risk:**

- A graph requires more visual attention than a KPI.
- In genuinely low-attention contexts (car, customer meeting), it may be harder to read quickly.
- The link between the time period selected and the KPIs is going to be hard to create.

---

## Option C — KPIs + simplified graph (combination of A and B)

Display **two KPIs**:

- Projected balance in 8 weeks
- Cash runway

Display a **balance curve only** (no cash in/cash out histograms), with three KPIs beneath it, related to the time period that is selected:

- Cash in
- Cash out
- Balance at end of period

**Does it answer *"Am I safe in the near term?"*  : YES**

**Risk:**

- increases screen length.
- On mobile, this may require scrolling, which defeats the "quick glance" purpose.
- Could result in users seeing only the KPIs and ignoring the graph, making the graph redundant.

---

## Selection process

<aside>
🗣️

**Research method:** User interviews with existing desktop users who also have the mobile app installed.

**Target sample:** 5–8 users, mix of business sizes and usage frequency.

**Target profile:**

- Recurring users of the mobile application
- Use both mobile app and desktop version
- Shine customer since +6months
</aside>

**Key interview questions:**

When you are away from your desk

1. Do you ask yourself cash flow related questions?

If so :

1. What cash-related question are you most likely trying to answer?
2. When and where are you asking yourself these questions? Example: on the field with customer or at home during non office hours?
3. What would make you open the desktop version after checking your mobile application?

**Decision criteria:** A solution is validated if users can answer *"Is my cash position healthy right now?"* within 5 seconds of opening the mobile view, without scrolling and without switching to desktop to interpret the data shown.

[](Research%20%E2%80%94%20Cash%20Flow%20forecast%20for%20Mobile/Sans%20titre%20372f148b3ab78080869ddac49f307da2.md)---

## 📚 Related Documentation

**Hub:** [[../../../../Cash Pilot - Overview.md|Overview]]
**Product:** [[../../../../product-and-features.md]]
