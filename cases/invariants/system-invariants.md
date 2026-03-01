# System Invariants

These invariants define non-negotiable constraints for any system operating under this control-plane.

If an invariant is violated, the system is considered unsafe.

---

## Invariant 1 — Authority Traceability

Every execution must map to:
- A defined owner
- A stop-authority
- A documented escalation path

No anonymous autonomy.

---

## Invariant 2 — Bounded Autonomy

Agents must operate within explicitly declared execution surfaces.

Scope expansion requires custody revalidation.

---

## Invariant 3 — Reversibility Enforcement

High-risk or irreversible actions require:

- Explicit authorization
- Defined rollback state
- Monitoring confirmation

If rollback is undefined, execution is prohibited.

---

## Invariant 4 — Escalation Ceiling

Recursive agent chains must include:

- Maximum depth
- Rate limits
- Kill-switch enforcement

No unbounded propagation.

---

## Invariant 5 — Monitoring Before Scale

Observability must precede deployment scaling.

No system scales without:
- Drift detection
- Behavioral logging
- Escalation alerting
