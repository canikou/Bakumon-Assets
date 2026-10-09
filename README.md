# Bakumon Assets

Public downloads for the **Bakumon** Minecraft server (`play.bakumon.net`).

**New here? You probably don't need this page.** The step-by-step installation guides are in our Discord
(*Getting Started → installation guides*). They show the easiest way to install the game with pictures.

## Downloads

| What | Link | For |
|---|---|---|
| **Modpack (manual install)**, newest version | [Bakumon-Legacy.zip](https://github.com/canikou/Bakumon-Assets/releases/latest/download/Bakumon-Legacy.zip) | Players who can't use CurseForge or Prism |
| **TCG resource pack** (optional backup) | [Bakumon.TCG.Additions.zip](https://github.com/canikou/Bakumon-Assets/releases/download/resourcepack/Bakumon.TCG.Additions.zip) | Only if the server doesn't load it for you |

The link in the first row always gives the **newest** modpack. Version, size and SHA-256 checksum of every file are in
[`downloads.json`](downloads.json). To check a download on Windows:
`Get-FileHash .\Bakumon-Legacy.zip -Algorithm SHA256`.

Older modpack versions stay available under [Releases](https://github.com/canikou/Bakumon-Assets/releases).

## What is in the modpack

Minecraft **1.21.1** with **Fabric**: the Bakumon mods, configs and resource packs, and `servers.dat` with
`play.bakumon.net` already in your server list. The zip has no account data and nothing of ours that is private.

## For maintainers

- Each modpack version is its own release, `modpack-<version>`, with the file named exactly `Bakumon-Legacy.zip`.
  The release for the version players should use is marked **Latest**, so the link above never changes.
  Only mark a version Latest once it is the public version.
- Other downloads sit in fixed releases (for example `resourcepack`) and are never marked Latest.
- After a release, `downloads.json` and the table above are updated in the same commit.
- Every modpack zip is checked before publishing (`tools/verify_client_zip.py` in the BakuBot repository): no
  server files, secrets or personal paths, and `servers.dat` points only at `play.bakumon.net`.

## Licence

The files authored in this repository are under the [MIT licence](LICENSE). The mods inside the modpack and the
resource pack belong to their authors and keep their own licences.
