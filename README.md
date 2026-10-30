# setup-codegrapher

Install an exact [CodeGrapher](https://github.com/code-grapher/codegrapher) release in GitHub Actions without Go. This action installs the CLI only; workflows choose which commands to run.

`version` is required and must be an exact release tag. `expected-sha256` optionally supplies an independently obtained digest for the selected platform archive. The release checksum file detects corruption but cannot authenticate a release if both archive and checksum are replaced. Outputs include the installed release tag and binary path.

Linux and macOS support amd64 and arm64; Windows supports amd64 where the release contains those assets.
