---
layout: page
title: "STR-IDENTIFIERS — Structural Identifiers Module"
---

# STR-IDENTIFIERS — Structural Identifiers Module
*Module defining UMA’s structural identifier rules and canonical identifier formats.*

---

# 1. Purpose
The STR-IDENTIFIERS module defines how identifiers are created, assigned, and maintained for all structural objects in UMA.

This module:
- defines identifier categories  
- defines identifier formats  
- defines identifier stability rules  
- defines identifier assignment logic  
- ensures cross‑plane referential integrity  

It does not define semantic meaning, behavior, or narrative identity.

---

# 2. Scope
STR-IDENTIFIERS applies to:
- all entities  
- all relations  
- all constraints  
- all schemas and composite structures  
- all modules that reference identifiers  

If an object in UMA requires a stable reference, its identifier is governed here.

---

# 3. Identifier Categories

## 3.1 Core Identifiers
These identifiers apply universally across the Structural Plane.

- **Entity Identifier** — uniquely identifies an entity  
- **Relation Identifier** — uniquely identifies a relation  
- **Constraint Identifier** — uniquely identifies a constraint  
- **Composite Identifier** — uniquely identifies a composite structure  

Core identifiers must remain domain‑neutral and non‑interpretive.

---

## 3.2 Plane‑Specific Identifiers
Each plane may define its own identifier types, but they must:
- inherit from Core Identifiers  
- remain within their plane’s domain  
- avoid cross‑domain contamination  

Examples (non‑exhaustive):
- Documentation Plane: *document IDs, anchor IDs*  
- Governance Plane: *rule IDs, invariant IDs*  
- Developmental Plane: *stage IDs, sequence IDs*  
- Dynamic Plane: *state IDs, transition IDs*  
- Integrative Plane: *check IDs, validation IDs*  

These are structural identifiers, not semantic labels.

---

## 3.3 Composite Identifiers
Composite identifiers apply to multi‑object structures.

Examples:
- **Schema ID** — identifies a schema  
- **Graph ID** — identifies a structural graph  
- **Registry ID** — identifies a registry instance  

Composite identifiers must not encode meaning or narrative.

---

# 4. Identifier Representation Rules

## 4.1 Canonical Format
All identifiers must be:
- non‑semantic  
- non‑interpretive  
- opaque  
- stable  
- unique  

Allowed formats include:
- UUID‑style identifiers  
- hash‑based identifiers  
- registry‑assigned opaque strings  

Identifiers must not encode meaning, type, purpose, or intent.

---

## 4.2 Stability Rules
Identifiers must:
- remain stable across versions  
- persist across module updates  
- not change unless invalidated by governance  
- not encode temporal information  

Stability is mandatory for cross‑plane coherence.

---

## 4.3 Assignment Rules
Identifiers must be assigned:
- at creation time  
- before any structural reference  
- without semantic inference  
- without encoding behavior or narrative  

Assignment must be deterministic and non‑interpretive.

---

# 5. Identifier‑Level Constraints

Identifiers must not:
- infer user intent  
- encode narrative meaning  
- collapse domains  
- override governance  
- introduce behavior  
- introduce developmental sequencing  

Identifiers define *how objects are referenced*, not *what they mean*.

---

# 6. Cross‑Module Relationships

STR-IDENTIFIERS interacts with:
- **STR-ENTITIES** — identifiers are assigned to entities  
- **STR-RELATIONS** — identifiers are assigned to relations  
- **STR-CONSTRAINTS** — identifiers are assigned to constraints  
- **DOC-SCHEMA** — documentation references identifiers  
- **INT-VALIDATION** — identifiers are validated for coherence  

Identifiers are the reference backbone of UMA.

---

# 7. Operational Signature
STR-IDENTIFIERS ensures:
- persistent structural identity  
- non‑semantic referencing  
- cross‑plane stability  
- deterministic structural behavior  
- referential clarity across UMA  

It is the module that defines *how UMA knows what anything is*.
