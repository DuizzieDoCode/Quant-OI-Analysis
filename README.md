##  Index Options OI Engine – Quant-OI-Analysis

### What I’ve built

- **Index options open‑interest engine** that tracks how call and put OI evolve around the at‑the‑money strikes for the nearest expiry.
- Generates a **clean time series** of:
  - Total CALL OI, total PUT OI,
  - PUT–CALL OI differential,
  - A simple **regime signal**: bullish / bearish / sideways.
- Persists these signals in **PostgreSQL** and projects them onto a dashboard for **live monitoring** alongside price.

### How it’s useful to a quant / systematic desk

- Acts as a **market‑regime and positioning indicator** for NIFTY BANKNIFTY SENSEX, building up across the options strip rather than just price.
- Provides a **complementary signal layer** for systematic strategies:
  - Filter entries/exits by OI regime.
  - Adjust risk or leverage when OI imbalances become extreme.
  - Detect crowding and potential squeeze/crash conditions in index options.
- All of this is built as a **repeatable, data‑driven process** suitable for research, backtesting and production use.

### Why this showcases me as a systematic trader

- I work from **market structure first** (who is taking risk, where is OI concentrating) and then turn that into **quantifiable signals**.
- I’m comfortable with the **full pipeline**:
  - Broker APIs and live derivatives data (Finvasia, futures and options).
  - Python signal‑generation code and OI aggregation logic.
  - SQL / PostgreSQL storage for research‑grade time series.
- I use this OI engine not as a toy, but as a **live risk and confirmation tool** that sits next to my systematic strategies and helps me understand when the market regime supports or contradicts my models.

