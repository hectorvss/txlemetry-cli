# Txlemetry CLI

Release binaries of `txlemetry-cli`, the command-line tool for [Txlemetry](https://txlemetry.com).

## Install

```bash
npm install -g @txlemetry/cli
```

The npm package installs the binary for your platform. Prebuilt archives for every platform are also attached to each [release](../../releases):

| Platform | Archive |
| --- | --- |
| macOS Apple Silicon | `txlemetry-cli-aarch64-apple-darwin.tar.gz` |
| macOS Intel | `txlemetry-cli-x86_64-apple-darwin.tar.gz` |
| Windows x64 | `txlemetry-cli-x86_64-pc-windows-msvc.zip` |
| Windows ARM64 | `txlemetry-cli-aarch64-pc-windows-msvc.zip` |
| Linux x64 (glibc / musl) | `txlemetry-cli-x86_64-unknown-linux-gnu.tar.gz` / `-musl.tar.gz` |
| Linux ARM64 (glibc / musl) | `txlemetry-cli-aarch64-unknown-linux-gnu.tar.gz` / `-musl.tar.gz` |

`txlemetry-cli api` needs Node.js 22 or newer.

## Release validation

`Validate release` runs `txlemetry-cli --version` and `txlemetry-cli api --agent-help` against the release archives on macOS (Apple Silicon and Intel) and Windows ARM64 runners and uploads one evidence record per platform.
