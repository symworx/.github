# Welcome to the _SymWorx_ Project

**SymWorx** began as a focused effort to develop a modular computational stack for biosignal analysis as well as training load & training periodization, while incorporating methods from nonlinear dynamics and machine learning — capable of being deployed on bare metal, mobile, and web applications. To achieve this, these tools were written in **Rust** and coupled with **Python** bindings.

Since beginning this work, the _product_ offering has expanded and we are working on other tools and resources that would/could accompany the scientist, engineer, or product manager in their efforts. Examples include (1) tools and resources to manage research/scientific articles and (2) resources to generate text-based insights for blog articles or social media campaigns.

The core [scientific repo](https://github.com/symworx/symworx) and [insights generation tools](https://github.com/symworx/symworx-insights) are **pending public release**.

The [electronic library](https://github.com/symworx/symworx-elibrary) tools are available under a beta release.

## Repositories
| Project                                                                     |  Visibility               | Description                                                       |
|:----------------------------------------------------------------------------|:-------------------------|:------------------------------------------------------------------|
| [**symworx**](https://github.com/symworx/symworx)                   | *Pending public release* | Core monorepo: Rust + Python stack, crates, and **`symview`** TUI |
| [**symworx-elibrary**](https://github.com/symworx/symworx-elibrary) | ***Public (beta)***      | Local paper (PDF) library: metadata, search, lists, TUI (`elib`)  |
| [**symworx-insights**](https://github.com/symworx/symworx-insights) | *Pending public release* | Text-based insights for blogs, social, and related communication  |

---

### [SymWorx](https://github.com/symworx/symworx)

An inspectable **Rust** kernel with **Python** bindings for people who need the same scientific methods on a workstation today and a path toward constrained hardware tomorrow — biosignals, training load, nonlinear dynamics, and classical ML in one stack, with a keyboard-driven terminal UI (**`symview`**) for local testing, development, and analysis. 

**Focus:** physiological & biomechanical analysis · nonlinear dynamics & complexity · classical ML & stats · embedded & portable computation

Much of the original work began in Python but has since transitioned to **Rust** as the long-term engine with Python bindings for teaching and rapid prototyping. The stack is built to stay explicit and testable — from host-side streaming and research workflows toward microcontrollers, mobile, and web recipes for exported models — without bolting together a new toolchain for each study.

Install, crate map, and `symview` workflows will live in the monorepo when it opens.

**Status:** pending public release

    
### [SymWorx-elibrary](https://github.com/symworx/symworx-elibrary)

A local digital library for research PDFs: ingest, enrich metadata (PubMed → Crossref → local fallback), full-text search, reading lists, and an optional agents/RAG path on your own corpus. Day-to-day work runs through the **`elib`** CLI and TUI.

Quickstart, install, and library layout live in the product repo.

**Status:** **public beta**


### [SymWorx-insights](https://github.com/symworx/symworx-insights)

Tools and workflows for turning notes, analyses, and research artifacts into draft **blog** and **social** copy — inspectable, human-editable narrative that sits alongside the scientific stack and literature library rather than replacing either.

**Status:** pending public release

---

## Philosophy

- **Security**    : Minimize unsafe code, reduce unintended execution paths, and lower supply-chain risk
- **Robustness**  : Predictable behavior, strong typing, and explicit error handling across the stack
- **Scalability** : One scientific kernel for analysis, simulation, classical ML, and portable inference — with companion tools for literature and communication


## Contributors
| [ntberry](https://github.com/ntberry) | [PalEm Dynamics](https://www.PalEmDynamics.com) | [cSYMd](https://www.cSYMd.com) |

## Get involved

 [Contributing](https://github.com/symworx/.github/blob/main/.github/CONTRIBUTING.md) | [Security](https://github.com/symworx/.github/blob/main/.github/SECURITY.md) | [Site](https://symworx.github.io/.github/)
