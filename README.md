# Platform Workflows

Reusable GitHub Actions workflows for portable, secure, and maintainable CI/CD.

## Available Workflows

| Workflow             | Purpose                                                                                                  |
| -------------------- | -------------------------------------------------------------------------------------------------------- |
| ci-go.yml            | Go dependency verification, formatting, static analysis, testing, and build                              |
| ci-node.yml          | npm installation, linting, testing, build, and dependency auditing                                       |
| container-build.yaml | Container build, vulnerability scanning, SBOM generation, runtime smoke testing, and registry publishing |

## Design Principles

- Portable application contracts
- Least privilege
- Immutable workflow references
- Reproducible dependency installation
- No production credentials in CI
- Compatibility with container-based deployment targets
- Incremental adoption without unnecessary abstraction

## Usage

Call reusable workflows from application repositories using `workflow_call` inputs and pin the workflow reference to a reviewed commit SHA.

## Status

Pilot-validated using lrc-translate (Go and React).

Reusable CI, container builds, security scanning, SBOM generation,
runtime smoke testing, and registry publishing are supported.

Production deployment integration is planned for a later phase.
