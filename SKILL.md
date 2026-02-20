---
name: chip-kimi
description: "Use Kimi K2.5 (kimi-coding/k2p5) flagship coding model via alias 'kimi'. High-performance model for complex coding tasks, architecture design, and multi-file implementations. Equivalent to Claude 3.5 Sonnet / GPT-4o level for code generation."
---

# chip-kimi — Kimi K2.5 Flagship Model

Quick reference for using **Kimi K2.5** (kimi-coding/k2p5) through OpenClaw.

## Model Overview

| Property | Value |
|----------|-------|
| **Full ID** | `kimi-coding/k2p5` |
| **Alias** | `kimi` |
| **Provider** | Moonshot AI |
| **Context** | 256K tokens |
| **Strength** | Code generation, architecture, debugging |
| **Level** | Flagship (Claude 3.5 Sonnet / GPT-4o equivalent) |

## When to Use Kimi

**Choose Kimi when:**
- Complex multi-file implementations
- System architecture design
- Refactoring large codebases
- Debugging intricate issues
- Need deep reasoning with code

**Consider alternatives when:**
- Need fastest response (use `mmfast` / MiniMax)
- Creative writing / non-technical tasks (any model works)
- Cost-sensitive high-volume tasks

## How to Switch

### One-time switch (current session)
```
Use kimi for this task
```

Or simply mention:
```
/kimi [your request]
```

### Set as primary (default) model
Add to your OpenClaw configuration:
```yaml
model:
  default: kimi
```

### Set as fallback model
Configure fallback chain in OpenClaw:
```yaml
model:
  default: mmfast        # Primary: fast responses
  fallback: kimi         # Fallback: complex tasks
```

### Check current model
```
/status
```

Shows: `model=kimi-coding/k2p5` when active.

## Usage Patterns

### Direct model specification
```
Model: kimi

Refactor this React component to use TypeScript...
```

### Via slash command (if configured)
```
/kimi analyze this codebase
```

### In sub-agents
```yaml
model: kimi
task: complex implementation task
```

## Capabilities

- ✅ **Code generation** — Functions, classes, full modules
- ✅ **Architecture** — System design, API patterns, DB schemas
- ✅ **Refactoring** — Large-scale code transformations
- ✅ **Debugging** — Root cause analysis, fix suggestions
- ✅ **Code review** — Style, security, performance feedback
- ✅ **Documentation** — Technical docs, API references
- ✅ **Multi-language** — Python, TypeScript, Rust, Go, etc.

## Comparison

| Model | Alias | Speed | Code Quality | Best For |
|-------|-------|-------|--------------|----------|
| Kimi K2.5 | `kimi` | Medium | ⭐⭐⭐⭐⭐ | Complex coding, architecture |
| Claude Sonnet | `sonnet` | Medium | ⭐⭐⭐⭐⭐ | General purpose, reasoning |
| MiniMax M2.5 | `mmfast` | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐☆ | Fast responses, quick tasks |
| GPT-4o | — | Medium | ⭐⭐⭐⭐⭐ | General purpose |

## Tips

1. **Be specific** — Kimi handles detailed requirements well
2. **Provide context** — Use full file contents for accurate changes
3. **Multi-step tasks** — Break complex work into logical chunks
4. **Review outputs** — Always verify generated code before applying

## References

- [Moonshot AI Kimi](https://www.moonshot.ai/)
- OpenClaw model aliases in system documentation
