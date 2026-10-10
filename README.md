# homebrew-kwd

Homebrew tap for [kwd](https://github.com/hrodrig/kwd) — Kubernetes workload readiness watchdog (single-pass or daemon, Slack notify, HTTP `/healthz` + `/metrics`).

Same pattern as **[homebrew-kzero](https://github.com/hrodrig/homebrew-kzero)** / **[homebrew-pgwd](https://github.com/hrodrig/homebrew-pgwd)**: **`Casks/kwd.rb`** is generated and pushed by **GoReleaser** on each [kwd release tag](https://github.com/hrodrig/kwd/releases) (`HOMEBREW_TAP_TOKEN` on the **kwd** repo).

## Install

```bash
brew install hrodrig/kwd/kwd
```

Works on **macOS** and **Linux** (Homebrew on Linux). Installs the **`kwd`** and **`kubectl-kwd`** binaries plus man pages from the release tarball.

## Links

- **Project:** [github.com/hrodrig/kwd](https://github.com/hrodrig/kwd)
- **Operator docs:** [kwd-selfhosted](https://github.com/hrodrig/kwd-selfhosted)
- **Releases:** [kwd releases](https://github.com/hrodrig/kwd/releases)

## Maintainers

- **Do not edit `Casks/kwd.rb` by hand** — the next kwd tag overwrites it.
- If your local clone only shows this README, run **`git pull`** (GoReleaser commits land on **`main`** after each tag).
- If the tap did not update after a release, check the **kwd** Release workflow and **`HOMEBREW_TAP_TOKEN`** (PAT with **`contents:write`** on this repo).
