# renovate-config

[![CI Status](https://github.com/kachick/renovate-config/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/kachick/renovate-config/actions/workflows/ci.yml?query=branch%3Amain+)

Personal [shareable config presets](https://docs.renovatebot.com/config-presets/) for Renovate.

## Usage

Add the preset to your `renovate.jsonc`:

```jsonc
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": [
    "github>kachick/renovate-config//default.jsonc"
  ]
}
```
