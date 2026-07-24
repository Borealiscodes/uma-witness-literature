# Provenance Schema v0.1  
### NDH · Schema 2 of 4 · Lineage Preservation Substrate

---

## **1. Schema Identity**

**Schema Name:** Provenance Schema  
**Schema Version:** v0.1  
**Schema Type:** Governance‑grade schema  
**Schema Monad Binding:** \(\mathcal{G}(\text{Provenance})\)

**Purpose:**  
Define how NDH artifacts record, preserve, and expose their **lineage**, ensuring that all migrations, placements, and transformations remain fully traceable across repos, layers, and governance phases.

This schema ensures NDH never loses its history.

---

## **2. Mathematical Foundation**

### **2.1 Provenance Functor (Required)**

\[
\mathcal{P}: A \rightarrow \text{Lineage}
\]

Where:

- \(A\) = artifact type (from classification schema)  
- \(\text{Lineage}\) = structured provenance record

**Interpretation:**  
Every artifact type maps to a lineage structure appropriate for its domain.

### **2.2 Provenance Composition Law**

\[
\mathcal{P}(x \rightarrow y) = \mathcal{P}(x) \cup \mathcal{P}(y)
\]

Any migration merges provenance sets.

### **2.3 Provenance Invariant**

\[
\forall x, \; \mathcal{P}(x) \neq \emptyset
\]

No artifact may exist without provenance.

---

## **3. Provenance Record Structure (v0.1)**

Every NDH artifact must contain the following fields:

```
origin:
  author: <string>
  context: <string>
  timestamp: <ISO-8601>
  initial_location: <repo/layer>

lineage:
  migrations: [ ... ]
  placement_decisions: [ ... ]
  invariant_references: [ ... ]

current_state:
  location: <repo/layer>
  classification: <type>
  routing_source: <operator>
```

### **3.1 Origin Block**

Defines the artifact’s birth conditions:

- **author** — human or system origin  
- **context** — why it was created  
- **timestamp** — creation time  
- **initial_location** — first repo/layer placement

### **3.2 Lineage Block**

Tracks everything that happens after origin:

- **migrations** — every move across repos/layers  
- **placement_decisions** — why each move occurred  
- **invariant_references** — which governance rules applied

### **3.3 Current State Block**

Tracks the artifact’s present condition:

- **location** — current repo/layer  
- **classification** — governance/emergent/manifold/trauma  
- **routing_source** — which routing operator placed it here

---

## **4. Provenance Rules (v0.1)**

### **Rule P1 — Provenance is mandatory.**  
No artifact may exist without a provenance block.

### **Rule P2 — Provenance must be updated on every migration.**  
Every move must append a new lineage entry.

### **Rule P3 — Provenance must reference invariants.**  
Placement decisions must cite the invariants that justified them.

### **Rule P4 — Provenance must be readable.**  
Direction Manifold requires clarity and narrative coherence.

### **Rule P5 — Provenance must be preserved.**  
No provenance entry may be deleted or rewritten.

### **Rule P6 — Provenance determines routing eligibility.**  
Routing operators check provenance before moving artifacts.

---

## **5. Provenance Templates (v0.1)**

### **5.1 Governance Artifact Provenance Template**

Governance artifacts require:

- full lineage  
- invariant references  
- routing justification  
- placement audit trail

### **5.2 Emergent Artifact Provenance Template**

Emergent artifacts require:

- phenomenon context  
- expressive origin notes  
- stabilization references  
- case study linkage

### **5.3 Manifold Artifact Provenance Template**

Manifold artifacts require:

- operator lineage  
- transformation history  
- layer‑binding notes  
- routing operator references

### **5.4 Trauma‑Informed Artifact Provenance Template**

Trauma‑informed artifacts require:

- safety context  
- principle references  
- audit lineage  
- sensitivity notes

---

## **6. Integration Points**

### **6.1 With Classification Schema**  
Classification determines which provenance template applies.

### **6.2 With Routing Schema**  
Routing operators require provenance to determine legal moves.

### **6.3 With Full Schema Document**  
Provenance defines schema binding and validation rules.

### **6.4 With Atlases & Indexes**  
Provenance entries populate the **Provenance Index** and **Lineage Hyperatlas**.

---

## **7. Versioning Rules**

- v0.1 is minimal and stable.  
- v0.2 may add:
  - machine‑readable provenance tags  
  - automated lineage validators  
  - cross‑repo provenance diff tools  
  - provenance compression (non‑destructive)

---

## **8. Closing Statement**

Provenance Schema v0.1 is now complete.  
It is the **second schema** in the quartet and the foundation for routing and full schema binding.

It is ready for placement and commit.

---


