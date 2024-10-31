# Specifications for Multichannel Order Management project

[![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)

Specifications for MOM (Multichannel Order Management)

## Usage

This repository can be used as reference or included as an npm package to use
specification files directly.

Require the project executing:

```bash
# with npm
$ npm install -D @sprinterfront/spec-mom
# with yarn
$ yarn add -D @sprinterfront/spec-mom
```

> ❗ Remember, you have to add .npmrc file in your root project directory to
> point our dedicated npm registry. [Check .npmrc.example file](.npmrc.example).

# Development

## Requirements

You should have installed Stoplight studio to design API specifications.

Download Stoplight studio from: https://stoplight.io/studio/

## Getting started

This repository uses commitlint and standard-version to generate a CHANGELOG
file from git history commits.

To ensure correct commit message format, you should execute in root project
path:

```bash
$ yarn install
```

## Release

This project is using [semantic-release](https://github.com/semantic-release/semantic-release) to automate release process.

You just need to follow three rules:

- Use [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/)
- Use [master and maintenance branches](https://github.com/semantic-release/semantic-release/blob/master/docs/recipes/maintenance-releases.md#publishing-maintenance-releases) workflow to generate new release
- Execute the release job in Gitlab CI only when you are sure that is time to generate the release

**Notes:**

- We don't use changelog, you can check the history of the project on the [releases page](../../releases)
- Did you executed release job and the pipeline has failed? Don't worry, fix the issue with the pipeline and commit your changes with a `fix` or `feat` message to assure the release is generated.

## Publish

Publication to registries is automatically executed by release job thanks to [semantic-release](https://github.com/semantic-release/semantic-release).
