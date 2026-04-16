---
inclusion: always
---

# Project Structure

```
.kiro/
├── agents/                    # Kiro agents (copied to target repo)
│   ├── elk-setup.md           # Interactive ELK stack onboarding
│   ├── kibana-agent.md        # Dashboard builder from plain English
│   └── elk-debugger.md        # Pipeline debugger (read-only)
├── hooks/                     # Kiro hooks (copied to target repo)
│   └── elk-commit.md          # Auto-prompt commit after ELK config changes
├── steering/                  # Steering docs for this repo's development
│   ├── product.md
│   ├── tech.md
│   └── structure.md
└── templates/                 # Config templates with {{PLACEHOLDER}} vars
    ├── .env.example
    ├── docker-compose.yml
    ├── filebeat.yml
    ├── kibana.yml
    ├── logstash.conf
    └── Makefile
```

## Agent → template path convention
Agents read templates from `.kiro/templates/` and write rendered output to the target repo root (`elk/`, `.env`, `Makefile`, `ELK_README.md`).
