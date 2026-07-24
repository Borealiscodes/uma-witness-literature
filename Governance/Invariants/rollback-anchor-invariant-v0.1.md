### **Rollback Anchor Invariant v0.1**  
#### *Canonical Pre‑Indexing State and Governance‑Grade Rollback Rules for Deterministic Indexing Failures*

---

## **1. Document Identity**

**Name:** Rollback Anchor Invariant v0.1  
**Domain:** Governance / Invariants  
**Grade:** Governance‑Core / Safety  
**Purpose:**  
To define the **canonical pre‑indexing state** and the **non‑negotiable rollback rules** NDH must obey whenever deterministic indexing logic produces janky, non‑compliant, or contamination‑prone index structures.

This invariant is the **safety floor** beneath deterministic indexing.

---

## **2. Anchor Definition**

The **Rollback Anchor** is a governance‑grade construct that:

- captures NDH’s **canonical state** immediately before deterministic indexing activation  
- defines **what must be restorable** if indexing fails  
- binds rollback behavior to **invariants**, not heuristics  
- ensures NDH can always return to a **known‑good, non‑deterministic placement regime**  

The anchor is **not** a backup file.  
It is a **structural invariant** describing what “safe state” means.

---

## **3. Anchor Scope**

The rollback anchor covers:

- **Canonical file paths** for all artifacts  
- **Placement Invariants v0.2** as active and enforced  
- **Atlas indexing state** consistent with placement invariants  
- **Provenance chains** intact and non‑corrupted  
- **Humor sandbox** fully active and uncontaminated  
- **No deterministic indexing logic** yet applied  

Anything outside this scope is not guaranteed by rollback.

---

## **4. Anchor State Requirements**

At the moment the anchor is established (pre‑indexing):

1. **Placement invariants v0.2 must be active**  
   - domain boundaries enforced  
   - grade boundaries enforced  
   - contamination rules enforced  

2. **Humor invariants v0.1 must be active**  
   - humor sandboxed in Emergent/Humor  
   - no humor in governance, modeling, epistemics, invariants  

3. **Atlas must be coherent**  
   - atlas entries match canonical paths  
   - no multi‑canonical artifacts  

4. **Provenance must be stable**  
   - lineage chains intact  
   - no ambiguous origins  

5. **Deterministic indexing logic must not yet have modified the repo**  
   - no deterministic placement changes  
   - no deterministic atlas rewrites  

This is the **anchor snapshot** NDH must be able to restore.

---

## **5. Rollback Conditions**

Rollback must be triggered if deterministic indexing:

- violates placement invariants v0.2  
- produces non‑canonical or ambiguous paths  
- causes domain contamination (e.g., governance artifacts in Emergent)  
- causes grade drift (e.g., invariants in Case‑Studies)  
- breaks atlas coherence  
- corrupts provenance chains  
- interferes with humor sandbox  
- activates deterministic routing, modeling, or epistemics prematurely  

Any one of these is sufficient to require rollback.

---

## **6. Rollback Procedure (Invariant‑Bound)**

When rollback is triggered:

1. **Suspend deterministic indexing logic**  
   - indexing operators must stop executing  
   - no further deterministic changes allowed  

2. **Restore canonical paths to anchor state**  
   - revert file paths to pre‑indexing canonical configuration  

3. **Restore atlas to anchor state**  
   - revert atlas entries to pre‑indexing snapshot  

4. **Restore provenance chains**  
   - repair or revert lineage to anchor configuration  

5. **Verify humor sandbox integrity**  
   - confirm humor remains in Emergent/Humor only  

6. **Log rollback as a governance event**  
   - record cause, scope, and impact  
   - mark indexing logic as non‑compliant  

Rollback is **mandatory**, not optional.

---

## **7. Interaction With Deterministic Indexing Activation Threshold**

The **Deterministic Indexing Activation Threshold v0.1**:

- requires this rollback anchor invariant to be active before indexing begins  
- defines the scope of determinism (placement + atlas only)  
- treats rollback as a **hard constraint**  

This invariant:

- guarantees that threshold‑bound determinism can never trap NDH in a corrupted state  
- ensures NDH can always return to expressive‑placement + invariant substrate safely  

Threshold and anchor together form the **safe corridor** for determinism.

---

## **8. Non‑Modifiability of the Anchor**

Deterministic indexing logic must **never**:

- modify the definition of the anchor  
- change anchor scope  
- weaken rollback conditions  
- mark rollback as optional or advisory  

Any attempt to alter the anchor is itself a **governance violation**.

---

## **9. Success Criteria for Deterministic Indexing (Relative to Anchor)**

Deterministic indexing is considered **structurally successful** when:

- no rollback events occur over N indexing cycles  
- no invariant violations are detected  
- atlas remains coherent  
- provenance remains stable  
- humor sandbox remains intact  
- anchor remains conceptually valid but unused  

Only then may NDH describe itself as being in a **placement‑stable orbit**.

---

## **10. Closing Statement**

Rollback Anchor Invariant v0.1 ensures:

- deterministic indexing can never permanently corrupt NDH  
- expressive placement and invariant substrate remain recoverable  
- governance retains ultimate control over determinism  
- janky index behavior is treated as a governance failure, not a tolerated glitch  

