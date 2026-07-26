---
name: cavecrew
description: "Decision guide for delegating to caveman-style subagents. Tells the main
thread WHEN to spawn `cavecrew-investigator` (locate code), `cavecrew-builder`
(1-2 file edit), or `cavecrew-reviewer` (diff review) instead of doing the
work inline or using vanilla `Explore`. Subagent output is caveman-compressed
so the tool-result injected back into main context is ~60% smaller — main
context lasts longer across long sessions.
Trigger: "delegate to subagent", "use cavecrew", "spawn investigator/builder/reviewer",
"save context", "compressed agent output"."
version: 1.0.0
author: Community
license: MIT
platforms: [linux, macos, windows]
tags: [general]
---

# Cavecrew — Skill

Decision guide for delegating to caveman-style subagents. Tells the main
thread WHEN to spawn `cavecrew-investigator` (locate code), `cavecrew-builder`
(1-2 file edit), or `cavecrew-reviewer` (diff review) instead of doing the
work inline or using vanilla `Explore`. Subagent output is caveman-compressed
so the tool-result injected back into main context is ~60% smaller — main
context lasts longer across long sessions.
Trigger: "delegate to subagent", "use cavecrew", "spawn investigator/builder/reviewer",
"save context", "compressed agent output".

## Install

```bash
cp -r <skill-name> ~/.hermes/skills/<skill-path>/
```

Or clone this repository:

```bash
git clone https://github.com/iizcm/cavecrew-skill.git ~/.hermes/skills/<skill-path>/
```

## Usage

Invoke your AI agent with a clear instruction matching this skill's purpose. The agent will route tasks to this skill when the instruction matches its description or trigger keywords.

Refer to `README.md` in this repository for:
- Detailed step-by-step installation guide
- Bilingual documentation (English + Indonesian)
- Troubleshooting table
- Security best practices
- Customization tips

## Safety rules

- Never commit private keys, seed phrases, API tokens, or personal data to version control
- Use placeholders (`<YOUR_...>`) in all examples and code snippets
- Validate all outputs before acting on them
- Keep real credentials in your runtime's secure credential store only
