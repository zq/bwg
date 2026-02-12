# CLAUDE.md

## Project Overview

**BWG (搬瓦工)** is a Chinese-language documentation repository providing a beginner's guide to Bandwagon Host VPS services. It covers plan selection, purchase tutorials, speed testing, renewal instructions, and promotional coupon information.

**Website:** www.bandwagonhost.net

## Repository Structure

```
bwg/
├── README.md              # Project description and attribution
├── CLAUDE.md              # This file — AI assistant guidance
└── docs/                  # Documentation articles (Chinese)
    ├── plan.md            # Plan selection guide (方案选择)
    ├── purchase.md        # Purchase tutorial (购买教程)
    ├── speedtest.md       # Speed testing guide (速度测试)
    ├── renewal.md         # Renewal guide (续费教程)
    ├── cn2.md             # CN2 network line guide
    ├── cn2gia.md          # CN2 GIA line guide
    ├── hk.md              # Hong Kong datacenter plans
    └── coupon             # Promotional coupon codes (plain text)
```

## Tech Stack

- **Content format:** Markdown (`.md`) and plain text
- **Language:** Simplified Chinese
- **No build system, dependencies, or CI/CD** — this is a static documentation repository

## Development Workflow

### Branching

- Default branch: `master`
- No formal branching strategy; all historical commits are linear on `master`

### Making Changes

1. Edit or create Markdown files in the `docs/` directory
2. Keep `README.md` as the top-level project description
3. Commit with clear messages describing what was changed

### File Conventions

- Documentation files go in `docs/`
- Use `.md` extension for Markdown content
- The `coupon` file is plain text (no extension)
- All content is written in Simplified Chinese
- File names use lowercase English identifiers that map to topics (e.g., `cn2gia.md` for CN2 GIA network documentation)

## Key Conventions for AI Assistants

- **Content language:** Write documentation content in Simplified Chinese to match existing style
- **No code or build tools:** This repo has no package manager, linter, test suite, or build process. Do not introduce tooling unless explicitly requested.
- **Keep it simple:** This is a lightweight documentation project. Avoid over-engineering with static site generators or complex tooling unless asked.
- **File organization:** New documentation topics should be added as separate files in `docs/`, following the existing flat structure
- **No `.gitignore`** is present. Be careful not to commit OS-generated files (e.g., `.DS_Store`) — one was previously removed in commit history
