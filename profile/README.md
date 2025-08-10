# ShagaDAO

**One‑page map:** GAP → NGC → DGN

- **GAP** — _Data spec + validator_. Defines **G**ameplay‑**A**ction **P**airs (frames+controls).  
  → Repo: https://github.com/ShagaDAO/gap
- **NGC** — _Research only_. Consumes GAP shards to explore **Neural Game Codecs**; can emit **DGN‑shaped** sample files **offline**.  
  → Repo: https://github.com/ShagaDAO/ngc
- **DGN** — _Protocol spec + validator_. Wire format for **semantic + residual** streaming.  
  → https://github.com/ShagaDAO/dgn

---

## Core principles
- **Physics‑first, thermodynamically honest.** Designs and token policy are grounded in power, bandwidth, and latency budgets—not vibes.  
- **Zero‑overhead host, thin client.** The PC captures/encodes with near‑zero perf hit; phones run light models for efficiency.  
- **Dual‑Stream architecture.** Anchor video + control/delta stream (causal + residual) for stability and fidelity under real networks.  
- **Open pipes, verifiable flow.** GAP (data) → NGC (research) → DGN (protocol) with validators and CI across repos.  
- **Conservative emissions.** Token emissions target electricity coverage first; growth is earned by usage/retention—not printing.

---

## Quick start
- **Validate data (GAP):**
  ```bash
  python3 tools/validate.py samples/
  ```
- **Inspect DGN‑shaped samples (NGC):** `ngc/samples/dgn/*`
- **Run the DGN validator:** see `dgn` README for schema checks on NGC samples.

## Compatibility
| Producer | Consumer | Status |
|---|---|---|
| GAP v0.2.x shard | NGC notebooks/tools (research) | ✅ supported (toy) |
| NGC DGN‑shaped samples | DGN validator | ✅ passes schemas |
| DGN 0.1.0 schemas | DGN validator | ✅ CI enforced |

---

## Status & safety

- **Alpha software.** Expect breaking changes.
- **Token not live.** If you see a $SHAG token today, it's a scam. Do not buy it.
- **Data ethics.** "Frames+controls" capture is opt‑in; no personal content needed for research samples. 