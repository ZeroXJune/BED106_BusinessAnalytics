# Dashboard Presentation Script

**Checkpoint 3, Task 3.4 — live in-class presentation**
BED 106 Business Analytics · Mini Capstone Project
Talibon Polytechnic College

Ten minutes, presented live with the dashboard on screen. All three speak.

| Speaker | Covers | Time |
| --- | --- | --- |
| **Alber** | Opening and Page 1 — Executive Summary | 3:00 |
| **Julebeth** | Page 2 — Trend & Comparison | 3:00 |
| **Mardy** | Page 3 — Deep Dive, including the live demonstration | 3:30 |
| **Alber** | Close and hand to questions | 0:30 |

Measured at a normal speaking pace this is **8 minutes of talking**, which
lands at nine to ten once the page switches and the two deliberate pauses in
the demonstration are counted. That leaves a little room, which is the right
way round for a ten-minute slot.

*Lines in italics inside brackets are what to click. Do not read them aloud.*

**Before you record this in your own words.** Section 3.2 of the brief does not
allow AI-generated analysis. This script was drafted with AI help, so change
the wording as you rehearse — say it the way you would say it. The numbers and
the reasoning stay; the phrasing should become yours.

---

## What the brief requires

Check each off during the rehearsal, not on the day.

- Walk through **all three** dashboard pages, narrating the business story
- Demonstrate **at least one** interactive feature live — ours is the segment
  slicer on Page 3, with the drill-through as a second
- Answer **at least two** questions from the instructor or classmates
- **Every member speaks**

---

## Before you start

- Power BI Desktop open on `Checkpoint_3_Dashboard.pbix`, **not** the PDF
- **All slicers cleared** on all three pages. A leftover filter from rehearsal
  makes every number on screen wrong, and it is the single most common way a
  live demo goes bad
- Page 1 showing, window maximised, presentation mode if the projector is small
- The PDF export open in a second window as a fallback if Power BI hangs
- Agree who drives the mouse. The driver should not be the person speaking

---

# Alber — Opening and Page 1

*[Page 1 on screen. All slicers cleared.]*

Good day. We are Alber, Julebeth and Mardy, and this is our dashboard for the
sales trend analysis.

The business is a multi-category retailer — electronics, furniture and office
supplies — trading across six US states. The question we were asked to answer
is simple to state: the company grew, and then it stopped. Nobody could say
why.

This dashboard is built to answer that in three pages. What happened, what
drove it, and who it happened to.

*[Point to the four KPI cards across the top.]*

Starting with the headline figures. The company is writing **twenty orders a
month**. At its 2022 peak it was writing twenty-four. Revenue per month is
**100,206**, against a peak of **121,648** — a gap of **17.6 percent**.

Now look at the third card. Margin is **25.64 percent**. At the peak it was
**26.93**. It barely moved.

That is the finding that shaped this entire dashboard. If margin had collapsed,
the answer would be that the company discounted too hard, and you would not
need a dashboard to see it. Margin held steady while revenue fell. That means
the company is writing **fewer orders, not worse ones**.

*[Point to the line chart.]*

This is revenue per month across the fifty-seven months we analysed, April 2020
to December 2024. You can see the shape: it climbs to a peak in late 2022, and
then it flattens. Two different periods, not one trend.

*[Point to the dashed line on the chart.]*

The dashed line marks that 2022 peak, so the gap is visible rather than
something you have to work out.

*[Point to the table on the right.]*

And the table breaks it down by year. One column there is worth explaining —
**months covered**. 2020 shows nine, not twelve, because our data starts on the
22nd of March. Every figure on this dashboard is measured **per month** for
that reason. Comparing a nine-month year against a full one was a mistake we
made earlier in this project and corrected, and this column is how we make sure
it cannot happen again.

*[Hand over.]*

So that is what happened. Julebeth will show you what drove it.

---

# Julebeth — Page 2

*[Switch to Page 2.]*

Thank you. This page answers which parts of the business are responsible.

*[Point to the line chart, top left.]*

Here is revenue by category over time — three lines, one per category. The
important thing is that they **diverge**. They are not falling together.

*[Point to the bar chart, top right.]*

This is where it becomes clear. Each bar is one sub-category, and the length is
how much its revenue changed between 2023 and 2024. Red is a loss, green is a
gain.

Look at the top bar. **Printers lost 136,865.** That is a seventy-one percent
collapse in one year, and on its own it is **more than half** of the entire gap
between the 2022 peak and 2024.

And now look at the bottom. **Paper gained 85,689** — up a hundred and
forty-nine percent.

So this is not a general slowdown. Two opposite things are happening at the
same time. Every Electronics sub-category fell. Every Office Supplies
sub-category grew. The company-wide figure is just the average of the two,
which describes neither of them.

*[Point to the quarterly chart, bottom left.]*

The second finding is about timing. These are three separate panels, one per
category, showing which quarter each one sells in.

If you looked at the company as a whole you would say Q4 is the peak quarter.
But look at Electronics on the left — it peaks in **Q2**, at nearly thirty-one
percent of its own annual revenue. Furniture and Office Supplies peak in Q4.

That matters because stock and staffing are planned on the blended curve. That
curve is wrong for all three categories, and it mistimes about a third of the
business.

*[Point to the margin chart, bottom right.]*

