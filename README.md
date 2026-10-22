# 1go CLI releases

Release binaries of `1go`, the command line and MCP server of [1Go.vn](https://1go.vn) short links. This repository only holds
releases; the source is private.

```sh
npm install -g @1go/cli
# or
curl -LsSf https://github.com/kdigivn/1go-cli/releases/latest/download/onego-cli-installer.sh | sh
```

Windows (PowerShell):

```powershell
powershell -ExecutionPolicy Bypass -c "irm https://github.com/kdigivn/1go-cli/releases/latest/download/onego-cli-installer.ps1 | iex"
```

Then `1go --version` and `1go auth login`. Docs: https://docs.1go.vn

Every archive has a `.sha256` file and a GitHub build attestation (`gh attestation verify <file> -R kdigivn/1go-cli`).

`.github/workflows/release.yml` is generated in the source repo (`scripts/gen-public-release-workflow.mjs`); do not edit it here.
