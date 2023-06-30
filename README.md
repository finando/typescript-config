# Finando | TypeScript configuration

Shareable and extendable TypeScript configuration.

[![semantic-release: conventionalcommits](https://img.shields.io/badge/semantic--release-conventionalcommits-e10079?logo=semantic-release)](https://github.com/semantic-release/semantic-release)
[![GitHub Actions](https://github.com/finando/typescript-config/actions/workflows/release.yaml/badge.svg)](https://github.com/finando/typescript-config/actions/workflows/release.yaml)

## Table of Contents

  - [Usage](#usage)
    - [Installation](#installation)
      - [NPM](#npm)
    - [Configuration](#configuration)
  - [Contributing](#contributing)
    - [Implementing changes](#implementing-changes)
    - [Releasing new versions](#releasing-new-versions)
  - [Change log](#change-log)

## Usage

### Installation

#### NPM
```sh
npm install -D @finando/typescript-config
```

### Configuration

The simplest possible configuration of [TypeScript](https://www.typescriptlang.org) that can be used in `tsconfig.json` is as follows:

```json
{
  "$schema": "https://json.schemastore.org/tsconfig",
  "extends": [
    "@finando/typescript-config/react"
  ]
}
```

The configuration is extensible and can thus be extended with other configurations, plugins and rules to accomodate any additional requirements.

## Contributing

### Implementing changes

In order to implement changes, create a branch from `master` branch, commit changes and open a pull request. Use [atomic](https://en.wikipedia.org/wiki/Atomic_commit) [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/) to add changes to Git history. Use `npm run commit` to start an interactive wizard that helps with formatting commits according to specified standard.

### Releasing new versions

Once changes are approved by pull request reviewers, merge the pull request to `master` branch. This will trigger an automatic release workflow in GitHub Actions. Follow along to make sure it completes successfully.

## Change log

Detailed changes for each release are documented in [CHANGELOG.md](https://github.com/finando/typescript-config/blob/HEAD/CHANGELOG.md).
