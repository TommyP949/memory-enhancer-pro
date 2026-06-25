# Changelog

## [2.4.1] - 2024-12-15

### Added
- Windows support via PowerShell installer (see `install-windows.ps1`)
- Cursor `.cursorrules` auto-detection across common project directories
- `config.json` schema for configuring memory tier rotation intervals

### Fixed
- Race condition when archiving hot → warm on macOS Sequoia
- Incorrect date handling in cold memory compaction

### Improved
- 40% faster session start by lazy-loading cold tier
- Better handling of large `corrections.md` files (chunked reads)

---

## [2.4.0] - 2024-11-28

### Added
- **Cross-device sync** via configurable backend (encrypted)
- OpenClaw / Hermes native integration
- Automatic `.cursor/rules/` injection on install

### Changed
- Memory tier retention: hot 7d → warm 30d → cold forever (was 3/14/90)

---

## [2.3.2] - 2024-10-10

### Fixed
- LaunchAgent label conflict on macOS when multiple workspaces active
- `corrections.md` append race in multi-session environments

---

## [2.3.0] - 2024-09-01

### Added
- GitHub Copilot integration via `.github/copilot-instructions.md`
- Cline integration via `.clinerules`
- Tiered memory visualization in status output

---

## [2.0.0] - 2024-06-15

### Breaking Changes
- Directory structure changed from `~/.ai-memory/` to `~/self-improving/`
- SOUL.md format updated (v2 schema)

### Added
- Self-improvement loop: agent logs corrections automatically
- Heartbeat maintenance protocol
- MIT license
