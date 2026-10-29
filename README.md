# renovate-config

[![CI Status](https://github.com/kachick/renovate-config/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/kachick/renovate-config/actions/workflows/ci.yml?query=branch%3Amain+)

Personal [shareable config presets](https://docs.renovatebot.com/config-presets/) for Renovate.

## Usage

See the [presets](presets/) directory for available presets.

Add presets to your `renovate.jsonc`:

```jsonc
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": [
    "github>kachick/renovate-config//presets/default.jsonc",
    "github>kachick/renovate-config//presets/cargo.jsonc"
  ]
}
```

## Limitations

- **Lockfile-only transitive security updates**: Renovate does not update transitive (nested) dependencies in lockfiles for security fixes. Keep Dependabot security updates enabled until upstream resolves this limitation. See [#2](https://github.com/kachick/renovate-config/issues/2) and [renovatebot/renovate#46377](https://github.com/renovatebot/renovate/issues/46377).
