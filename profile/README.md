# ShagaDAO

### Shaga in one page
**Principles**
- **Sovereign > SaaS** — your PC, your keys, your rules. Clients never get raw game assets.
- **Physics‑first** — proximity beats datacenters; latency is a geography problem.
- **Spec‑first** — open specs + validators (GAP, DGN). Research stays in NGC; no stealth claims.
- **Preview‑secure** — ship audits, limits, and negative tests before features.
- **Consent by default** — GAP capture is opt‑in, minimized, and validated; no PII required.
- **Transparency** — targets ≠ guarantees; provenance noted when AI helps.

**What's live today**
- GAP v0.2 spec + validator (preview‑secure)
- DGN 0.1.0 schemas + validator (preview‑secure)
- NGC research docs + DGN‑shaped samples (no runtime)

**Pick your lane**
- 🧑‍💻 **Implementers:** run DGN/GAP validators → open issues
- 🧪 **Researchers:** start with NGC `docs/interop.md` + samples
- 🖥️ **Node ops / creators:** watch for host/client releases on Discord
- 🤝 **Partners:** see `IMPLEMENTATIONS.md` and email contact in repo READMEs

> **Safety notes:** $SHAG is **not live**. Patent pledge is **non‑binding**. Report security issues via GitHub advisories in each repo.

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