# Changelog

## 1.2.0

- **Built on the app's official controls.** Keys use the ChatGPT desktop app's documented shortcuts and `codex://` app links, so New chat, Settings, Skills and Scheduled open inside the app (starting it if needed).
- **Top features as keys:** Temporary chat, Quick chat, Projects, Chat/Work/Codex modes, Dictate (Win+H), Archive, Pin, Rename, Copy link, Skills, Scheduled, Full view, Go back/forward, Undo/Redo, Full screen, More/Main. 39 actions; every existing action ID is kept (Commands is now **Search**, Ctrl+K).
- **Faster, safer keys:** shortcuts go through the already-running helper, which checks that ChatGPT is really in front before each step and sends nothing otherwise. Presses do not overlap.
- **New look:** ChatGPT Dark (default) with near-black keys, white line icons, ChatGPT-green accents and bold Segoe UI labels. Every icon has its own animation (6-second loop, labels stay still). ChatGPT Light, Colourful, Vivid and Pro use the same icons; the new ChatGPT colour is the default for the colour looks.
- **Two-page layout:** page 1 has the everyday keys, **More** opens page 2.
- Installer: asks before installing Stream Deck through Windows Package Manager, waits up to 60 s for the plugin to start, keeps working when WMI is restricted, runs every rollback step independently and pins the package checksum.
- Reliability: the background helper restarts after a stuck command, and its crash budget resets after healthy replies.

## 1.1.1

- Added a double-click Windows installer with prerequisite checks, package verification, local backups, preserved profiles/settings and automatic rollback.
- Included the pinned Windows Daily Toolkit dependency for automatic app switching. Compatible or newer installed versions are kept.
- Added a connected-runtime startup receipt and isolated installer tests.
- Added installation, update, troubleshooting and recovery documentation.
- Switched the development bundler to official Rollup WASM for restricted Windows environments.