Last on this page — margin by sub-category. We put this next to the revenue
chart deliberately, because **the ranking is different**. The sub-categories
that bring in the most revenue are not the ones that earn the most margin. That
difference is the whole reason the next page exists.

*[Hand over.]*

Mardy will take the deep dive.

---

# Mardy — Page 3 and the live demonstration

*[Switch to Page 3.]*

Thanks. This page is about who, not what — and it is where we applied
clustering.

*[Point to the left scatter.]*

On the left, our twelve sub-categories, grouped by k-means into three segments.
Growth is along the bottom, margin up the side, and the bubble size is total
revenue. The algorithm separated them into **Growth Engines**, **Declining
Lines**, and a small low-margin group in the middle. Printers sits at the far
left edge of the declining group.

*[Point to the right scatter.]*

On the right, the same method applied to all **807 customers** — clustered on
value, margin and how recently they bought.

*[Point to the table, bottom left.]*

And this table is the finding we would most want you to take away.

Look at the bottom row. **Thin-Margin Buyers** are our largest group —
forty-three percent of customers, and nearly a third of all revenue. Now look
at the profit column. **Eighteen point seven percent.**

Now the row above it. **High-Margin Buyers** — a smaller group, bringing in
*less* revenue — and they produce **forty-two point six percent** of the
profit.

So the largest group of customers by revenue returns the least profit. A sales
push aimed at revenue would chase exactly the wrong group of the two.

### The live demonstration

Let me show you that the dashboard actually responds to this.

*[Click "Thin-Margin Buyers" on the segment slicer at the bottom. Pause — let
the page redraw before speaking.]*

I have selected just that one segment. Every visual on this page has refiltered
to those 350 customers.

*[Point to the scatter, then the table.]*

You can see the scatter has collapsed to the low-margin band, and the table now
shows only that group.

*[Clear the slicer. Pause again.]*

And clearing it brings the whole book back.

*[Optional, if time allows: go to Page 2, right-click the Printers bar →
Drill through → 3 Deep Dive.]*

There is a second interaction worth showing. From the sub-category chart on
Page 2, right-clicking any bar drills through to this page filtered to it — so
you can go from "Printers lost 136,865" straight to everything behind it in one
click.

*[Return to Page 3, slicers cleared.]*

### The two things we ruled out

Two visuals on this page exist to show what is **not** true, and we think that
matters as much as the rest.

*[Point to the map.]*

The map. Revenue by state spans only twenty-eight percent across five years,
and no state moves against the others. **Geography is not driving this.** We
put it on the dashboard so you can check that rather than take our word for it.

*[Point to the bottom-right scatter.]*

And this one. Units sold against order value, with a trend line through it. The
line is **flat** — the correlation is 0.045 and it is not statistically
significant. Selling more units per order would not move revenue in this
business. That rules out an obvious strategy, and the flatness is the finding.

*[Hand back.]*

---

# Alber — Close

*[Return to Page 1.]*

So, to bring it together. Growth stopped in 2022. It was driven by a small
number of sub-categories moving against the rest of the business, not by a
general decline. Order count is what drives revenue. And the customer base
splits on margin in a way that revenue reporting completely hides.

Our recommendation from all of this is that the business should track **order
count** rather than revenue, and segment on **margin** rather than revenue.

Thank you — we are happy to take questions.

---

## Questions — prepared answers

The brief requires you to field at least two. Whoever presented the page
answers first; the others should be able to take any of these.

**"Why is order count your main KPI instead of revenue?"**
Because it is what actually drives revenue, and we measured it. Order count
explains about eighty-five percent of the month-to-month variation. Revenue is
the result; order count is the thing the business can act on.

**"How did you decide on three customer segments?"**
We scored two through six using the silhouette measure, which tells you how
well-separated the clusters are. Five actually scored slightly higher than
three — 0.295 against 0.277 — but two of those five segments came out with
almost the same profile, so they were not telling us anything different. Three
gave us segments we could act on.

**"Is the data real?"**
No, and we found that out ourselves and said so. It is synthetic — generated
data. We have five pieces of evidence, including that there is not a single
loss-making sale in five years, and that the transaction amounts are spread
perfectly flat, which is what a random number generator produces. The figures
illustrate the method; every query and model here would run the same way on
real data.

**"What would you do about Printers?"**
That is honestly beyond what this dataset can tell us. It could be a supply
problem, a competitor, or a product category that is simply shrinking. What the
analysis gives us is where to look — one sub-category that lost 136,865 in a
single year, which is over half the entire gap.

**"Why is 2020 only nine months?"**
Our data starts on the 22nd of March 2020. We treated it as a full year at
first, which overstated our growth figure, and we caught it and corrected it.
That is why the year table on Page 1 shows a months-covered column and why
everything is measured per month.

**"Can the dashboard show a single month?"**
Yes — *[use the year slicer, then clear it]*. All three pages have slicers on
year, category and geography, and Page 3 adds the segment slicer.

---

## Rehearsal checklist

- Run it twice with a timer. Ten minutes goes faster than it reads
- Rehearse the slicer demonstration at least three times until the click is
  automatic. That is the moment most likely to go wrong in front of people
- Clear every slicer at the end of each rehearsal, so you never start a run
  with a stale filter
- Each of you can answer a question about someone else's page
- Decide who drives the mouse, and make sure it is not the person talking
- Have the exported PDF open in another window in case Power BI freezes
