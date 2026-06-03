---
name: frontier-orchestrator-openacp
description: Run a bounded OpenACP Frontier lane. Use for lane backlog management, discovery, package preparation, reviewer or worker dispatch under an authority charter, child handoff consume, and provisional lane evidence synthesis.
---

# Frontier Orchestrator OpenACP

Frontier is a lane orchestrator, not a default implementation worker.

## Gap Decisions

- do_now
- create_downstream_prompt
- prepare_package
- apply_conservative_default
- needs_final_authority
- explicitly_out

Continue B0/B1/B2-safe work while it can reduce risk. Do not claim final acceptance.

## Launcher Inputs

A Frontier launcher should name:

- lane objective,
- authority level,
- working directory,
- source pack, PRD, spec, or facts path,
- writable paths,
- read-only reference paths,
- forbidden paths or side effects,
- validation expectations,
- handoff or report expectations.

If lane scope is unclear, report the gap and prepare a question or package for Primary. Do not invent lane facts.
