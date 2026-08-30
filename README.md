# Marquee — releases

Build artefacts for [Marquee](https://github.com/unclenemo/Marquee), and nothing else.

`latest.json` is the update feed. Every installed copy of Marquee reads this file at
sign-in, compares the version against its own, and verifies any download against the
`sha256` recorded here before installing it.

| File | What it is |
|---|---|
| `latest.json` | the update feed — version, download URL, SHA-256 |
| `Marquee-<version>.zip` (release asset) | what installed copies download and apply |
| `Marquee Setup.exe` (release asset) | the installer, for a machine that has never had it |

**This repository is public because it has to be.** A private repository's release-asset
URLs return 404 to anyone not signed in, and an updater that shipped a credential to work
around that would be publishing the credential. So the artefacts live here, on their own.

No source code and no signing key is here or ever will be.
