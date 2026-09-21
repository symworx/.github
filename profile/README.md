# SymWorx

Open computational tools for **biosignal analysis**, **teaching**, and the supporting toolchain.

Public repositories are [Apache-2.0](https://github.com/symworx/symworx/blob/HEAD/LICENSE). The analysis kernel is in beta; sibling tools have their own release lines.

Default branch for the software listed below is **`worx`** (GitHub Flow; tags on `worx`). Until the GitHub rename lands, clones still check out **`develop`**.

## Software

| Repository | What it is |
|------------|------------|
| [symworx](https://github.com/symworx/symworx) | Analysis stack: biosignals, training load, nonlinear dynamics, classical ML. Rust kernel, Python bindings, keyboard-driven TUI (`symview`). **Public.** |
| [symkit](https://github.com/symworx/symkit) | Installer for agent harnesses (teaching, research, engineering, and related roles). Shared policies for Grok, Claude Code, Codex, and similar tools. **Public.** |
| [symcourse](https://github.com/symworx/symcourse) | Scaffold a course repository: layout, runtime, and identity. Agent packs come from [symkit](https://github.com/symworx/symkit). **Private.** |
| [symelib](https://github.com/symworx/symelib) | Local paper library (`elib`): PDF ingest, PubMed / Crossref metadata, search, and a TUI. **Public.** |
| [symsight](https://github.com/symworx/symsight) | Insight generator for articles and social posts. Rust core, CLI, Textual TUI, YAML brand files. **Public.** |
| [symjump](https://github.com/symworx/symjump) | Terminal favorites and actions (`sjmp`): pinned places, toolbox / agent actions, bash hook. **Private.** |

The org site ([symworx-web](https://github.com/symworx/symworx-web), private) is not a product crate. Research manuscripts stay out of this org.

## Analysis stack ([symworx/symworx](https://github.com/symworx/symworx))

Modular stack for **biosignal analysis**, **training load**, **nonlinear dynamics**, and **classical stats / ML** — same methods from notebooks to constrained devices.

From a local clone:

```bash
cargo run -p symworx-tui --bin symview
```

**`symview` Home:** `1` BioSym · `2` StatsSym · `3` LoadSym · `4` SpatialSym.

| Crate | Focus |
|-------|--------|
| [`symworx-tui`](https://github.com/symworx/symworx/tree/HEAD/crates/symworx-tui) | TUI (`symview`) |
| [`symworx-biosym`](https://github.com/symworx/symworx/tree/HEAD/crates/symworx-biosym) | PPG, respiration, gait, CPG |
| [`symworx-loadsym`](https://github.com/symworx/symworx/tree/HEAD/crates/symworx-loadsym) | Training load, FIT, nutrition, `symload` |
| [`symworx-spatialsym`](https://github.com/symworx/symworx/tree/HEAD/crates/symworx-spatialsym) | 2D trajectories and spatial decisions |
| [`symworx-dynamics`](https://github.com/symworx/symworx/tree/HEAD/crates/symworx-dynamics) | RQA, embedding, entropy, DMD, SINDy |
| [`symworx-signal`](https://github.com/symworx/symworx/tree/HEAD/crates/symworx-signal) | Filters, peaks, sparse sensing, Kalman family |
| [`symworx-stats`](https://github.com/symworx/symworx/tree/HEAD/crates/symworx-stats) | Statistics and classical ML |
| [`symworx-io`](https://github.com/symworx/symworx/tree/HEAD/crates/symworx-io) | Canonical signal / activity I/O |
| [`symworx-embed`](https://github.com/symworx/symworx/tree/HEAD/crates/symworx-embed) | Host-side PPG streaming / simulator |
| [`symworx-dbsym`](https://github.com/symworx/symworx/tree/HEAD/crates/symworx-dbsym) | Per-study / edge catalog |

Also: [`symworx-core`](https://github.com/symworx/symworx/tree/HEAD/crates/symworx-core), [`symworx-math`](https://github.com/symworx/symworx/tree/HEAD/crates/symworx-math), [`symworx-loadsym-db`](https://github.com/symworx/symworx/tree/HEAD/crates/symworx-loadsym-db), [`symworx-backend`](https://github.com/symworx/symworx/tree/HEAD/crates/symworx-backend), [`symworx-error`](https://github.com/symworx/symworx/tree/HEAD/crates/symworx-error), and [Python bindings](https://github.com/symworx/symworx/tree/HEAD/bindings/python).

## Philosophy

| | |
|---|---|
| **Security** | Minimize unsafe code, reduce unintended execution paths, and lower supply-chain risk |
| **Robustness** | Predictable behavior, strong typing, and explicit error handling |
| **Scalability** | One kernel for analysis, simulation, classical ML, and portable inference |

The long-term engine is **Rust**, with Python for teaching and rapid prototyping.

## Contributors

- [ntberry](https://github.com/ntberry) (Nathaniel T. Berry)
- [cSYMd](https://www.cSYMd.com)

## Get involved

- **Org:** [github.com/symworx](https://github.com/symworx)
- **Contributing:** [CONTRIBUTING.md](https://github.com/symworx/.github/blob/main/.github/CONTRIBUTING.md)
- **Security:** [SECURITY.md](https://github.com/symworx/.github/blob/main/.github/SECURITY.md)
