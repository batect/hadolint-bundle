# hadolint-bundle

[![Build Status](https://img.shields.io/github/workflow/status/batect/hadolint-bundle/Pipeline/master)](https://github.com/batect/hadolint-bundle/actions?query=workflow%3APipeline+branch%3Amaster)
[![License](https://img.shields.io/github/license/batect/hadolint-bundle.svg)](https://opensource.org/licenses/Apache-2.0)

A bundle for [batect](https://batect.dev) that provides a task to lint Dockerfiles with [Hadolint](https://github.com/hadolint/hadolint).

## Usage

### Setup

Add the following to your `batect.yml`:

```yaml
include:
  - type: git
    repo: https://github.com/batect/hadolint-bundle.git
    ref: XXX # Replace with latest version from https://github.com/batect/hadolint-bundle/releases
```

### Tasks

### `lint:docker`

Runs [Hadolint](https://github.com/hadolint/hadolint) on all Dockerfiles in the project directory.

Exits with a non-zero status code if any issues are found.

## Development

Run `./batect --list-tasks` to see a list of available tasks for this project.
