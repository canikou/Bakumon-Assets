# Bakumon Assets

Public downloads for the **Bakumon** Minecraft server (`play.bakumon.net`).

**New here? You probably don't need this page.** The step-by-step installation guides are in our Discord
(*Getting Started → installation guides*). They show the easiest way to install the game with pictures.

## Downloads

| What | Link | For |
|---|---|---|
| **Modpack for Prism** (import) | [Bakumon-Official-1.3.1.zip](https://github.com/canikou/Bakumon-Assets/releases/download/modpack-1.3.1/Bakumon-Official-1.3.1.zip) | Drag it onto the Prism window |
| **Modpack for the official launcher** and others | [Bakumon-Legacy-1.3.1.zip](https://github.com/canikou/Bakumon-Assets/releases/download/modpack-1.3.1/Bakumon-Legacy-1.3.1.zip) | Extract into `.minecraft` |
| **TCG resource pack** (optional backup) | [Bakumon.TCG.Additions.zip](https://github.com/canikou/Bakumon-Assets/releases/download/resourcepack/Bakumon.TCG.Additions.zip) | Only if the server doesn't load it for you |

Version, size and SHA-256 checksum of every file are in
[`downloads.json`](downloads.json). To check a download on Windows:
`Get-FileHash .\Bakumon-Official-1.3.1.zip -Algorithm SHA256`.

Older modpack versions stay available under [Releases](https://github.com/canikou/Bakumon-Assets/releases).

## What is in the modpack

Minecraft **1.21.1** with **Fabric**: the Bakumon mods, configs and resource packs, and `servers.dat` with
`play.bakumon.net` already in your server list. The zip has no account data and nothing of ours that is private.

## For maintainers

- Each modpack version is its own release, `modpack-<version>`, with the files named `Bakumon-Official-<version>.zip` (Prism) and `Bakumon-Legacy-<version>.zip`.
  The release for the version players should use is marked **Latest**. The links in the table and in the Discord guides name the
  version and are updated at every release. Only mark a version Latest once it is the public version.
- Other downloads sit in fixed releases (for example `resourcepack`) and are never marked Latest.
- After a release, `downloads.json` and the table above are updated in the same commit.
- Every modpack zip is checked before publishing (`tools/verify_client_zip.py` in the BakuBot repository): no
  server files, secrets or personal paths, and `servers.dat` points only at `play.bakumon.net`.

## Licence

The files authored in this repository are under the [MIT licence](LICENSE). The mods inside the modpack and the
resource pack belong to their authors and keep their own licences.
