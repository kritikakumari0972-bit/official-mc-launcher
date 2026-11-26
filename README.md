# Official MC Launcher

A community-maintained Minecraft launcher fork with its own project identity.

> **Important:** Official MC Launcher is an independent community project. It is **not affiliated with, endorsed by, or an official product of Mojang Studios or Microsoft**. Minecraft is a trademark of Mojang Studios. The word “Official” is part of this project's chosen name only and does not indicate Mojang/Microsoft approval.

## Project origin and license

This repository is based on the **Millida Launcher** open-source project and is being rebranded and adapted independently. The upstream source is licensed under **GNU GPL v3.0 only**. This fork retains the upstream license and required notices. See:

- [LICENSE](LICENSE)
- [NOTICE](NOTICE)
- [TRADEMARK.md](TRADEMARK.md) and [TRADEMARK.ru.md](TRADEMARK.ru.md)
- [THIRD-PARTY.md](THIRD-PARTY.md)

The Millida name, logos, artwork, domains, credentials, and hosted services are not part of the GPL license and are not used as this project's brand. Upstream attribution is retained.

## Current project status

This repository is in the rebranding and integration stage. The desktop application is built with **Tauri 2, Rust, React, TypeScript, and Vite**.

The codebase contains integrations that originally depended on Millida-operated services. Those integrations must be replaced with independently configured services or disabled before being presented as working in an Official MC Launcher release. Do not assume Millida account, social, skin/cape, rating, hosting, CurseForge proxy, or auto-update services are available in this fork.

## Build prerequisites

- Git
- Rust toolchain (stable)
- Bun
- Platform-specific Tauri prerequisites: https://v2.tauri.app/start/prerequisites/

Install dependencies:

```bash
bun install
```

Run the desktop app in development:

```bash
bun run tauri dev
```

Build the frontend:

```bash
bun run build:web
```

Build a release bundle (after platform prerequisites are installed):

```bash
bun run build:release
```

## Roadmap

- [x] Create an independently named GitHub project
- [x] Replace the initial app/package identity and desktop metadata
- [ ] Replace upstream logos, icons, splash art, and other protected brand assets with original artwork
- [ ] Audit and remove upstream service endpoints, credentials, and updater configuration
- [ ] Configure independent Microsoft sign-in registration
- [ ] Verify offline account and Minecraft version installation flows
- [ ] Run platform builds and automated tests
- [ ] Publish signed releases and checksums

## Contributing

Please open an issue before large changes. Preserve GPL-3.0-only and all third-party notices. Clearly mark modified upstream components and do not include credentials or private keys in commits.

## Disclaimer

This project is not an official Minecraft product and is not approved by or associated with Mojang Studios or Microsoft. Users must obtain Minecraft through legitimate channels and comply with the applicable Minecraft terms.
