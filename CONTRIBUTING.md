# Contributing to bp-centiles-app

This repository contains a SMART/FHIR blood-pressure centile application. The [readme](readme.md) explicitly marks it deprecated and not actively maintained; this guide describes how to prepare a useful change without implying renewed support.

## Before you start

Search existing issues and pull requests before starting, and discuss substantial changes or new dependencies in an issue. Use an issue template when one is offered. For a bug, include the affected commit or version, environment, a minimal reproduction, and expected versus observed behavior; remove sensitive information from logs and screenshots.

## Development and validation

The [package.json](package.json) defines the local preview workflow documented in the README:

```sh
npm install
npm run serve
```

Use a compatible Node environment and record the version and browser used. There is no npm test script in this manifest. For changed behavior, provide a focused reproducible check and explain any validation that remains unavailable.

Check input units, age or measurement boundaries, missing values, centile calculations, and the print view when relevant. Use fictional observations and a synthetic SMART/FHIR test context. Document the source and assumptions for clinical calculations; distinguish software verification from clinical validation. Keep dependency or protocol modernization scoped and explain compatibility implications for the existing application.

## Pull requests

Work on a focused branch from the current default branch. Open a pull request explaining the problem, the resulting behavior, and any compatibility or data-format changes. Link the relevant issue and complete any existing PR template.

Add focused regression coverage for changed behavior and update affected examples or documentation. Describe the checks actually run, their results, and any checks you could not run. For documentation-only changes, verify links, examples, and rendered formatting. Use the repository's existing checks and review/merge process; preserve required checks and resolve actionable feedback without weakening the checks.

## Security and sensitive information

Follow the [account security policy](https://github.com/edithatogo/.github/blob/main/SECURITY.md). Report vulnerabilities privately through the repository's **Report a vulnerability** option if available; otherwise request a private reporting contact without posting exploit details. Never include credentials, personal information, restricted datasets, or confidential records in issues, commits, fixtures, or diagnostic output.

## Licensing and conduct

The repository's [license](LICENSE) continues to apply. Be respectful and constructive, and follow the [account code of conduct](https://github.com/edithatogo/.github/blob/main/CODE_OF_CONDUCT.md). Preserve attribution and third-party notices. Contribute only material you are entitled to share; resolve unclear permissions before adding third-party content. This guide does not change licensing terms or introduce a CLA or DCO requirement.

## References

- [GitHub contribution guideline conventions](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/setting-guidelines-for-repository-contributors)
- [OpenSSF contribution and quality criteria](https://www.bestpractices.dev/en/criteria)
