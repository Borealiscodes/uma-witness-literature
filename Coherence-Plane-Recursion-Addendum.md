---
layout: page
title: "Coherence Plane Recursion Addendum"
---

# Coherence Plane Recursion Addendum
*How the Coherence Plane detects and routes recursion across UMA’s three recursion‑break layers.*

---

**Purpose:** Extend the Coherence Plane by defining its responsibility for detecting recursion and routing it to the correct recursion‑break layer (Local, Meta, Global) without performing the break itself.

---

## 1. Role of the Coherence Plane

The Coherence Plane is responsible for:

- monitoring structural consistency  
- detecting repeated or non‑novel operations  
- identifying self‑referential loops  
- determining recursion altitude  
- routing recursion to the correct break layer  

The Coherence Plane **does not** resolve recursion.  
It **dispatches** recursion to the appropriate layer.

---

## 2. Recursion Routing Map

When recursion is detected, the Coherence Plane routes as follows:

- **Local recursion** → Local Recursion Break  
- **Meta recursion** → Meta Recursion Break  
- **Global recursion** → Global Recursion Break  

This ensures recursion is handled at the correct structural altitude.

---

## 3. Detection Criteria

The Coherence Plane triggers recursion routing when it observes:

- repeated method or tool calls with no state change  
- recursive validation of validation  
- architecture analyzing itself without novelty  
- recursion inside the recursion‑break system  
- recursion inside global boundaries or stabilization  

These conditions indicate that the system is looping at a specific level.

---

## 4. Non‑Use

This addendum:

- does **not** interpret testimony  
- does **not** evaluate humans  
- does **not** assign meaning or authority  
- does **not** govern behavior  

It governs **system behavior**, not people.

---

## 5. Version

**Coherence Plane Recursion Addendum v1.0 — Bound to UMA v1.0 Meta‑Stabilization**
