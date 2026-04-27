# Data Engineering Fundamentals

> Think like a data engineer by lunch.

**10 chapters · 15 live simulators · no signup · no build step · runs in your browser**

[**→ Open the live demo**](https://www.timloehr.me/de-fundamentals/) &nbsp;·&nbsp;
[**⭐ Star on GitHub**](https://github.com/Mavengence/de-fundamentals)

<!-- 
  ADD A GIF HERE before the public launch.
  Record 30s: Overview pipeline hover → drag the watermark → flip Scanner to columnar → break a Capstone gate.
  Tools: Cleanshot X, QuickTime + gifski, or Loom.
  Target: <5 MB, 800px wide, 15fps.
-->

---

## What you'll learn

The system, not the tools. By the end you know *where* a pipeline fails before it does.

| # | Chapter | The lesson |
|---|---------|-----------|
| 00 | Core Fundamentals | Why columnar skips 99% of disk. What Parquet actually is. |
| 01 | Ingest | Two clocks per event. The one that's wrong decides what you lose. |
| 02 | Streaming | Fast loses on completeness; slow loses on latency. Pick one. |
| 03 | Store | One bad day on Day 3 poisons every day that follows it. |
| 04 | Compute | The planner bets on statistics. Wrong stats, wrong plan. |
| 05 | Orchestrate | A task that ran twice must equal a task that ran once. Non-negotiable. |
| 06 | Quality | A bad row is worse than a missing row — the bad one ships. |
| 07 | Discover | Six commands. The answer in under 3 seconds. Always. |
| 08 | Serve | Five teams. Five DAU numbers. One meeting. |
| 09 | Govern | An unannotated PII column never ships. |
| 10 | Capstone | Break any one of six contracts. Watch exactly what fails. |

---

## The simulators

15 live simulators — every concept is interactive, not described:

- **Column scanner** — flip row ↔ columnar; 99 columns dim to near-invisible, one glows blue
- **Watermark drag** — drag the event-time window; watch late events drop in real time
- **Hash-join shuffle** — push skew to 90%; worker 0 overflows while the others idle
- **7-layer stack** — hover any infrastructure layer; trace a query from SQL to disk and back
- **Byte trace** — follow one byte: cold Metastore lookup (80ms) vs warm cache (0.04ms)
- **Idempotent backfill** — flip `INSERT OVERWRITE` → `INSERT`; retry doubles every row
- **Cumulative table** — scrub 5 days; Day 3 has a bug; watch drift compound forward
- **Trust meter** — disable row-count checks; watch bad data reach the exec dashboard
- **Discovery speedrun** — 5 timed questions; find the table owner in under 3 seconds
- **Lineage camera** — click any node; upstream/downstream highlights with animated flow
- **Metrics query** — governed vs ungoverned; same question, same warehouse, different answer
- **Permission gate** — drag actor chips onto PII columns; Access Gateway blocks bad deploys
- **Capstone pipeline** — six gates, six sabotage buttons; rows burst at broken contracts

---

## Run it in 30 seconds

No npm. No build step. No account.

```bash
git clone https://github.com/Mavengence/de-fundamentals.git
cd de-fundamentals
python3 .serve.py          # → http://127.0.0.1:5002
```

Or just open `index.html` directly in Chrome — it works without a server.

---

## Why this exists

I built this material for a production data team's onboarding program.
After running it internally, I sanitized and open-sourced it because every
DE resource I've used was either a 9-week bootcamp or a list of Medium posts.
Neither teaches you *why* the pipeline breaks. This one does.

The course treats every concept as a failure mode: watermarks exist because
you can't tell what you dropped, idempotency exists because retries are
inevitable, governance exists at write-time because read-time is too late.

---

## Tech

Vanilla React 18 via CDN · Babel standalone · plain CSS · no bundler · no `npm install`.

Everything lives in `src/chapters/` (JSX per chapter) and `styles.css`.
Fork it, clone it, teach with it.

---

## Contributing

Found a bug? Wrong number in a sim? Open an issue or a PR.
The chapter files are self-contained — each one is a single JSX file you can
read top to bottom in 10 minutes.

---

## License

MIT — see [LICENSE](LICENSE).
