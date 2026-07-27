# symworx/.github

> **First public release of SymWorx is pending.** Product code lives in [symworx/symworx](https://github.com/symworx/symworx) (default branch **`develop`**; private until public release).

Special organization repository for **[symworx](https://github.com/symworx)**.

**SymWorx** is a Rust + Python computational stack for **biosignal analysis**, **training load**, **nonlinear dynamics**, and **classical ML**, with an interactive TUI (**`symview`**: BioSym, StatsSym, LoadSym, SpatialSym). Intended license: Apache-2.0.

Public-facing org copy lives in [`profile/README.md`](profile/README.md) (shown on the org Overview). Keep [`docs/`](docs/) aligned with that narrative for the Pages landing site.

## Layout

| Path | Purpose |
|------|---------|
| [`profile/README.md`](profile/README.md) | Organization profile on [github.com/symworx](https://github.com/symworx) |
| [`.github/`](.github/) | Default community health files and issue/PR templates for org repos without their own |
| [`docs/`](docs/) | Static source for the org GitHub Pages site |

### Community defaults (in `.github/`)

- [`CONTRIBUTING.md`](.github/CONTRIBUTING.md) · [`CODE_OF_CONDUCT.md`](.github/CODE_OF_CONDUCT.md)
- [`SECURITY.md`](.github/SECURITY.md) · [`SUPPORT.md`](.github/SUPPORT.md)
- Issue templates · PR template · [`workflows/pages.yml`](.github/workflows/pages.yml)

## Editing product copy

| Surface | Edit |
|---------|------|
| Org Overview | `profile/README.md` |
| Landing site | `docs/` (mirror hero, focus, TUI, crates, release banner) |
| Monorepo deep links | Use branch **`develop`** until public default changes |

This root README is for maintainers of the special repo only — not the product manual.

## GitHub Pages

Deployed from `docs/` via [`.github/workflows/pages.yml`](.github/workflows/pages.yml).

**Cost:** Free for this **public** repository on GitHub Free (soft limits on site size / bandwidth).

**First-time enablement** (required; the workflow fails until this is set):

1. Repo **Settings → Pages → Build and deployment → Source**: **GitHub Actions**
2. Re-run **Deploy GitHub Pages** (Actions tab) or push a change under `docs/`
3. Site URL: [https://symworx.github.io/.github/](https://symworx.github.io/.github/)

Optional: custom domain under **Settings → Pages**.

### Local preview

```bash
python -m http.server 8080 --directory docs
# open http://localhost:8080
```

## What belongs here

- Org-wide community defaults and templates  
- Org profile README  
- Lightweight marketing / landing Pages  

What does **not** belong here:

- Product source code ([symworx/symworx](https://github.com/symworx/symworx))  
- Per-repo licenses (must live in the product repository)  
