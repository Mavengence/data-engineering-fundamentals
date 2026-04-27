# Data Engineering Fundamentals

> An interactive crash course on building production data pipelines — 10 chapters, 15 live simulators, no signup required, runs entirely in your browser.

**Live demo:** _coming soon_

## What's inside

- **10 chapters** — Ingest → Streaming → Store → Compute → Orchestrate → Quality → Discover → Serve → Govern → Capstone
- **15 simulators** — drag the watermark, shuffle a hash join, break a DQ gate, run the capstone pipeline end-to-end
- **Guided tutorial** — automated walkthrough that breaks each pipeline contract and shows exactly what fails downstream
- **No signup, no build step, no framework** — open `index.html` and go

## Run locally

```bash
git clone https://github.com/Mavengence/de-fundamentals.git
cd de-fundamentals
python3 .serve.py        # serves at http://127.0.0.1:5002
```

Then open [http://127.0.0.1:5002](http://127.0.0.1:5002) in your browser.

## Tech

Vanilla React 18 via CDN + Babel standalone + plain CSS — no build step, no bundler. Everything in `src/v6/` and `v6-styles.css`.

## License

MIT — see [LICENSE](LICENSE).
