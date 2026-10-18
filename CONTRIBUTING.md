# Contributing to ergo

Thanks for your interest in ergo. The project is pre-alpha: most repositories are still empty, and the first code lands with the initial open source release. Until then, the most useful contributions are discussions and issues.

## Before you start

- Search existing issues and [discussions](https://github.com/ergoprobat/ergo/discussions) first.
- For anything larger than a small fix, open an issue to agree on the approach before writing code.
- Report security issues privately as described in the [security policy](https://github.com/ergoprobat/.github/blob/main/SECURITY.md), never in a public issue.

## Licenses and contributor terms

| Repository | License | Contributor terms |
| --- | --- | --- |
| `edr-spec` | CC-BY-4.0 (text), Apache-2.0 (schema) | DCO |
| `ergo`, `ergo-action`, `agent-plugins`, `examples` | Apache-2.0 | DCO |
| `terraform-provider-ergo` | MPL-2.0 | DCO |
| `ergo-server` | FSL-1.1-ALv2 | CLA |
| `.github` | CC-BY-4.0 | DCO |

**DCO.** Every commit must carry a `Signed-off-by` trailer certifying the [Developer Certificate of Origin](https://developercertificate.org/). Add it with `git commit -s`; edits made in the GitHub web editor add it automatically.

**CLA.** `ergo-server` is source-available under the Functional Source License, and each release converts to Apache-2.0 after two years. Contributions to it need a one-time Contributor License Agreement. The agreement is still being finalized, so `ergo-server` does not accept outside contributions yet.

## Pull requests

- Branch from `main` and open a pull request. Changes are merged with squash merge only.
- The pull request title becomes the commit subject, so it must follow [Conventional Commits](https://www.conventionalcommits.org/), for example `feat(cli): add explain command` or `docs: clarify waiver expiry`.
- Fill in the pull request template, including the decisions the change affects.
- Keep each pull request to one logical change. Required checks must pass, and a maintainer reviews every change.
- The default branch accepts only signed commits; squash merges made through GitHub satisfy this.

## Code of conduct

Everyone taking part in ergo spaces follows the [Code of Conduct](https://github.com/ergoprobat/.github/blob/main/CODE_OF_CONDUCT.md).
