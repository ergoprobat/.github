# ipso

[![OpenSSF Scorecard](https://api.scorecard.dev/projects/github.com/ipsofacto-io/ipso/badge)](https://scorecard.dev/viewer/?uri=github.com/ipsofacto-io/ipso)
[![OpenSSF Best Practices](https://www.bestpractices.dev/projects/15758/badge)](https://www.bestpractices.dev/en/projects/15758)

Registry of binding engineering decisions, enforced at PR, CI, plan and AI-agent time.

Architecture and infrastructure decisions usually live in ADRs, PR threads and chat, where nothing enforces them and nobody can prove which rules applied when a change shipped. AI coding agents now write a large share of changes and follow rules files only probabilistically. ipso makes every binding decision explicit, owned, scoped and time-bounded, compiles it into checks for engines teams already run (OPA/Conftest, Semgrep, dependency-cruiser, ArchUnit, Checkov, Kyverno), and enforces it on pull requests, in CI, on `terraform plan` and before an AI agent edits a file. LLMs may propose decisions; people approve them, and only deterministic checks block.

> Status: pre-alpha. The repositories are set up; code lands with the first open source release.

## Repositories

| Repository | What it holds | License |
| --- | --- | --- |
| [edr-spec](https://github.com/ipsofacto-io/edr-spec) | Open specification and JSON Schema for the Engineering Decision Record (EDR) format | CC-BY-4.0 / Apache-2.0 |
| [ipso](https://github.com/ipsofacto-io/ipso) | CLI, check compilers, agent hooks and local MCP server | Apache-2.0 |
| [ipso-action](https://github.com/ipsofacto-io/ipso-action) | GitHub Action that runs ipso checks in CI | Apache-2.0 |
| [agent-plugins](https://github.com/ipsofacto-io/agent-plugins) | Claude Code, Cursor, Copilot and Kiro plugins | Apache-2.0 |
| [examples](https://github.com/ipsofacto-io/examples) | Sample repositories with enforced decisions | Apache-2.0 |
| [ipso-server](https://github.com/ipsofacto-io/ipso-server) | Source-available control plane | FSL-1.1-ALv2 |
| [terraform-provider-ipso](https://github.com/ipsofacto-io/terraform-provider-ipso) | Terraform and OpenTofu provider | MPL-2.0 |

## Get involved

- Questions and ideas: [Discussions in ipso](https://github.com/ipsofacto-io/ipso/discussions)
- How to contribute: [CONTRIBUTING.md](https://github.com/ipsofacto-io/.github/blob/main/CONTRIBUTING.md)
- Security reports: [SECURITY.md](https://github.com/ipsofacto-io/.github/blob/main/SECURITY.md)
