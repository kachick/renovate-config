# Agent Guidelines

## Principles

- Keep items solid and concise (around one line per item) to avoid noise for human maintainers.
- Rules here are preferred guidelines; requirements in `README.md` always take priority.

## Renovate Configuration

- Always use `.jsonc` instead of `.json` or `.json5` for Renovate configurations and presets.
- Place all shared presets under the `presets/` directory.
- Never let Renovate update compiler or runtime versions (such as Go versions in `go.mod`, Node engines in `package.json`, Ruby versions in `Gemfile`, or `rust-version` in `Cargo.toml`) because toolchains are managed and synchronized through Nix and `bump-flake` workflows.
- When adding or updating presets, consider updating the automerge logic in `kachick/workflows` (`pkgs/automerge/`) so new PR body patterns or update types are allowed.
