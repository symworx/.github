# SymWorx

> **First public release pending.** The monorepo and APIs are under active development; packaging, docs, and stability guarantees for a public release are not final yet. Watch [symworx/symworx](https://github.com/symworx/symworx) for updates.

### Isolated environments for modeling, analysis & simulation

**SymWorx** is a modular open-source computational framework with a **Rust kernel** and **Python bindings**. It provides an isolated, high-assurance environment for mathematical signal processing, nonlinear dynamics, and simulation — consistent from research notebooks to edge devices.

Interactive exploration is first-class via the **terminal UI (TUI)** — **`symview`** (`symworx-tui`) — for selecting, converting, and visualizing biosignals, running nonlinear-dynamics workflows (e.g. RQA), and analyzing training load without leaving the terminal.

The platform is designed for broad use across **scientific computing**, **embedded systems**, **performance and health informatics**, and education, with the same APIs and methods available wherever the stack runs.

Open development lives in a single monorepo:

**→ [github.com/symworx/symworx](https://github.com/symworx/symworx)**

## Focus

SymWorx turns dynamical systems theory and rigorous signal methods into **usable computational pipelines** — tools you can inspect, extend, and run under real constraints of noise, latency, and power.

### Physiological & biomechanical analysis and simulation

Process and model biosignals and movement with quality-aware features and physiologically meaningful metrics. Domain crates cover:

- Wearable and lab modalities such as **PPG**, respiration, and related time series  
- **Gait** and biomechanical responses, including work toward integrated running / performance simulation  
- **Central pattern generators (CPG)** that couple physiological and biomechanical signals  
- Training **load, recovery, and multi-source** performance time series (ACWR/TSS-style metrics, FIT ingestion, nutrition modeling)  
- Sport-agnostic **spatial / trajectory** analysis for how agents use space over time  

### Nonlinear dynamics & complexity

Expose temporal structure that linear summaries often miss:

- **Recurrence quantification** (RQA / CRQA), recurrence plots, and related pipelines  
- **Entropy and complexity** measures  
- Embedding, DMD, Koopman/EDMD, and related dynamical tools  
- Signal processing foundations — filters, peaks, sparse sensing, interpolation, resampling  

### Embedded systems & portable computation

A portable computational engine intended to:

- Run on **microcontrollers and bare-metal** as well as desktop and cloud  
- Support **host-side embedded streaming** (e.g. PPG protocols, serial and simulator sources)  
- Integrate cleanly with **Python** for education, data science, and rapid prototyping  
- Prefer **secure, explicit, testable** implementations suitable for high-assurance stacks  

### Terminal UI (*symview*)

The **TUI** (`symworx-tui`, binary **`symview`**) is the interactive front end for day-to-day work in the monorepo:

- Load and convert physiological / biosym signals (CSV, Parquet, IBI, and related formats via `symworx-io`)  
- Explore and visualize signals in the terminal  
- Run **dynamics** workflows (including RQA parameter exploration)  
- First-class **LoadSym** workflows for workout analysis, calendar trends, and load-related recommendations  

```bash
cargo run -p symworx-tui --bin symview
```

## Philosophy

| | |
|---|---|
| **Security** | Minimize unsafe code, reduce unintended execution paths, and lower supply-chain risk |
| **Robustness** | Predictable behavior, strong typing, and explicit error handling across the stack |
| **Scalability** | Consistent APIs for embedded, desktop, scientific, and educational workloads |

Much of the original work began in Python and is being rewritten in Rust to deepen assurance and portability while keeping research-friendly bindings.

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
| [`symworx-tui`](https://github.com/symworx/symworx/tree/main/crates/symworx-tui) | **TUI** (*symview*) — interactive terminal UI for biosignals, dynamics (RQA), and LoadSym analysis |
| [`symworx-io`](https://github.com/symworx/symworx/tree/main/crates/symworx-io) | Canonical I/O for biosignals and activity data (CSV, Parquet, FIT, email) |
| [`symworx-embed`](https://github.com/symworx/symworx/tree/main/crates/symworx-embed) | Host-side embedded streaming — PPG sample protocol, serial / simulator sources |

Also in the monorepo: [`symworx-loadsym-db`](https://github.com/symworx/symworx/tree/main/crates/symworx-loadsym-db), [`symworx-stats`](https://github.com/symworx/symworx/tree/main/crates/symworx-stats), [`symworx-math`](https://github.com/symworx/symworx/tree/main/crates/symworx-math), [`symworx-backend`](https://github.com/symworx/symworx/tree/main/crates/symworx-backend), [`symworx-error`](https://github.com/symworx/symworx/tree/main/crates/symworx-error), and [Python bindings](https://github.com/symworx/symworx/tree/main/bindings/python).

## Contributors

- [ntberry](https://github.com/ntberry)
- [PalEm Dynamics](https://www.PalEmDynamics.com)
- [cSYMd](https://www.cSYMd.com)

## Get involved

- **Code:** [symworx/symworx](https://github.com/symworx/symworx)
- **Contributing:** [CONTRIBUTING.md](https://github.com/symworx/.github/blob/main/.github/CONTRIBUTING.md)
- **Security:** [SECURITY.md](https://github.com/symworx/.github/blob/main/.github/SECURITY.md)
- **Site:** [symworx.github.io/.github](https://symworx.github.io/.github/)
