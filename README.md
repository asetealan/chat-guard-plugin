# Chat Guard Plugin

Chat Guard is a moderation plugin focused on keeping public chat clean and readable.
It is intended for servers that want strict language and spam control without giving moderation power to normal players.

## What It Does
- Filters profanity and abusive wording
- Blocks common ad-style messages (links/IP-like text patterns)
- Helps reduce repetitive chat spam
- Provides staff controls for monitoring and maintenance

## Package Contents
- `jar/ChatGuard-1.1.1.jar`
- `README.md`
- `SECURITY.md`
- `SANITIZATION_NOTES.md`
- `DISCLAIMER.md`
- `metadata/NOTES.md`

## Platform
- Paper/Spigot

## Installation
1. Stop the server.
2. Copy `jar/ChatGuard-1.1.1.jar` into `plugins/`.
3. Start the server once so plugin files initialize.
4. Tune your filter settings in generated plugin config files.
5. Restart the server (or use plugin reload if your policy allows it).

## Commands
| Command | Purpose | Permission | Default |
|---|---|---|---|
| `/ChatGuard reload` | Reload plugin config | `ChatGuard.reload` | OP |

## Permissions
| Permission | Purpose | Default |
|---|---|---|
| `ChatGuard.reload` | Access reload command | OP |
| `ChatGuard.bypass` | Ignore chat filtering | OP |
| `ChatGuard.notify` | Receive moderation notifications | OP |

## Recommended Role Setup
- Keep `ChatGuard.bypass` staff-only.
- Keep `ChatGuard.reload` admin-only.
- Give `ChatGuard.notify` to moderators who review chat.
- Do not grant any of these to default players.

## Typical Usage Flow
1. Player sends a message.
2. Plugin checks profanity/ad/spam rules.
3. If rule match occurs, message is blocked and warning is shown.
4. Staff with notify permission can receive signal messages.

## Troubleshooting
- **Too many false positives:** reduce strict words/patterns and test again.
- **Staff not getting alerts:** verify `ChatGuard.notify`.
- **Reload denied:** verify `ChatGuard.reload` on admin group.
- **No filtering happening:** confirm plugin loaded and check conflicts with other chat format/moderation plugins.

## Notes
- This repository intentionally excludes Docker/DB/infra files.
- The artifact is provided as runtime binary.
- Deep localization and internal code-level rebranding require source rebuild.
