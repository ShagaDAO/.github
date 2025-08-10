# Shaga Principles (2‑minute read)

## 1) Host & Transport ("Zero‑Overhead")
- **Capture** via modern APIs (e.g., Windows Graphics Capture) with microsecond timestamping.
- **Anchor stream**: hardware H.264 tuned for ultra‑low‑latency (no B‑frames, CBR).
- **Control & Delta**: control inputs + compressed residuals (SEI‑carried or side‑channel).
- **Multi‑protocol reality**: WebTransport/QUIC primary; WebRTC fallback; WebSocket as last resort.

## 2) Client ("Thin, Predictive, Stable")
- **Adapted TKN**: keypoints + control‑conditioned temporal predictor.
- **Closed loop**: anchor frames correct drift; delta stream patches the unpredictable.
- **Thermal governor**: mobile‑first PID loop to sustain performance.

## 3) Open Pipelines (GAP → NGC → DGN)
- **GAP**: gameplay data spec + validator.
- **NGC**: research repo; emits **DGN‑shaped** static samples for validator CI.
- **DGN**: wire schemas + CLI validator; cross‑repo CI keeps everything honest.

## 4) Economics ("Cybernetic, not inflationary")
- **Conservative emissions**: baseline targets electricity coverage per node; dilutive risk minimized.
- **Regulator = model of the network**: emissions respond to measurable signals (supply/demand, retention), not tweets.
- **Data as a sink/faucet**: sessions can be subsidized by opt‑in "frames+controls" data; compute cycles can train models when idle.

## 5) Trust & Safety
- **Token**: not live yet. Beware scams.
- **Privacy**: research samples do not require personal content; opt‑in only.
- **Claims**: performance numbers are targets until independently verified. 