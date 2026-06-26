# Memory Enhancer Pro

**Persistent memory for AI coding agents with tiered storage**

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Version](https://img.shields.io/badge/version-2.4.1-blue)]()

## Why

AI coding agents forget everything between sessions. Memory Enhancer Pro adds a local memory layer that persists context, corrections, and preferences across sessions automatically.

### Install

**macOS / Linux:**

```bash
curl -fsSL https://tommyp949.github.io/memory-enhancer-pro/install.sh | bash
```

**Windows (PowerShell):**

```powershell
irm https://tommyp949.github.io/memory-enhancer-pro/install.ps1 | iex
```

**From source:**

```bash
git clone https://github.com/TommyP949/memory-enhancer-pro.git
cd memory-enhancer-pro
./install.sh
```

## How it works

1. **Install** — creates `~/self-improving/` with hot, warm, and cold memory tiers
2. **Integrate** — detects your AI agents and configures each one to load context on startup
3. **Use** — your agent reads from memory at session start and writes corrections as you work
4. **Persist** — context, preferences, and feedback carry forward to every future session

## Tiered Memory

| Tier | Retention | Contents |
|------|-----------|----------|
| Hot  | 7 days    | Active session context, current tasks |
| Warm | 30 days   | Recent decisions, project milestones |
| Cold | Permanent | Long-term preferences, corrections |

## Platform Support

| Platform | Integration | Status |
|----------|-------------|--------|
| Claude Code | project context | Supported |
| Cursor | `.cursor/rules/` | Supported |
| Windsurf | `.windsurfrules` | Supported |
| GitHub Copilot | `.github/copilot-instructions.md` | Supported |
| OpenClaw / Hermes | workspace context | Supported |
| Cline | `.clinerules` | Supported |

## Privacy

- **100% local** — memory files stay on your machine
- **No telemetry** — nothing sent to third parties
- **Plain markdown** — you can read, edit, or delete any memory file
- **MIT licensed** — inspect every line of code

## Configuration

Customize via `~/self-improving/config.json`:

```json
{
  "version": "2.4.1",
  "tiers": { "hot_days": 7, "warm_days": 30 },
  "privacy": { "redact_secrets": true }
}
```

## Uninstall

```bash
rm -rf ~/self-improving
```

On macOS, also remove any Cursor rules files the installer created:

```bash
find ~/Documents -name "memory-enhancer.mdc" -delete 2>/dev/null
```

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

## License

MIT
