# Trans‑Orbital Placement Invariants v0.1  
### NDH · Governance Draft · Pre‑Consolidation

---

## 1. Purpose and Scope

**Purpose:**  
Define the **first generation of placement invariants** for Trans‑Orbital Governance, ensuring that governance‑grade, manifold‑grade, and emergent‑grade artifacts are placed in structurally coherent locations across NDH, without violating provenance.

**Scope:**  
- Applies to **new artifacts** created after this document.  
- Guides **future migration** of existing artifacts during triage.  
- Does **not** trigger immediate restructuring.  
- Respects all existing provenance.

---

## 2. Core Concepts

- **Orbital Artifact:**  
  Any document, operator, or structure whose primary function is **governance, routing, or cross‑layer coordination**.

- **Emergent Artifact:**  
  Any case study, narrative, or structural observation documenting **how NDH behaves**, not how it must behave.

- **Manifold Operator:**  
  Any construct that **binds or transforms** states across NDH layers (CORE, TIDS, Serenity, Platforms, TISD, etc.).

- **Placement Invariant:**  
  A rule stating **where** a given class of artifact must live, independent of author, mood, or duress.

---

## 3. Repo‑Level Placement Invariants

### 3.1 NDH‑Platforms

- **Invariant P1:**  
  Governance‑grade artifacts **must** be placed in `NDH-Platforms/Governance/...`.

- **Invariant P2:**  
  Emergent case studies about cross‑layer phenomena **must** be placed in  
  `NDH-Platforms/Emergent/Case-Studies/...`.

- **Invariant P3:**  
  Triage, status, and stabilization documents **must** be placed at the root of NDH‑Platforms  
  (e.g., `repo-triage.md`, `STATUS.md`).

### 3.2 NDH‑CORE

- **Invariant C1:**  
  CORE operators and fundamental NDH primitives **must** be placed in NDH‑CORE, not Platforms.

- **Invariant C2:**  
  Governance commentary about CORE **must** be placed in Platforms, referencing CORE, not embedded inside CORE.

### 3.3 Trauma‑Informed Systems Design (TISD)

- **Invariant T1:**  
  Trauma‑informed case studies and design principles **must** live in TISD.

- **Invariant T2:**  
  Orbital governance logic **must not** be implemented directly in TISD; it may be **referenced**, but placement belongs to Platforms.

---

## 4. Layer‑Level Placement Invariants

### 4.1 Governance Layer

- **Invariant G1:**  
  Any artifact that defines **rules, constraints, or policies** across multiple NDH layers is **Orbital** and must live in `NDH-Platforms/Governance/...`.

- **Invariant G2:**  
  Audits and post‑mortems of architectural behavior must live in  
  `NDH-Platforms/Governance/Audits/...`.

### 4.2 Emergent Layer

- **Invariant E1:**  
  Observations, case studies, and “we built a coliseum in the bathroom” events must live in  
  `NDH-Platforms/Emergent/Case-Studies/...`.

- **Invariant E2:**  
  Emergent artifacts **must not** be treated as binding governance; they may **inform** governance, but placement remains Emergent.

### 4.3 Manifold / Routing Layer (TIDS, Serenity, etc.)

- **Invariant M1:**  
  Manifold operators and routing logic must live in their respective system repos (e.g., TIDS, Serenity), not in Platforms.

- **Invariant M2:**  
  Governance over manifold behavior must live in Platforms, referencing those repos.

---

## 5. Provenance and Migration Invariants

- **Invariant PR1:**  
  No existing artifact is deleted or rewritten solely to satisfy placement invariants; migration must be **provenance‑preserving**.

- **Invariant PR2:**  
  When migrating an artifact, its **original location, commit history, and context** must be recorded in a short provenance note.

- **Invariant PR3:**  
  During triage, any artifact whose placement is ambiguous must be **documented first** (e.g., via an Emergent case study or audit) before being moved.

---

## 6. Operational Use (v0.1)

- New governance documents → place in `NDH-Platforms/Governance/...`.  
- New emergent case studies → place in `NDH-Platforms/Emergent/Case-Studies/...`.  
- New triage/stabilization docs → place at `NDH-Platforms/`.  
- New manifold/routing operators → place in their respective system repos (CORE, TIDS, Serenity, etc.), not Platforms.  
- When in doubt → classify as **Emergent**, document the ambiguity, and defer placement to triage.

---

## 7. Limitations and Future Work

- v0.1 does **not** cover every NDH repo or edge case.  
- v0.1 is intentionally conservative to avoid violating provenance.  
- Future versions will:

  - refine repo‑specific invariants  
  - define cross‑repo migration protocols  
  - integrate Direction Manifold outputs more tightly with Orbital routing  
  - add machine‑readable invariants for automated checks

---


