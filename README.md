# Chat Guard Plugin

Generic, shareable plugin artifact package for Minecraft servers.

## What This Repository Contains
- jar/ChatGuard-1.1.1.jar
- metadata/plugin.yml
- Documentation files for safe usage and publishing.

## Platform
- Paper/Spigot

## Purpose
Profanity, ad, and spam protection for public chat.

## Installation
1. Stop your server (or proxy for Velocity plugins).
2. Copy jar/ChatGuard-1.1.1.jar into the correct plugins/ directory.
3. Start the server.
4. Configure generated files under your server's plugin config folder.

## Technical Metadata
- Internal plugin name: $(@{Kind=paper; Name=PeraChatGuard; Version=1.1.0; Main=me.peranw.chatguard.PeraChatGuardPlugin; RawMeta=name: PeraChatGuard
version: 1.1.0
main: me.peranw.chatguard.PeraChatGuardPlugin
api-version: "1.20"
author: PeraNW
commands:
  perachatguard:
    description: PeraChatGuard yönetim komutu
    usage: /perachatguard reload
permissions:
  perachatguard.reload:
    default: op
  perachatguard.bypass:
    default: op
  perachatguard.notify:
    default: op
}.Name)
- Internal version: $(@{Kind=paper; Name=PeraChatGuard; Version=1.1.0; Main=me.peranw.chatguard.PeraChatGuardPlugin; RawMeta=name: PeraChatGuard
version: 1.1.0
main: me.peranw.chatguard.PeraChatGuardPlugin
api-version: "1.20"
author: PeraNW
commands:
  perachatguard:
    description: PeraChatGuard yönetim komutu
    usage: /perachatguard reload
permissions:
  perachatguard.reload:
    default: op
  perachatguard.bypass:
    default: op
  perachatguard.notify:
    default: op
}.Version)
- Main class: $(@{Kind=paper; Name=PeraChatGuard; Version=1.1.0; Main=me.peranw.chatguard.PeraChatGuardPlugin; RawMeta=name: PeraChatGuard
version: 1.1.0
main: me.peranw.chatguard.PeraChatGuardPlugin
api-version: "1.20"
author: PeraNW
commands:
  perachatguard:
    description: PeraChatGuard yönetim komutu
    usage: /perachatguard reload
permissions:
  perachatguard.reload:
    default: op
  perachatguard.bypass:
    default: op
  perachatguard.notify:
    default: op
}.Main)

## Important Notes
- This repository is intentionally infrastructure-free (no Docker, no MariaDB dumps, no production compose files).
- Binary internals are preserved from the live-tested artifact. Rebranding inside bytecode or message localization requires source-code rebuild.
- Public release docs are fully in English.

## License
No license is bundled automatically. Add your preferred license before public release.
