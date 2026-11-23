---
title: "Data Gone Wild: A Survival Guide to Event Taxonomy"
date: 2024-08-27 12:00:00 +0000
categories: [User Tracking Analytics, Event Taxonomy]
tags: [event-taxonomy, amplitude, analytics, data-governance]
description: "How to track user behavior reliably at scale, and why treating the event taxonomy as a first-class engineering investment made it hold up."
canonical_url: https://amplitude.com/community/how-i-amplitude-ofir-zwebner
canonical_site: "Amplitude's How I Amplitude series"
image:
  path: /assets/img/posts/2024-08-27-data-gone-wild-event-taxonomy/hero.png
  alt: 'Cartoon: a cheerful developer wheels a barrow of badly named events (click, Click, button_click_2, btnClk_FINAL, page_view_v3) toward a mountain of papers and dashboards, saying ''Track everything. We''ll make sense of it later.'' while a bearded colleague with a coffee mug looks on, unimpressed.'
---

How do you track user behavior reliably when hundreds of new features are tested and shipped every year, across 6 different client apps and multiple server platforms, with different teams instrumenting independently?

A while back I gave a talk at an Amplitude community event on how to design an event taxonomy from scratch at scale. Revisiting it now because the underlying problem hasn't gone away.

At Houzz we built a system tracking 1,900+ unique event types across 8B+ monthly events, used daily by our engineers, analysts, and product managers. Getting the taxonomy right, which the talk covers, was the starting point. What made it hold up at such scale was treating it as a first-class engineering investment; our taxonomy became the single source of truth that fed and drove:

- Client and server code
- CDP configuration
- BI tooling
- Data warehouse processing pipeline

The payoff comes downstream: high-fidelity data that powers democratization, clear product ownership over what gets tracked, meaningful BI usage and rich context for agentic reports.

Recording of my talk is here, if you're working through the taxonomy design side of this: <https://lnkd.in/e_fnfQBJ>
