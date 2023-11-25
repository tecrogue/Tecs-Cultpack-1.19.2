# .minecraft

[![Build](https://github.com/juraj-hrivnak/.minecraft/actions/workflows/Build.yml/badge.svg)](https://github.com/juraj-hrivnak/.minecraft/actions/workflows/Build.yml)

Repository template based off of juraj-hrivnak's [.minecraft template](https://github.com/juraj-hrivnak/.minecraft)
An easy-to-use template for an automated modpack development environment.

## Features

- **⌨️ Manage mods in command-line interface** using **[PAX]** without the need to use CurseForge launcher.
- **📦 Export modpack and server pack** easily, using **[PAX]** and **[ServerPackCreator]**.
- **🤝** Designed for multiple people working together...
  - **📥** Mod `.jar`s, resource packs, shader packs and overrides are handled properly! **[ModpackDownloader]**.
  - **🧰 Easy integration with [MultiMC] file structure**.
- **📝 Handle changelogs easily**, based on **[Keep a Changelog]**.
- **🧬 CI/CD** using **[GitHub Actions]**.
  - **📤 Automatically deploy** to CurseForge and GitHub in about 5 minutes.
  - **📃 Automatically generate mod changelog**.
  - **🗃️ Share development builds**.
  - **⚙️ Close issues** with the 'fixed in dev' label on release.

## How It Works

This template uses various tools to help you with your modpack development and release process.

- **Release** uses: **[PAX]** to export the modpack as zip, **[ModpackDownloader]** to download mod `.jar`'s and other files from `manifest.json`, and **[ServerPackCreator]** to remove client-side mods and create the server pack.
  - Modpack can be released using GitHub actions, which requires a CurseForge API token. (Recommended)
  - Or it can be exported locally and then released on CurseForge manually. (Not recommended)

- **Development** uses: **[PAX]** to manage mods, and **[ModpackDownloader]** to download mod `.jar`'s and other files from `manifest.json`.

![Development_02](https://github.com/juraj-hrivnak/.minecraft/assets/71150936/71a4622a-54dd-44af-9e37-e76aad3b2e2b)

<!-- Links: -->
[PAX]: https://github.com/froehlichA/pax
[ServerPackCreator]: https://github.com/Griefed/ServerPackCreator
[ModpackDownloader]: https://github.com/Joshyx/ModpackDownloader
[MultiMC]: https://multimc.org/
[Keep a Changelog]: https://keepachangelog.com/en/1.0.0/
[GitHub Actions]: .github/workflows
["Use this template"]: https://github.com/juraj-hrivnak/.minecraft/generate
[Create a new Secret for GitHub Actions]: https://docs.github.com/en/actions/security-guides/encrypted-secrets#creating-encrypted-secrets-for-a-repository
