# trade-performance-analytics

This repository is a curated, public-facing overview of a larger private system built to analyze trading performance, execution quality, and behavioral patterns using locally owned data.

The full application (code, database, and ingestion pipelines) remains private by design. This repo exists to document *what* was built, *why* it was built, and *how* the system thinks — not to provide a runnable demo.

---

## Why This Exists

After stepping away from traditional infrastructure roles, I spent time actively trading equities and quickly found that most tools focus on **PnL**, not **process**.

This project was built to answer different questions:

- Am I executing my plan, or breaking it?
- Where do losses actually come from — setup quality, stops, timing, or behavior?
- What patterns repeat when I’m disciplined vs impulsive?
- How do I hold myself accountable using *my own data*, not a broker’s dashboard?

The result is a local-first analytics platform that treats trading as a **feedback system**, not a scoreboard.

---

## What’s Included Here

This repo documents the core components of the system through screenshots and written walkthroughs:

- **Dashboard** – A post-trade execution snapshot focused on behavior, not profit
- **Performance** – Deeper analysis by symbol, time-of-day, duration, and stop behavior
- **Behavior / Coaching** – Rule-based diagnostics that call out execution failures using real trades
- **Admin** – The ingestion and data engine that powers everything else

Each section is documented in its own markdown file:

- [`Dashboard.md`](./Dashboard.md)
- [`Performance.md`](./Performance.md)
- [`Behavior.md`](./Behavior.md)
- [`Admin.md`](./Admin.md)

---

## Design Principles

- **Local-first**: Trades and analytics live on my machine, not in a third-party cloud
- **Rebuildable**: Trades can be re-derived when logic changes without re-importing raw data
- **Opinionated**: The system is designed to call out mistakes, not validate feelings
- **Execution over outcome**: Behavior and discipline matter more than short-term PnL

---

## What This Is *Not*

- A trading bot
- A signal generator
- A SaaS product
- An attempt to sell a strategy

This is a personal system built to improve decision-making through data, iteration, and accountability.

---

## Notes

All screenshots use real or synthetic trade data. Sensitive logic, broker integrations, and full source code are intentionally omitted.