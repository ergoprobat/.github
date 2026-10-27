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

## Verifying releases published as ergo

Releases up to v0.1.1 were published as `ergo` from the `ergoprobat` organization. Their cosign signatures and build attestations carry the signer workflow identity `https://github.com/ergoprobat/.github/.github/workflows/release-cli.yml`, and their image is `ghcr.io/ergoprobat/ergo`. Later releases use the image `ghcr.io/ipsofacto-io/ipso` and the identity `https://github.com/ipsofacto-io/.github/.github/workflows/release-cli.yml`. Verify each release against the identity it was signed with. The `ergoprobat` organization stays empty so that nobody else can obtain a token with the old identity.
