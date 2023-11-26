# Go Example Flake Project

## Overview
A Nix flake project tailored for Go development, featuring multi-platform support and a focus on reproducibility.

## Structure
- `cmd/main.go`: Main Go application source.
- `flake.nix`: Configures Nix dependencies and project outputs.
- `flake.lock`: Lock file for Nix dependencies.
- `go.mod`: Go module definition.

## Features
- Supports multiple platforms: Linux (`x86_64`, `aarch64`) and Darwin (`x86_64`, `aarch64`).
- Utilizes Nix flakes for dependency management and reproducible builds.
- Development shells equipped with Go-specific tools (`go-mockery`, `golangci-lint`, `go_1_21`, `just`).

## Usage
- Compile using Nix commands.
- Development environment setup with tailored dev shells.

```
# Inspect the flake
nix flake show

# Others
nix build
nix run
nix develop
```
