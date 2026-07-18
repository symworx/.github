# SymWorx

### Isolated environments for modeling & simulation

**SymWorx** is a multi-use computational framework with a **Rust kernel** and **Python bindings** — built for security, robustness, and portability from microcontrollers to the cloud.

Open development lives in a single monorepo:

**→ [github.com/symworx/symworx](https://github.com/symworx/symworx)**

## Philosophy

| | |
|---|---|
| **Security** | Minimize unsafe code, reduce unintended execution paths, and lower supply-chain risk |
| **Robustness** | Predictable behavior, strong typing, and explicit error handling across the stack |
| **Scalability** | Consistent APIs for embedded, desktop, scientific, and educational workloads |

## Crates

Domain and foundation crates inside [symworx/symworx](https://github.com/symworx/symworx):

| Crate | Focus |
|-------|--------|
| [`symworx-biosym`](https://github.com/symworx/symworx/tree/main/crates/symworx-biosym) | Physiological signals (PPG, respiration), gait analysis, and central pattern generators |
| [`symworx-loadsym`](https://github.com/symworx/symworx/tree/main/crates/symworx-loadsym) | Training load, periodization, ACWR/TSS, monotony/strain, and nutrition modeling |
| [`symworx-spatialsym`](https://github.com/symworx/symworx/tree/main/crates/symworx-spatialsym) | Sport-agnostic 2D trajectory analysis and post-hoc spatial decision modeling |
| [`symworx-dynamics`](https://github.com/symworx/symworx/tree/main/crates/symworx-dynamics) | Nonlinear dynamics — RQA, embedding, entropy, DMD, Koopman/EDMD, LTI control |
| [`symworx-signal`](https://github.com/symworx/symworx/tree/main/crates/symworx-signal) | Filters, peaks, sparse sensing, interpolation, and resampling |
| [`symworx-core`](https://github.com/symworx/symworx/tree/main/crates/symworx-core) | Core re-exports and shared utilities across the simulation crates |
| [`symworx-tui`](https://github.com/symworx/symworx/tree/main/crates/symworx-tui) | Terminal UI (*symview*) for biosignal exploration, dynamics, and load analysis |
| [`symworx-io`](https://github.com/symworx/symworx/tree/main/crates/symworx-io) | Canonical I/O for biosignals and activity data (CSV, Parquet, FIT, email) |

Also in the monorepo: [`symworx-loadsym-db`](https://github.com/symworx/symworx/tree/main/crates/symworx-loadsym-db), [`symworx-stats`](https://github.com/symworx/symworx/tree/main/crates/symworx-stats), [`symworx-math`](https://github.com/symworx/symworx/tree/main/crates/symworx-math), [`symworx-embed`](https://github.com/symworx/symworx/tree/main/crates/symworx-embed), [`symworx-backend`](https://github.com/symworx/symworx/tree/main/crates/symworx-backend), [`symworx-error`](https://github.com/symworx/symworx/tree/main/crates/symworx-error), and [Python bindings](https://github.com/symworx/symworx/tree/main/bindings/python).

## Contributors

- [PalEm Dynamics](https://www.PalEmDynamics.com) — [www.PalEmDynamics.com](https://www.PalEmDynamics.com)
- [cSYMd](https://www.cSYMd.com) — [www.cSYMd.com](https://www.cSYMd.com)

## Get involved

- **Code:** [symworx/symworx](https://github.com/symworx/symworx)
- **Contributing:** [CONTRIBUTING.md](https://github.com/symworx/.github/blob/main/.github/CONTRIBUTING.md)
- **Security:** [SECURITY.md](https://github.com/symworx/.github/blob/main/.github/SECURITY.md)
- **Site:** [symworx.github.io/.github](https://symworx.github.io/.github/)
