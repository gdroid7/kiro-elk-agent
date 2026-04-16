---
inclusion: always
---

# Tech Stack

## ELK Stack
- Elasticsearch 8.12.0 — document store + search
- Logstash 8.12.0 — log pipeline (Beats → filter → ES)
- Kibana 8.12.0 — dashboards + UI
- Filebeat 8.12.0 — log shipper (file → Logstash)

## Orchestration
- Docker Compose 3.8

## Agent format
- Kiro markdown agents with YAML frontmatter
- Step-by-step instructions, one Q per message, caveman style
- Templates use `{{PLACEHOLDER}}` substitution pattern

## Requirements (target repos)
- Docker Desktop
- Git repo
- Log file (JSON or plain text)
