# chip-kimi

OpenClaw skill for using **Kimi K2.5** flagship coding model.

## Quick Start

```bash
# Install skill (in OpenClaw workspace)
cp -r chip-kimi /opt/clawd-workspace/skills/public/
```

## Usage

Simply use the alias `kimi` in your OpenClaw session:

```
Switch to kimi model

Refactor this Python codebase to use async/await...
```

Or reference directly:

```
Using kimi-coding/k2p5, analyze this architecture...
```

## Model Specs

- **Model**: Kimi K2.5 (kimi-coding/k2p5)
- **Alias**: `kimi`
- **Context**: 256K tokens
- **Provider**: Moonshot AI
- **Strength**: Complex coding, architecture, debugging

## When to Use

- Multi-file implementations
- System architecture design
- Code refactoring
- Deep debugging
- Technical documentation

## License

MIT — See [LICENSE](LICENSE)
