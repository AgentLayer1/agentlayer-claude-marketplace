<div align="center">

<img src="assets/agentlayer-logo.png" alt="AgentLayer" width="120" />

# AgentLayer Claude Code Marketplace

**Agentic primitives, identity-aware assistants, and industry-tuned skill packs.**
Curated plugins for [Claude Code](https://docs.claude.com/en/docs/claude-code), maintained by [AgentLayer](https://agentlayer.one).

[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](./LICENSE)
[![Claude Code](https://img.shields.io/badge/Claude_Code-marketplace-orange.svg)](https://docs.claude.com/en/docs/claude-code)

</div>

---

## What's inside

| Plugin | What it does | License |
|---|---|---|
| [`agent-kevin`](./agent-kevin) | Portable, file-based personal AI assistant. Knowledge pipeline, project lifecycles, daily/weekly/monthly cadences, SEO audit suite. | Apache-2.0 |

More plugins are in the AgentLayer roadmap. Watch this repo or follow [agentlayer.one](https://agentlayer.one) for updates.

---

## Install

From inside any running Claude Code session:

```text
/plugin marketplace add github:AgentLayer1/agentlayer-claude-marketplace
```

### Updating

```text
/plugin marketplace update agentlayer
```

Or, if you cloned this repo locally, `git pull` and re-launch Claude Code.

### Local development

```bash
git clone https://github.com/AgentLayer1/agentlayer-claude-marketplace ~/Developer/agentlayer-claude-marketplace
cd ~/Developer/agentlayer-claude-marketplace
# Inside Claude Code:
/plugin marketplace add /Users/<you>/Developer/agentlayer-claude-marketplace
```

This adds the local directory as a marketplace. Any edits you make to plugins in the repo show up after a `/reload-plugins`.

---

## What AgentLayer builds

AgentLayer is an enterprise platform for designing, building, and orchestrating AI agent systems across industries. We provide:

1. A **runtime engine** for long-running agent processes (where regulatory boundaries permit).
2. **Agentic primitives**, knowledge pipelines, task systems, dispatch tools, cadence frameworks, that anyone can compose into a working assistant.
3. **Industry-tuned modules** covering fintech, government, healthcare, legal, education, and hospitality, each with built-in human oversight, audit trails, and ASEAN-regional compliance awareness.

This marketplace is how those primitives reach Claude Code users today, as portable, locally-running plugins. Larger AgentLayer products run elsewhere; everything here is the open-source, single-machine slice.

---

## Roadmap

Plugins AgentLayer is exploring next:

- **agent-mira** (working title): finance-focused assistant, bookkeeping + reconciliation + KYC workflows.
- **agent-jules**: paralegal assistant, statute lookup + case briefing + drafting.
- **agent-luna**: education assistant, lesson planning + curriculum tracking + student feedback synthesis.
- **agent-haven**: hospitality assistant, guest CRM + booking ops + multilingual concierge prompts.

Each will follow the same pattern as Kevin: portable markdown brain, MCP server for tools, hooks for the session lifecycle, opt-in skill packs.

---

## Contributing

We welcome PRs that:

- Add a new plugin under this marketplace
- Improve existing plugins (skills, dispatch tools, documentation)
- Add platform-specific notes (currently macOS-tested; Linux and Windows notes wanted)
- Translate documentation

Open an issue first for architectural changes. Each plugin maintains its own `LICENSE`, `NOTICE`, and `CONTRIBUTING` if needed.

---

## License

This marketplace catalog and the included plugins are licensed under [Apache 2.0](./LICENSE). Each plugin may also carry its own LICENSE/NOTICE inside its subdirectory; the inner license governs that plugin specifically.

Third-party skill libraries installable via individual plugins (e.g. via `/agent-kevin:configure-skills` → skills.sh) are not bundled here. They install from upstream repos each carrying their own LICENSE.

---

<div align="center">

<a href="https://agentlayer.one"><img src="assets/agentlayer-logo.png" alt="AgentLayer" height="40" /></a>

**Built by [AgentLayer](https://agentlayer.one)** · *agentic infrastructure for AI-native operations*

</div>
