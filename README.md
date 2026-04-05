# AI Mindset Business Analyst Skill

**Product discovery & requirements analysis specialist with AI automation mindset.**

> Also available in Russian / Также доступен на русском языке (all skill files are in Russian).

## What it does

An AI coding assistant skill that guides structured product discovery and creates comprehensive product briefs. The key differentiator: **every task is evaluated through the L0-L3 automation spectrum before detailed solution design**.

### The AI Automation Mindset

Before diving into solution details, the skill forces a critical analysis step:

| Level | Approach | When to use |
|-------|----------|------------|
| **L0** | Manual | Current state baseline |
| **L1** | Rules | Deterministic logic, lookup tables, mappings |
| **L2** | Automation | Scripts, integrations, ETL, cron jobs |
| **L3** | AI-assisted | ML, LLM, embeddings, RAG, AI agents |

**Step 0: Problem Reframing** — Before optimizing a process, the skill checks whether the process itself is the problem. If users struggle with a complex UI, maybe they need an AI agent that translates intent to action, not a better UI.

### Key patterns recognized

- Fuzzy Matching, Classification, Extraction, Enrichment
- Anomaly Detection, Summarization, Routing
- **Intent-to-Action** (AI as Interface) — replacing complex UIs with conversational AI
- **Domain Assistant** — AI-guided decision making in complex domains

## Workflows

| Command | Description |
|---------|-------------|
| `/product-brief` | Full product brief through structured discovery |
| `/brainstorm-project` | Structured brainstorming with AI analysis |
| `/research` | Market and competitive research |

## Installation

### Claude Code

```bash
# Clone to your plugins directory
git clone <repo-url> ~/.claude/plugins/business-analyst
```

Or copy the skill directory to your project:

```
.claude/skills/business-analyst/
```

### Windsurf

Copy to:
```
.windsurf/skills/business-analyst/
```

### Cursor / Other agents

Copy to your project root or agent skills directory. The `SKILL.md` format is cross-platform compatible.

## Structure

```
business-analyst/
├── .claude-plugin/
│   └── plugin.json            # Plugin metadata
├── SKILL.md                   # Main skill definition
├── REFERENCE.md               # Interview frameworks & techniques reference
├── README.md                  # This file
├── resources/
│   ├── ai-mindset.md          # AI automation analysis methodology (L0-L3)
│   └── interview-frameworks.md # Detailed interview techniques
└── templates/
    ├── product-brief.template.md    # Product brief template
    └── research-report.template.md  # Research report template
```

## How it works

1. **Understand** — Review context, conduct stakeholder interviews
2. **Discover** — Use structured frameworks (5 Whys, JTBD, SMART)
3. **Confirm** — Validate understanding with stakeholders
4. **Analyze automation potential** (blocking step):
   - Step 0: Reframe the problem (is the process itself the problem?)
   - Step 1: Pain map (manual steps, cognitive complexity, intent-action gap)
   - Step 2: Solution spectrum L0-L3
   - Steps 3-4: Evaluation matrix & AI pattern matching
   - Step 5: Recommendation (level, MVP, evolution path, fallback)
   - Step 6: Anti-pattern self-check
5. **Deliver** — Create product brief with automation analysis section
6. **Hand off** — To product manager for PRD creation

## Anti-patterns the skill checks for

- **AI Hammer** — proposing AI where simple rules suffice
- **UI Tunnel Vision** — optimizing a UI instead of questioning whether it's needed
- **Process Fixation** — optimizing steps instead of replacing the whole process
- **Data Blindness** — proposing ML without checking data availability
- **Premature Complexity** — complex solution for low-volume operations

## Language

All skill content is in **Russian**. The skill works with any user language — the agent adapts its responses to the user's language while following the Russian-language methodology internally.

## Compatibility

Works with any AI coding assistant that supports the `SKILL.md` / `AGENTS.md` format:
- Claude Code
- Cursor
- Windsurf (Cascade)
- Cline
- Gemini CLI
- Codex CLI
- And others

## License

MIT
