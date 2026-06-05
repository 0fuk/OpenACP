# Primary Orchestrator Flow Example

This is a concept example for final-authority coordination.

Primary is the role that turns provisional evidence into a final decision. It can assign authority charters, dispatch a Frontier or scoped workers, consume handoffs and reviewer reports, and decide whether work is accepted, amended, rejected, waived, merged, or published.

This example intentionally does not make Primary a worker. The Primary reads evidence from other roles and records a final consume decision only when the basis is complete enough for the owner risk level.

Use:

- `primary-authority-charter.json` to see the B3 final-authority shape.
- `final-consume-status.json` to see how Primary reports that reviewed evidence is ready for, or blocked from, final acceptance.

Validate:

```bash
python tools/openaccp_validate.py --artifact examples/primary-orchestrator-flow/primary-authority-charter.json --ruleset authority-charter --strict
python tools/openaccp_validate.py --artifact examples/primary-orchestrator-flow/final-consume-status.json --ruleset status-report --strict
```
