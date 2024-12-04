# Contributing to the Anim Chess Project <!-- omit from toc -->

Thank you for taking time to contribute to the Anim Chess Project. As a contributor, below are the guidelines we would like you to follow:

- [Code of Conduct](#code-of-conduct)
- [Submission Guidelines](#submission-guidelines)
  - [Submitting an Issue](#submitting-an-issue)
  - [Submitting a Pull Request (PR)](#submitting-a-pull-request-pr)
- [Branch Organization](#branch-organization)
- [Commit Message Format](#commit-message-format)
- [Semantic Versioning](#semantic-versioning)
- [Development](#development)
- [License](#license)

# Code of Conduct
Please read and follow our [Code of Conduct](https://github.com/lborres/animchess/blob/main/CODE_OF_CONDUCT.md).

# Submission Guidelines
## Submitting an Issue
Before submitting an issue, please check the Issues tab to see if your issue already exists.

Bugs will only be fixed if they can be reproduced and confirmed to occur. Please include steps on how to reproduce any bugs or issues.

New feature requests should be discussed before any time is spent building them.

## Submitting a Pull Request (PR)
The core team is actively monitoring for pull requests. We'll do our best to provide updates and feedback throughout the process.

Please **fork** the repository and create your branch off of main.

The proposed changes in the PR must NOT have any build errors.
As of writing, no test suites are available yet. If a test suite exists by the time you are reading this, please ensure the tests pass.

If you are proposing a bug fix or new code/feature, we encourage you to add tests for it. However, this is not required as of writing (2024-12-04).

# Branch Organization
Code that lands in **main** must be compatible with the latest stable release. It may contain additional features, but no breaking changes. We should be able to release a new minor version from the tip of **main** at any time.

# Commit Message Format
Please see the [Conventional Commits Specifications](https://www.conventionalcommits.org/en/v1.0.0/).\
Also, read [AngularJS commit message format](https://github.com/angular/angular/blob/main/CONTRIBUTING.md#-commit-message-format) for additional information.

We use the [Conventional Commits Specifications](https://www.conventionalcommits.org/en/v1.0.0/) to enable a number of automation solutions such as auto generated changelogs and determining a semantic version bump.

# Semantic Versioning
The Anim Chess project follows semantic versioning. We release patch versions for critical bugfixes, minor versions for new features or non-essential changes, and major versions for any breaking changes.

Every significant change shall be documented in the [changelog file](https://github.com/lborres/animchess/blob/main/CHANGELOG.md).

<!-- ## Packages -->


# Development
This repository is managed with [turborepo](https://turbo.build/repo/docs#what-is-turborepo) and [pnpm](https://pnpm.io/motivation).\
Please have [pnpm installed](https://pnpm.io/installation).\
Turborepo also recommends you [install turborepo globally](https://turbo.build/repo/docs/getting-started/installation#installing-turbo): `pnpm install turbo --global`

The following commands will be useful in development:

**Commands run at the root of the project**
1. `pnpm install` - will install all the project's dependencies. This includes all npm projects defined in the *pnpm-workspace.yaml* file.
2. `pnpm dev` or `pnpm run dev` - will run the development environment for all the apps in this project. This may fail if you do not have the appropriate `.env` files.

<!-- # Building
**Commands run at the root of the project**
1. `pnpm build` or `pnpm run build` - runs all the build scripts -->

# License
By contributing to the Anim Chess project, you agree that your contributions will be licensed under the project's stated [LICENSE](https://github.com/lborres/animchess/blob/main/LICENSE).
