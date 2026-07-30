# SymWorx

> **First public release pending.** The monorepo and APIs are under active development; packaging, docs, and stability guarantees for a public release are not final yet. The product repository will open with the first public release — follow [github.com/symworx](https://github.com/symworx) for updates.

### Isolated environments for modeling, analysis & simulation

**SymWorx** is a modular computational stack for **biosignal analysis**, **training load**, **nonlinear dynamics**, and **classical ML** — with a **Rust kernel**, **Python bindings**, and a keyboard-driven terminal UI (**`symview`**).

It targets research, education, and portable inference (workstation today; embedded / mobile / web recipes for exported models), with the same methods available from notebooks to constrained devices.

Open development lives in a single [monorepo](https://github.com/symworx/symworx)


## Focus

We put dynamical systems methods, signal processing, and classical ML into one inspectable stack you can run in research workflows and on constrained hardware. 

### Physiological & biomechanical analysis and simulation

Process and model biosignals and movement with quality-aware features and physiologically meaningful metrics:

- Wearable and lab modalities such as **PPG**, respiration, and related time series
- **Gait** and biomechanical responses (including run / performance work inside biosym)
- **Central pattern generators (CPG)** that couple physiological and biomechanical signals
- Training **load, recovery, and multi-source** performance time series (ACWR/TSS-style metrics, FIT ingestion, nutrition modeling, `symload` CLI)
- Sport-agnostic **spatial / trajectory** analysis for how agents use space over time

### Nonlinear dynamics & complexity

Expose temporal structure that linear summaries often miss:

- **Recurrence quantification** (RQA / CRQA), recurrence plots, and related pipelines 
- **Entropy and complexity** measures 
- Embedding, DMD, SINDy / SINDYc, Koopman/EDMD, and related dynamical tools
- Signal processing foundations — filters, peaks, sparse sensing, Kalman family, interpolation, resampling

### Classical ML & statistics

Classical, interpretable ML and stats in **`symworx-stats`** (many APIs pure Rust; advanced LA behind optional `linalg` / OpenBLAS):

- Preprocessing (scalers), train/test splits and folds
- **Logistic regression** (binary + multiclass OVR), Gaussian **Naive Bayes**, **k-NN**, rule lists / stumps
- **k-means** clustering; classification metrics including **ROC/AUC**
- OLS / Ridge / Lasso / Elastic Net, LDA, PCA/SVD, polynomial regression (with `linalg` where needed)
- **Model export** for predict-only use on C/MCU, iOS, Android, and web

### Embedded systems & portable computation

A portable computational engine intended to:

- Run analysis and simulation on desktop and cloud, with a path toward **microcontrollers and bare-metal**
- Support **host-side embedded streaming** (e.g. PPG protocols, serial and simulator sources)
- Integrate cleanly with **Python** for education, data science, and rapid prototyping
- Prefer **secure, explicit, testable** implementations suitable for high-assurance stacks

### Terminal UI — *symview* (`symworx-tui`)

The **TUI** is the interactive front end for day-to-day work. From **Home**, workflows include:

| Key | Workflow | What it covers |
|-----|----------|----------------|
| **1** | **BioSym** | Import · Explore · Dynamics (RQA) · Generate demo signals |
| **2** | **StatsSym** | Import · **Lab** (classical ML / stats tasks) · Generate teaching presets |
| **3** | **LoadSym** | Workout analysis, calendar trends, load recommendations |
| **4** | **SpatialSym** | Trajectory / space metrics and decision views |

Also: keyboard-driven navigation, file conversion via `symworx-io`, sparkline/stats explore views.

When the monorepo is available locally:

```bash
cargo run -p symworx-tui --bin symview
```

## Philosophy

| | |
|---|---|
| **Security** | Minimize unsafe code, reduce unintended execution paths, and lower supply-chain risk |
| **Robustness** | Predictable behavior, strong typing, and explicit error handling across the stack |
| **Scalability** | One kernel for analysis, simulation, classical ML, and portable inference |

Much of the original work began in Python; the long-term engine is **Rust**, with Python for teaching and rapid prototyping. Intended license: **Apache-2.0**.

## Crates

Domain and foundation crates inside [symworx/symworx](https://github.com/symworx/symworx) (paths on default branch **`develop`**):

| Crate | Focus |
|-------|--------|
| [`symworx-tui`](https://github.com/symworx/symworx/tree/develop/crates/symworx-tui) | **TUI** (*symview*) — BioSym, **StatsSym** (ML lab), LoadSym, SpatialSym |
| [`symworx-core`](https://github.com/symworx/symworx/tree/develop/crates/symworx-core) | Core re-exports and shared utilities |
| [`symworx-stats`](https://github.com/symworx/symworx/tree/develop/crates/symworx-stats) | Statistics + **classical ML** (logistic, NB, k-NN, rules, k-means, PCA, …) |
| [`symworx-biosym`](https://github.com/symworx/symworx/tree/develop/crates/symworx-biosym) | Physiological signals (PPG, respiration), gait, CPG |
| [`symworx-loadsym`](https://github.com/symworx/symworx/tree/develop/crates/symworx-loadsym) | Training load, FIT, nutrition, `symload` CLI |
| [`symworx-spatialsym`](https://github.com/symworx/symworx/tree/develop/crates/symworx-spatialsym) | 2D trajectory analysis and spatial decision modeling |
| [`symworx-dynamics`](https://github.com/symworx/symworx/tree/develop/crates/symworx-dynamics) | Nonlinear dynamics — RQA, embedding, entropy, DMD, SINDy |
| [`symworx-signal`](https://github.com/symworx/symworx/tree/develop/crates/symworx-signal) | Filters, peaks, sparse sensing, Kalman family |
| [`symworx-io`](https://github.com/symworx/symworx/tree/develop/crates/symworx-io) | Canonical I/O for biosignals and activity data |
| [`symworx-embed`](https://github.com/symworx/symworx/tree/develop/crates/symworx-embed) | Host-side embedded streaming (PPG protocol, serial / sim) |

Also: [`symworx-loadsym-db`](https://github.com/symworx/symworx/tree/develop/crates/symworx-loadsym-db), [`symworx-math`](https://github.com/symworx/symworx/tree/develop/crates/symworx-math), [`symworx-backend`](https://github.com/symworx/symworx/tree/develop/crates/symworx-backend), [`symworx-error`](https://github.com/symworx/symworx/tree/develop/crates/symworx-error), and [Python bindings](https://github.com/symworx/symworx/tree/develop/bindings/python).

## Contributors

- [ntberry](https://github.com/ntberry)
- [PalEm Dynamics](https://www.PalEmDynamics.com)
- [cSYMd](https://www.cSYMd.com)

## Get involved

- **Code:** [symworx/symworx](https://github.com/symworx/symworx) (opens with public release)
- **Contributing:** [CONTRIBUTING.md](https://github.com/symworx/.github/blob/main/.github/CONTRIBUTING.md)
- **Security:** [SECURITY.md](https://github.com/symworx/.github/blob/main/.github/SECURITY.md)
- **Site:** [symworx.github.io/.github](https://symworx.github.io/.github/) (available after public release)
