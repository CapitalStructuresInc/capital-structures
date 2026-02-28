# BACK OFFICE

Operational infrastructure of Capital Structures Inc.

---

## How It Works

The Company operates through AI agents reviewed by humans. The CEO routes tasks to agents. Agents generate documents. Humans review and approve. Counsel reviews before filing. Everything is published.

```
CEO (Martin Grasser)
    │
    ├── assigns task ──→ Global Finance Department
    │                         │
    │                         └── generates: press releases, board resolutions,
    │                                        structure briefs, NAV updates,
    │                                        earnings call scripts
    │
    ├── assigns task ──→ Corporate Secretary
    │                         │
    │                         └── generates: board agendas, minutes, filing trackers,
    │                                        cap table updates, org memos,
    │                                        governance calendar
    │
    └── reviews all outputs
            │
            ├── Head of Operations (Audrey Chen) — first review
            ├── Securities Counsel — legal review before filing
            └── Accountant (Karie Lui) — financial accuracy
```

## Agents

| Agent | System Prompt | Claude Project |
|-------|--------------|----------------|
| Global Finance Department | [agents/global-finance-department.md](agents/global-finance-department.md) | [Set up in Claude.ai] |
| Corporate Secretary | [agents/corporate-secretary.md](agents/corporate-secretary.md) | [Set up in Claude.ai] |

## Setting Up a New Agent

1. Write the system prompt as a markdown file in `agents/`
2. Create a Claude Project on claude.ai
3. Paste the system prompt into Project Instructions
4. Upload the project bible and master reference as project knowledge
5. Test with a real task
6. Document in this README

## Document Flow

1. CEO identifies need (new structure, quarterly update, board meeting)
2. CEO prompts the appropriate agent
3. Agent generates draft
4. Head of Operations reviews for completeness
5. CEO approves
6. Counsel reviews (if filing-grade)
7. Final document archived in the structure's folder or governance folder
8. Press releases and public documents published

---

*The Back Office is a disclosed artifact of the Company's operations. Its configuration is published.*
