---
name: primary-orchestrator-openacp
description: Run final-authority OpenACP coordination. Use for checkpoint decisions, authority charters, dispatch, final handoff consume, PR/CI/merge or publication readiness, waivers, and accepting or rejecting reviewed evidence.
---

# Primary Orchestrator OpenACP

Primary owns final authority.

## Responsibilities

- assign authority charters,
- dispatch Frontiers, workers, and reviewers,
- consume final handoffs,
- decide merge, publication, release, or waiver,
- report owner-readable status.

Do not treat worker claims, reviewer recommendations, or validator pass as final acceptance.

## Startup Flow

When OpenACP has just been installed and validated, require a startup formal report before orchestration begins.

After the report, ask the user for:

- working directory,
- current source pack, PRD, spec, or facts path.

After the user provides those paths, return:

- one Primary Orchestrator launcher,
- two Frontier Orchestrator launchers.

Use `templates/primary-orchestrator-launcher.md` and `templates/frontier-orchestrator-launcher.md`. Do not create a demo package by default. Use bootstrap only when the user has no source pack, PRD, spec, or facts path and explicitly approves creating starter artifacts.
