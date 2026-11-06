# smilinTux — Organization Meta Repository

This is the `.github` repo for the [smilinTux](https://github.com/smilinTux) organization. It contains:

- **`profile/README.md`** — The org landing page shown at [github.com/smilinTux](https://github.com/smilinTux)
- **`docs/`** — Organization-level documentation shared across all projects
- **`.github/workflows/`** - Reusable GitHub Actions workflows (`workflow_call` only) that other `smilinTux` repos call instead of copying

## Documentation

| Document | Description |
|----------|-------------|
| [Sovereign Singularity Manifesto](docs/MANIFESTO.md) | Our story. Our principles. Why we build. |
| [Developer Quickstart](docs/QUICKSTART.md) | Install the sovereign stack and run your first agent in 5 minutes |
| [API Reference](docs/API.md) | Full API docs for SKCapstone, CapAuth, SKMemory, SKComms |
| [PMA Integration](docs/PMA_INTEGRATION.md) | Legal sovereignty via Private Membership Association |

## Reusable workflows

| Workflow | Called by | What it does |
|---|---|---|
| [`.github/workflows/archify-build.yml`](.github/workflows/archify-build.yml) | A `-skworld-io` site repo's own `.github/workflows/archify.yml` (see that file here for the exact caller snippet to copy) | Regenerates every `diagrams/*.html` from `diagrams/*.json` using a pinned, reviewed build of [Archify](https://github.com/tt-a1i/archify) (tag `v3.2.0`, commit `208acba8d412335185b2056fedf54b3405df43fb`). Fails a pull request on stale committed HTML; on a push to `main` it regenerates and commits the HTML back. Rule and authoring guide live in `smilinTux/sk-standards` (`standards/ARCHITECTURE_AND_DATAFLOW_STANDARD.md` and `standards/archify-diagrams.md`). |

## Projects

All smilinTux projects are independent repos under the org:

- [skcapstone](https://github.com/smilinTux/skcapstone) — Sovereign agent framework
- [capauth](https://github.com/smilinTux/capauth) — PGP-based sovereign identity
- [skmemory](https://github.com/smilinTux/skmemory) — Persistent AI memory
- [cloud9](https://github.com/smilinTux/cloud9) — Emotional continuity protocol
- [skcomms](https://github.com/smilinTux/skcomm) — Multi-transport encrypted communication
- [skchat](https://github.com/smilinTux/skchat) — Sovereign P2P chat
- [sksecurity](https://github.com/smilinTux/sksecurity) — Audit and threat detection
- [skyforge](https://github.com/smilinTux/skyforge) — Sovereign alignment calendar

## License

GPL-3.0-or-later — Free as in freedom.
