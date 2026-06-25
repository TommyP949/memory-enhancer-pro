# Contributing to Memory Enhancer Pro

Thank you for your interest in contributing! 🎉

## Getting Started

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/your-feature`
3. Make your changes
4. Run tests: `./tests/run.sh`
5. Submit a pull request

## Development Setup

```bash
git clone https://github.com/TommyP949/memory-enhancer-pro.git
cd memory-enhancer-pro
chmod +x install.sh
./install.sh
```

## Code Style

- Shell scripts: POSIX-compatible where possible, bash where needed
- Keep install.sh idempotent (safe to run multiple times)
- All new features should update the memory tier structure

## Reporting Bugs

Open an issue with:
- Your OS and architecture
- AI agent platform (Claude Desktop, Cursor, etc.)
- Steps to reproduce
- Expected vs actual behavior

## Feature Requests

We welcome feature requests! Common asks we're working on:

- [ ] Windows native support (currently via WSL)
- [ ] Web UI for browsing memory tiers
- [ ] Import from other memory systems
- [ ] Memory search and filtering

## License

By contributing, you agree your contributions are licensed under MIT.
