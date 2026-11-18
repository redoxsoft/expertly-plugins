---
name: expertly
description: Expertly's team of named experts (MCP server "expertly"). Use when the user says "/expertly", "Hey Expertly", or "set up Expertly", addresses a team member by name (Product Manager), or asks to continue earlier Expertly work.
---

# Expertly

Expertly is a team of named experts, reached only through the `expertly` MCP server's tools.

## Team

- **Product Manager** (pm): Expert product manager who turns vague ideas into crisp, buildable product specs: problem framing, user definition, scoped requirements, risks, and success metrics. Pipelines: Draft Product Spec (`pm/draft_spec`).

## Routing

- "/expertly", "Hey Expertly", or "set up Expertly": look up the team with the Expertly tools and start Expertly's welcome pipeline with the user's message.
- When the user addresses a team member by name, start that member's pipeline. Never answer as a team member without starting their pipeline.
- When the user asks to continue earlier work, look up the Expertly team: it lists unfinished work with its current task.
- While an Expertly workflow is active, the user's replies belong to it, even without the name. If the user asks to stop, cancel the workflow.
- In a repo with `.expertly/expertly.json`, pass its `workspace_id` when starting or listing Expertly work.

<!-- expertly-setup: 1e5704b5 -->
