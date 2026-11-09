# .github

[![License: Apache-2.0](https://img.shields.io/badge/License-Apache--2.0-blue.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/Platform-macOS%20%7C%20Linux%20%7C%20Windows-lightgrey.svg)](#)
[![Visibility](https://img.shields.io/badge/Visibility-PUBLIC-green.svg)](#)
[![Deterministic](https://img.shields.io/badge/Deterministic-Zero--Byte%20Success-brightgreen.svg)](#)

> **Organization-wide health files, reusable workflows, issue templates, and discussions**

---

## Overview

`.github` is a core component of **Codeme** — the autonomous code quality, verification, and invariant platform.

### Key Capabilities
- **Deterministic Local Execution:** Zero-byte stdout/stderr on success (`exit 0`), actionable diagnostics on failure.
- **Cross-Platform:** Native support across macOS, Linux (Ubuntu priority), and Windows.
- **Offline-First:** Runs without cloud dependencies or paid per-call inference.
- **Agent-Ready:** Tailored for seamless integration with autonomous AI coding agents.

```mermaid
graph TD
    A[Codeme CLI / Agent] --> B[.github]
    B --> C[Deterministic Core]
    C --> D{Verification Gate}
    D -->|Success| E[Exit 0 / Silent]
    D -->|Violation| F[Actionable Diagnostics & Rollback]
```

## Governance & Boundaries
- **Ownership:** `codeme-tools/.github`
- **Visibility:** `PUBLIC`
- **License:** `Apache-2.0`
- **Allowed Component Namespaces:** `github.templates`, `github.workflows`, `github.profile`

## Security Policy
Please review [SECURITY.md](SECURITY.md) for vulnerability reporting guidelines. Under no circumstances may proprietary code or customer tokens be committed to public repositories.

## Contributing
See [CONTRIBUTING.md](CONTRIBUTING.md) for branch management, conventional commit guidelines, and verification rules.
