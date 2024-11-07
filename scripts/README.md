# Deploy binary to releases

This script is used to deploy a binary to the releases page of a GitHub repository.

## Pre-requisites
`gh cli` must be installed and authenticated.

Installation:
```sh
brew install gh
```

Authentication:
```sh
gh auth login
```

## Usage

```sh
Usage: ./build.sh [options]
Options:
  --version <version>    Version of the release
  --target <platform>    Target platform
                           Platforms:
                             * "aarch64-apple-darwin"
                             * "x86_64-apple-darwin"
                             * "aarch64-unknown-linux-gnu"
                             * "x86_64-unknown-linux-gnu"
                             * "x86_64-pc-windows-msvc"
```

## Example

```sh
./build.sh --version 1.12.0 --target aarch64-apple-darwin
```
