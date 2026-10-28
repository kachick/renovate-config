# renovate-config

[![CI Status](https://github.com/kachick/renovate-config/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/kachick/renovate-config/actions/workflows/ci.yml?query=branch%3Amain+)

Personal [shareable config presets](https://docs.renovatebot.com/config-presets/) for Renovate.

## Usage

Add presets to your `renovate.jsonc`:

```jsonc
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": [
    "github>kachick/renovate-config//presets/default.jsonc"
  ]
}
```

### Available Presets

- `presets/default.jsonc`: Base configuration including GitHub Actions, dprint, and Docker.
- `presets/cargo.jsonc`: Rust / Cargo dependencies with `bump` range strategy.
- `presets/gomod.jsonc`: Go modules dependencies with `gomodTidy`.
- `presets/npm.jsonc`: Node.js / npm dependencies with `bump` range strategy.

Example for combining presets:

```jsonc
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": [
    "github>kachick/renovate-config//presets/default.jsonc",
    "github>kachick/renovate-config//presets/cargo.jsonc"
  ]
}
```
