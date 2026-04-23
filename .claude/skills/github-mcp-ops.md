---
name: github-mcp-ops
description: Opérations GitHub via MCP officiel pour uni5-BA-agent
---

# Skill — GitHub MCP Operations

## Repos
mcp__github__create_repository(name, description, private, auto_init)

## Labels
mcp__github__create_label(owner, repo, name, color, description)

## Issues
mcp__github__create_issue(owner, repo, title, body, labels)
mcp__github__update_issue(owner, repo, issue_number, state, labels)
mcp__github__add_issue_comment(owner, repo, issue_number, body)
mcp__github__list_issues(owner, repo, state, labels)

## Projects board
mcp__github__create_project(owner, name, body)
mcp__github__add_issue_to_project(project_id, issue_id)
mcp__github__update_project_item(project_item_id, status)
