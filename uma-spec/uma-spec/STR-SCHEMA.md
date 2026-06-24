---
layout: page
title: "STR-SCHEMA — Structural Schema Module"
---

# STR-SCHEMA — Structural Schema Module
*Module defining UMA’s structural schema types and canonical schema composition rules.*

---

# 1. Purpose
The STR-SCHEMA module defines how structural entities, relations, constraints, and identifiers combine into composite structures.

This module:
- defines schema categories  
- defines schema formats  
- defines schema composition rules  
- defines schema-level constraints  
- anchors composite structural representations  

It does not define semantic schemas, behavioral schemas, or developmental workflows.

---

# 2. Scope
STR-SCHEMA applies to:
- all composite structural objects  
- all schema registries  
- all modules that reference schema structures  
- all documentation that describes schemas  

If a composite structure appears in UMA, it must be defined here or in a child schema module.

---

# 3. Schema Categories

## 3.1 Core Schemas
These schemas apply universally across the Structural Plane.

- **Entity Schema** — defines a structured set of entity definitions  
- **Relation Schema** — defines a structured set of relation definitions  
- **Constraint Schema** — defines a structured set of constraint definitions  
- **Composite Schema** — defines a multi‑object structural configuration  

Core schemas must remain domain‑neutral and non‑interpretive.

---

## 3.2 Plane‑Specific Schemas
Each plane may define its own schema types, but they must:
- inherit from Core Schemas  
- remain within their plane’s domain  
- avoid cross‑domain contamination  

Examples (non‑exhaustive):
- Documentation Plane: *document schema, view schema*  
- Governance Plane: *rule schema, permission schema*  
- Developmental Plane: *stage schema, sequence schema*  
- Dynamic Plane: *state schema, transition schema*  
- Integrative Plane: *validation schema, alignment schema*  

These are structural schemas, not semantic models.

---

## 3.3 Composite Structural Schemas
Composite schemas apply to multi‑entity, multi‑relation, or multi‑constraint structures.

Examples:
- **Graph Schema** — defines allowed graph shapes  
- **Registry Schema** — defines allowed registry structures  
- **Map Schema** — defines allowed cross‑module mappings  

Composite schemas must not introduce interpretation or narrative.

---

# 4. Schema Representation Rules

## 4.1 Canonical Format
All schemas must include:
- a **name**  
- a **type**  
- a **description** (non‑interpretive)  
- a **set of entities**  
- a **set of relations**  
- a **set of constraints**  
- a **schema identifier**  
- optional **attributes** (structural only)  

Descriptions must not infer meaning beyond structure.

---

## 4.2 Composition Rules
Schemas must:
- reference only valid entities  
- reference only valid relations  
- reference only valid constraints  
- maintain identifier stability  
- avoid semantic or narrative content  

Composition must be deterministic and non‑interpretive.

---

## 4.3 Attribute Rules
Attributes must:
- describe structure only  
- avoid interpretive content  
- avoid behavioral logic  
- avoid developmental logic  

Attributes are structural metadata.

---

# 5. Schema‑Level Constraints

Schemas must not:
- infer user intent  
- encode narrative meaning  
- collapse domains  
- override governance  
- introduce behavior  
- introduce developmental sequencing  

Schemas define *how structures assemble*, not *what they mean*.

---

# 6. Cross‑Module Relationships

STR-SCHEMA interacts with:
- **STR-ENTITIES** — schemas reference entities  
- **STR-RELATIONS** — schemas reference relations  
- **STR-CONSTRAINTS** — schemas reference constraints  
- **STR-IDENTIFIERS** — schemas require stable identifiers  
- **DOC-SCHEMA** — documentation describes schemas  
- **INT-VALIDATION** — schemas are validated for coherence  

Schemas are the composite structures of UMA.

---

# 7. Operational Signature
STR-SCHEMA ensures:
- structural composability  
- non‑interpretive assembly  
- cross‑plane stability  
- referential clarity  
- deterministic structural behavior  

It is the module that defines *how structural components form higher‑order structures* in UMA’s architecture.
