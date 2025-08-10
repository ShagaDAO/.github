# ShagaDAO

**One‑page map:** GAP → NGC → DGN

- **GAP** — _Data spec + validator_. Defines **G**ameplay‑**A**ction **P**airs (frames+controls).  
  → Repo: https://github.com/ShagaDAO/gap
- **NGC** — _Research only_. Consumes GAP shards to explore **Neural Game Codecs**; can emit **DGN‑shaped** sample files **offline**.  
  → Repo: https://github.com/ShagaDAO/ngc
- **DGN** — _Protocol spec + validator_. Wire format for **semantic + residual** streaming.  
  → Repo: https://github.com/ShagaDAO/dgn

> **Notes:** Performance numbers are *targets*, not guarantees. $SHAG is **not** live—beware scams. Patent pledge is non‑binding; see repos for details.

## Quick start
1. GAP → validate a sample shard (see `gap` README).
2. NGC → inspect **DGN‑shaped** sample files (`samples/dgn/*`).
3. DGN → run the validator on those samples (see `dgn` README).

## Compatibility
| Producer | Consumer | Status |
|---|---|---|
| GAP v0.2.x shard | NGC notebooks/tools (research) | ✅ supported (toy) |
| NGC DGN‑shaped samples | DGN validator | ✅ passes schemas |
| DGN 0.1.0 schemas | DGN validator | ✅ CI enforced | 