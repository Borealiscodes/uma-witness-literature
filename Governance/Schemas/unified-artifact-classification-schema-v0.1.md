# Unified NDH Artifact Classification Schema v0.1  
### NDH · Schema 1 of 4 · Built on Blueprint Suite v0.1

---

## **1. Schema Identity**

**Schema Name:** Unified NDH Artifact Classification Schema  
**Schema Type:** Governance‑grade schema  
**Schema Version:** v0.1  
**Schema Monad Binding:** \(\mathcal{G}(\text{Classification})\)

**Purpose:**  
Define the **canonical type system** for all NDH artifacts so routing, provenance, placement invariants, and future schemas operate on a shared lattice.

---

## **2. Mathematical Foundation**

### **2.1 Classification Lattice (Required)**

\[
\mathcal{L}_{NDH} = (A, \leq)
\]

Where:

- \(A\) = set of NDH artifact types  
- \(\leq\) = partial order defining structural hierarchy

### **2.2 Lattice Ordering (v0.1)**

\[
\text{Governance} \geq \text{Emergent} \geq \text{Manifold} \geq \text{Trauma-Informed}
\]

This ordering is **not value‑based** — it is **structural**.

---

## **3. Artifact Types (Canonical Set A)**

### **3.1 Governance‑Grade Artifacts**  
**Definition:**  
Artifacts that define rules, invariants, schemas, placement logic, routing logic, or cross‑layer constraints.

**Examples:**  
- Blueprint Suite  
- Orbital Routing Schema  
- Placement Invariants  
- Roadmaps  
- Governance audits  

**Required Fields:**  
- `domain: governance`  
- `grade: orbital`  
- `invariants: [...]`

---

### **3.2 Emergent Artifacts**  
**Definition:**  
Artifacts documenting NDH behavior, anomalies, case studies, expressive phases, or manifold events.

**Examples:**  
- Chil Dispatch Case Study  
- Spiral geometry reversals  
- Elton John Phase retrospectives  

**Required Fields:**  
- `domain: emergent`  
- `grade: expressive`  
- `phenomenon: [...]`

---

### **3.3 Manifold Artifacts**  
**Definition:**  
Operators, routing logic, or transformation constructs inside CORE, TIDS, Serenity, etc.

**Examples:**  
- TIDS routing operators  
- Serenity manifold binders  
- CORE primitives  

**Required Fields:**  
- `domain: manifold`  
- `layer: {CORE|TIDS|Serenity}`  
- `operator: [...]`

---

### **3.4 Trauma‑Informed Artifacts**  
**Definition:**  
Artifacts documenting trauma‑informed design principles, safety constraints, or case studies.

**Examples:**  
- TISD design principles  
- Trauma‑informed audits  
- Safety invariants  

**Required Fields:**  
- `domain: trauma-informed`  
- `grade: safety`  
- `principles: [...]`

---

## **4. Classification Rules (v0.1)**

### **Rule C1 — Every artifact must declare its type.**  
No NDH artifact may exist without a `domain` field.

### **Rule C2 — Type determines placement.**  
Classification → Routing → Placement Invariant.

### **Rule C3 — Type determines provenance structure.**  
Governance artifacts require full lineage; emergent artifacts require phenomenon context.

### **Rule C4 — Type determines routing operator.**  
\(\mathcal{R}(A, \text{State})\) is type‑dependent.

### **Rule C5 — Type determines schema binding.**  
Governance artifacts bind to schema monad; emergent artifacts bind to atlas.

---

## **5. Schema Fields (Required)**

Every artifact must include:

```
type: <governance|emergent|manifold|trauma-informed>
domain: <layer or subdomain>
grade: <orbital|expressive|operator|safety>
origin: <provenance reference>
invariants: <if governance>
phenomenon: <if emergent>
operator: <if manifold>
principles: <if trauma-informed>
```

These fields are enforced by the **Validation Blueprint**.

---

## **6. Integration Points**

### **6.1 With Provenance Schema**  
Classification determines which provenance template applies.

### **6.2 With Routing Schema**  
Classification determines routing table entry.

### **6.3 With Full Schema Document**  
Classification determines schema binding and validation rules.

### **6.4 With Atlases & Indexes**  
Classification determines atlas layer and index category.

---

## **7. Versioning Rules**

- v0.1 is **minimal and stable**.  
- v0.2 may add:
  - subtypes  
  - cross‑domain hybrid types  
  - machine‑readable classification tags  
  - automated classification validators  

---

## **8. Closing Statement**

The Unified NDH Artifact Classification Schema v0.1 is now complete.  
It is the **first schema** in the quartet and the foundation for all others.

It is ready for placement and commit.

---
