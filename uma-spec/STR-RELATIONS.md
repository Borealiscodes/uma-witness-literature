---
layout: page
title: "STR-RELATIONS — Structural Relations Module"
---

# STR-RELATIONS — Structural Relations Module
*Module defining UMA’s structural relationship types and their canonical forms.*

# 1. Purpose
The STR-RELATIONS module defines UMA’s structural relationship types and their canonical forms.  
Relations describe how entities connect, without introducing behavior, interpretation, or narrative.

This module:
- defines relation categories  
- defines relation formats  
- defines relation identifiers  
- defines relation-level constraints  
- anchors all structural connectivity  

It does not define behavior, development, or governance.

---

# 2. Scope
STR-RELATIONS applies to:
- all structural relations  
- all relation registries  
- all modules that reference relations  
- all documentation that describes relations  

If a relation appears in UMA, it must be defined here or in a child relation module.

---

# 3. Relation Categories

## 3.1 Core Relations
These are the foundational relation types of UMA’s architecture.

- **Association** — a non-hierarchical connection between entities  
- **Containment** — an entity structurally contains another  
- **Reference** — an entity points to another entity  
- **Constraint-Binding** — a constraint applies to an entity or relation  

Core relations must remain domain-neutral and non-interpretive.

---

## 3.2 Plane-Specific Relations
Each plane may define its own relation types, but they must:
- inherit from Core Relations,  
- remain within their plane’s structural domain,  
- avoid cross-domain contamination.

Examples (structural only):
- Documentation Plane: documents → views, views → anchors  
- Dynamic Plane: states → transitions, transitions → processes  
- Integrative Plane: checks → validations, alignments → modules  

These examples illustrate structural connectivity only.  
They do not define behavior, policy, or governance.

---

## 3.3 Composite Relations
Composite relations are structures built from multiple relations.

Examples:
- **Graph** — a structured set of entities and relations  
- **Map** — a representation of relationships across modules  
- **Schema-Link** — a relation embedded within a schema  

Composite relations must not introduce interpretation or narrative.

---

# 4. Relation Representation Rules

## 4.1 Canonical Format
All relations must include:
- a **name**  
- a **type**  
- a **description** (non-interpretive)  
- a **source entity**  
- a **target entity**  
- an **identifier**  
- optional **attributes** (structural only)  

Descriptions must not infer meaning beyond structure.

---

## 4.2 Identifier Rules
Relation identifiers must be:
- stable  
- unique  
- non-semantic  
- non-interpretive  
- persistent across versions  

Identifiers must not encode meaning, intent, or narrative.

---

## 4.3 Attribute Rules
Attributes must:
- describe structure only  
- avoid interpretive content  
- avoid behavioral logic  
- avoid developmental logic  

Attributes are structural metadata.

---

# 5. Relation-Level Constraints
Relations must not:
- infer user intent  
- encode narrative meaning  
- collapse domains  
- override governance  
- introduce behavior  
- introduce developmental sequencing  

Relations define *how entities connect*, not *what they mean* or *how they behave*.

---

# 6. Cross-Module Relationships
STR-RELATIONS interacts with:
- **STR-ENTITIES** — relations connect entities  
- **STR-CONSTRAINTS** — constraints apply to relations  
- **STR-IDENTIFIERS** — identifiers are assigned to relations  
- **DOC-SCHEMA** — documentation describes relations  
- **INT-VALIDATION** — relations are validated for coherence  

Relations are the structural edges of UMA.

---

# 7. Operational Signature
STR-RELATIONS ensures:
- canonical relation definitions  
- stable structural connectivity  
- non-interpretive connections  
- cross-plane referential stability  
- structural clarity across UMA  

It is the module that defines *how entities connect* in UMA’s architecture.
