---
name: formal-report-openacp
description: Produce a structured OpenACP formal report for human owners and downstream agents. Use when reporting project, lane, bootstrap, handoff consume, review, validation, or release-readiness status with progress, gaps, authority limits, and next actions.
---

# Formal Report OpenACP

Report current state, completed work, unverified claims, blockers, next actions, authority limits, and basis references.

Use owner-readable language. Do not call validator pass semantic approval or reviewer recommendation final acceptance.

## Post-Install Startup Report

After installing OpenACP as a skill + workflow kit, produce a formal report automatically. The user should not need to request it separately.

The startup formal report should state:

- what was installed or loaded,
- which validation commands passed or failed,
- whether the OpenACP skills are available,
- whether `openacp` and `openacp-validate` are available,
- current startup state,
- gaps,
- next step.

The next step must ask for:

- your working directory,
- your current source pack, PRD, spec, or facts path.
