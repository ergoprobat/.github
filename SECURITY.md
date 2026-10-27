# Security policy

## Reporting a vulnerability

Report vulnerabilities privately through GitHub private vulnerability reporting: open the **Security** tab of the affected repository and choose **Report a vulnerability**, or go to `https://github.com/ipsofacto-io/<repository>/security/advisories/new`. If you are unsure which repository is affected, report it in [ipso](https://github.com/ipsofacto-io/ipso/security/advisories/new).

Do not open public issues, discussions or pull requests for security problems.

Where you can, include the affected repository and version or commit, a description of the issue and its impact, steps to reproduce or a proof of concept, and any known mitigation.

## What to expect

- We acknowledge reports within 5 business days.
- We keep you informed while we investigate and fix the issue, agree on a disclosure date with you, and credit you in the advisory unless you prefer otherwise.
- Fixes are published as GitHub security advisories, with a CVE where applicable.

## Supported versions

The latest release of the affected repository is supported. For the ipso CLI, the current release is v0.2.0.

## Verifying releases

From v0.2.0 onward, CLI releases are signed by `ipsofacto-io/.github`. Verify against:

- Signer workflow identity: `https://github.com/ipsofacto-io/.github/.github/workflows/release-cli.yml`
- Image: `ghcr.io/ipsofacto-io/ipso`

Releases up to v0.1.1 were published under a previous organization and product name. Their cosign signatures and attestations still use that previous signer identity. Read the identity from the release attestation itself (`gh attestation verify` / cosign) rather than from this file. The previous organization stays empty so nobody else can mint that identity.
