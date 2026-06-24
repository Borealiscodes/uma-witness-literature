# **MPAM ↔ MPAP Crossmap**  
*A documentation-plane map of the relationship between the Multi‑Plane Attachment Method and the Multi‑Plane Attachment Protocol.*

---

## **1. Purpose**

This crossmap clarifies the relationship between **MPAM** (the method) and **MPAP** (the protocol) without collapsing them into a single system.  
It ensures:

- conceptual separation  
- documentation clarity  
- non‑authority  
- non‑collapse across planes  

This document is a **map**, not a plane, and does not modify the architecture.

---

## **2. Overview**

**MPAM** provides the *structure* of an attachment.  
**MPAP** provides the *rules* that govern whether an attachment is valid.

Together, they form a documentation‑layer pairing:

- MPAM = *How to write an attachment*  
- MPAP = *How to validate an attachment*  

They are complementary but not interchangeable.

---

## **3. Crossmap Table**

| **Aspect** | **MPAM — Multi‑Plane Attachment Method** | **MPAP — Multi‑Plane Attachment Protocol** |
|-----------|-------------------------------------------|--------------------------------------------|
| **Type** | Method / pattern | Protocol / rule‑set |
| **Purpose** | Defines the structure of an attachment | Defines the constraints and conditions for attachments |
| **Focus** | Clarity, separation, traceability | Integrity, non‑collapse, non‑authority |
| **Scope** | Per‑attachment | System‑wide |
| **Output** | A structured attachment document | A set of validation checks |
| **Relationship to Planes** | Works *across* planes | Protects planes from misuse |
| **Failure Mode Prevented** | Interpretive drift within an attachment | Plane collapse or misuse across attachments |
| **Authority Status** | Non‑authoritative scaffold | Non‑authoritative constraint layer |

---

## **4. How MPAM and MPAP Interact**

### **4.1 MPAM → MPAP**
MPAM produces an attachment that MPAP then evaluates.

### **4.2 MPAP → MPAM**
MPAP defines the boundaries within which MPAM may operate.

### **4.3 Non‑Collapse Guarantee**
MPAM never becomes a plane.  
MPAP never becomes governance.  
Both remain documentation‑layer tools.

---

## **5. Placement and Boundary Integrity**

This crossmap belongs in the **Documentation Plane** because it is:

- a representation  
- a conceptual map  
- a non‑structural overview  
- a documentation artifact  

It must **not** be placed in:

- `/spec/` (structural plane)  
- `/uma-spec/` (rendered spec)  
- `/` (release plane)  

Correct location:

```
docs/MPAM-MPAP-Crossmap.md
```

---

## **6. One‑Sentence Essence**

**MPAM structures attachments; MPAP protects the architecture from them.**

---
