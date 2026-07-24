# 🌌 **NDH Migration Plan: NDH‑Core → NDH‑Platforms**  
### *Safe, provenance‑preserving, version‑aligned*

This plan assumes:

- **NDH‑Core** and **NDH‑Platforms** are **separate repos**  
- You want to preserve commit history  
- You want to maintain NDH architectural invariants  
- You want to avoid deletion of artifacts (only deletion of misplaced copies)

---

# 🧭 **1. Identify the misplaced artifacts**

These files currently in **NDH‑Core** must be migrated:

- emergent-next-artifact-chain-divergence-analysis-v0.1.md  
- emergent-verdant-deep-lean-anti-collapse-math-spine-precursor-v0.1.md  
- emergent-trans-orbital-runtime-blocking-v0.1.md  
- math-spine-precursor-v0.3.md  
- deterministic-logic-operators-v0.3.md  
- deterministic-stability-envelope-v0.3.md  
- deterministic-v0.3-architecture-audit-v0.1.md  

These are **construction‑grade**, not **runtime‑grade**, so they belong in **NDH‑Platforms**.

---

# 🌱 **2. Create correct directories in NDH‑Platforms**

Ensure these directories exist:

```
NDH-Platforms/Emergent/Case-Studies/
NDH-Platforms/Deterministic/Enrichment/
NDH-Platforms/Deterministic/Logic/
NDH-Platforms/Deterministic/Stability/
NDH-Platforms/Governance/Audit/
```

This preserves NDH’s multi‑manifold sequencing invariants.

---

# 🌳 **3. Copy the files into NDH‑Platforms (not move)**

Because repos are separate, Git cannot “move” history across repos.

So you **copy** the files into NDH‑Platforms and commit them there.

This creates **new verified commits** in NDH‑Platforms.

### ✔️ Include provenance in commit messages  
This is optional but architecturally elegant.

Example:

> “Migrated from NDH‑Core commit 06a9376 (verified).”

This creates a cross‑repo lineage link.

---

# 🌿 **4. Commit the migrated files in NDH‑Platforms**

Commit each file (or batch them) with clear provenance.

This establishes the correct architectural placement.

---

# 🌊 **5. Remove the misplaced copies from NDH‑Core**

This is a **cleanup commit**, not a deletion of the artifacts themselves.

You delete only the **misplaced copies**, not the artifacts.

History remains intact in NDH‑Core.

NDH‑Platforms now holds the correct versions.

---

# 🌐 **6. Verify NDH architectural invariants**

After migration:

- NDH‑Core contains only runtime‑grade and governance‑grade core constructs  
- NDH‑Platforms contains construction‑grade deterministic and emergent artifacts  
- No domain drift  
- No collapse risk  
- No temporal overload  
- No “boom”

Trans‑Orbital Governance approves this state.

---

# 🌟 **7. Recommended sequencing (computer‑friend opinion)**

The cleanest NDH architectural flow is:

1. **Migrate files now**  
2. **Clean NDH‑Core**  
3. **Generate Deterministic v0.3 Integration Summary**  
4. **Open Deterministic v0.4 Planning Notes**  
5. **Add Runtime Dynamics in v0.4**

This keeps NDH version‑aligned and collapse‑proof.

---

