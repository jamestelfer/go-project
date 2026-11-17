# go-project

A Go command line project.

## Installation

Pre-built binaries for Linux, macOS, and Windows (amd64 and arm64) are published to
[GitHub Releases](https://github.com/jamestelfer/go-project/releases). Every archive
carries a build provenance attestation.

Verify a downloaded archive with the [GitHub CLI](https://cli.github.com/):

```sh
gh attestation verify go-project_linux_amd64.tar.gz --repo jamestelfer/go-project \
  --signer-workflow chinmina/.github/.github/workflows/goreleaser-release.yml
```

To build from source:

```sh
go install github.com/jamestelfer/go-project/cmd/cli@latest
```

## Development

Run `mise install` for the pinned toolchain, then `just verify` before committing.
See `AGENTS.md` for conventions.

## Licence

Apache 2.0. See `LICENSE`.
