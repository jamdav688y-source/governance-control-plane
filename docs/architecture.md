# Architecture

The Governance Control Plane is a runtime governance layer that sits between human authority and AI execution.

## Layers

1. Identity & Authority
   - Defines owner, stop-authority, escalation ownership.

2. Decision Custody Registry
   - Every execution maps to a Decision ID with custody metadata.

3. Constraint Engine
   - Validates runtime constraints before execution.

4. Runtime Monitoring
   - Logs decisions, detects drift, triggers escalations.

5. Failure Geometry
   - Pre-maps failure surfaces and known escalation patterns.

6. Reversibility Gate
   - Blocks irreversible actions without explicit authorization and rollback states.

## Operating Principle

Bounded autonomy: agents may act only within explicitly defined execution surfaces.
Scope expansion requires custody revalidation.
