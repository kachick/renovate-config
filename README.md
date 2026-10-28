# renovate-config

[![CI Status](https://github.com/kachick/renovate-config/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/kachick/renovate-config/actions/workflows/ci.yml?query=branch%3Amain+)

Personal [shareable config presets](https://docs.renovatebot.com/config-presets/) for Renovate.

## Usage

Add the preset to your `renovate.jsonc`:

```jsonc
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": [
    "github>kachick"
  ]
}
```

## Included Configurations

- Uses WASM plugin updates from [kachick/renovate-config-dprint](https://github.com/kachick/renovate-config-dprint)
- Schedules updates on Tuesday with a 7-day minimum release age
- Disables semantic commits and Nix manager
- Adds `dependencies` and `renovate` labels
