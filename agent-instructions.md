# Agent Instructions

This repository contains the dependency-free static website for The Sicknotes. It is not a web application or a build-based site.

## Read First

- [README.md](README.md) - project overview and local preview.
- [agent-instructions.md](agent-instructions.md) - local guardrails.
- [~/code/house-style/AGENTS.md](~/code/house-style/AGENTS.md) - cross-repository standards.

## Core Invariants

- Keep the site dependency-free: plain HTML, CSS, and local assets only.
- Preserve the supplied copy, original imagery, links, and High Cruiser typography unless the owner explicitly changes them.
- Keep GitHub Pages artifact-based. Do not add a `gh-pages` branch deployment.
- Record third-party asset and font provenance in [README.md](README.md) and [REUSE.toml](REUSE.toml).

## Workflow

- `s/up` - serve on the first free port from 8000 to 8030, or from a supplied start port.
- `s/lint` - verify local HTML/CSS assets and whitespace.

## Before Every Commit

```sh
s/lint
```

## Approval Required

Ask before publishing releases, changing the custom domain, changing DNS, deleting branches, force-pushing, or changing licences and asset rights.
