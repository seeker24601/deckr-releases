# deckr downloads

Download the desktop preview and companion packages from [Releases](https://github.com/seeker24601/deckr-releases/releases/latest) or [deckr.sh](https://deckr.sh/downloads.html).

The source development repository is private. This repository holds public release files and installation instructions. The application includes its executable runtime and required third-party licenses.

## macOS Apple Silicon preview

1. Download `deckr-macos-arm64.zip`, unzip it, and move `deckr.app` to Applications.
2. Open deckr. The preview is unsigned and not notarized; macOS may require explicit approval in System Settings → Privacy & Security.
3. Allow first-launch setup to finish. An internet connection is required to download Python and runtime dependencies.
4. Configure your own model provider in the application. Rook is included.

Windows and Intel Mac downloads are not available in this release. Existing development checkouts are separate installations; the downloadable app does not import their credentials, conversations, or memory.

## Add companions

Download a `.deckr-companion` file and open it with deckr. Review the installation prompt. Luna and Taizong include executable plugins and require explicit consent. Restart deckr after installation, then choose the companion in Team.

Companions share the desktop client, with separate instructions, conversations, and memory. Reinstalling an existing companion is rejected to preserve local changes.

## Verification and updates

Every release includes `release.json` and `SHA256SUMS`. On macOS, run `shasum -a 256 <downloaded-file>` and compare its result with the published checksum. A checksum checks the file contents; it is not a code signature.

The latest client link follows the latest published release. Client updates are manual for this preview; built-in Hermes update and repair do not replace the Deckr runtime. Companion links identify exact package versions.
