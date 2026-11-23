---
title: "Data Gone Wild: A Survival Guide to Event Taxonomy"
date: 2026-09-27 12:00:00 +0000
categories: [User Tracking Analytics, Event Taxonomy]
tags: [event-taxonomy, amplitude, analytics, data-governance]
description: "How to track user behavior reliably at scale, and why treating the event taxonomy as a first-class engineering investment made it hold up."
canonical_url: https://amplitude.com/community/how-i-amplitude-ofir-zwebner
canonical_site: "Amplitude's How I Amplitude series"
image:
  path: /assets/img/posts/2026-09-27-data-gone-wild-event-taxonomy/hero.png
  alt: 'Cartoon: a cheerful developer wheels a barrow of badly named events (click, Click, button_click_2, btnClk_FINAL, page_view_v3) toward a mountain of papers and dashboards, saying ''Track everything. We''ll make sense of it later.'' while a bearded colleague with a coffee mug looks on, unimpressed.'
---

For the last 6 years, I have worked with engineers, analysts and product managers on event taxonomy. While it was never stated as such, the notion I had to push back on most often was that we should just "track everything, make sense of it later".

At Houzz, I built a user tracking model that scales. It supports 1,900+ unique event types and 8B+ monthly events, across 6 client apps and multiple server platforms, with different teams instrumenting independently. Engineers, analysts and product managers use it every day.

In this talk, I share the model and the methodology behind it. You will learn to:

- Build your tracking plan around the user's journey, not around the UI.
- Sort every event into one of four types: business outcomes, screens, funnel steps and UI interactions.
- Use a naming convention and a glossary that keep thousands of events readable.
- Ask the one question that decides what to track: "What are the business outcomes?"

What made the model hold up at this scale was treating the taxonomy as a first-class engineering investment. It became the single source of truth that feeds and drives:

- Client and server code
- CDP configuration
- BI tooling
- The data warehouse processing pipeline

The payoff comes downstream: high-fidelity data that powers democratization, clear product ownership over what gets tracked, meaningful BI usage, and rich context for agentic reports. These results are the testament that it works.

**[Watch the talk and read the written walkthrough](https://amplitude.com/community/how-i-amplitude-ofir-zwebner)**, from Amplitude's How I Amplitude series.
