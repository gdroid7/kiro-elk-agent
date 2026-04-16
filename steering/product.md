---
inclusion: always
---

# Kiro ELK Agents

Three agents + one hook. Drop `.kiro/` into any repo with a log file to get ELK observability running in minutes.

## Purpose
- Ship ELK stack config to any project without manual setup
- Create Kibana dashboards from plain English descriptions
- Debug log pipeline issues step by step
- Auto-prompt git commits after ELK config changes

## Target users
Developers who want ELK observability without writing YAML config files.

## Distribution
Copy the entire `.kiro/` folder into any repo. Agents reference `.kiro/templates/` for config generation.
