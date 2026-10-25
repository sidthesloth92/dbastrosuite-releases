# DB Astro Suite: downloads

Official downloads for the command-line tools of [DB Astro Suite](https://dbastrosuite.com),
a set of free tools for astrophotographers.

Every release here ships prebuilt binaries for macOS, Linux and Windows
(amd64 and arm64) with a `checksums.txt`. The one-line installers download the
right archive for your machine, verify its SHA-256 checksum and put the binary
on your `PATH`.

## Celestory

Your astrophotography imaging history, read straight from your FITS headers.
Web app: [celestory.dbastrosuite.com](https://celestory.dbastrosuite.com).

macOS & Linux:

```bash
curl -fsSL https://raw.githubusercontent.com/sidthesloth92/dbastrosuite-releases/main/celestory/install.sh | sh
```

Windows (PowerShell):

```powershell
irm https://raw.githubusercontent.com/sidthesloth92/dbastrosuite-releases/main/celestory/install.ps1 | iex
```

Full guide: [celestory/README.md](celestory/README.md).
Manual downloads: [Celestory releases](https://github.com/sidthesloth92/dbastrosuite-releases/releases?q=celestory).

## Reporting a problem

Found a bug or have an idea? [Open an issue](https://github.com/sidthesloth92/dbastrosuite-releases/issues/new)
and add the label for the tool it concerns (for example `celestory`). For CLI
problems, attach the report the tool generates with `-report` if you can; it
masks paths under your home directory.

## Layout

```
<tool>/install.sh     macOS / Linux installer
<tool>/install.ps1    Windows installer
<tool>/README.md      tool guide
```

Releases are tagged `<tool>-vX.Y.Z` (for example `celestory-v0.0.1`), so each
tool's installer only ever picks its own releases.
