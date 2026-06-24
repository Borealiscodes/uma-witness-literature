---
layout: page
title: "Local Recursion Break"
---

# Local Recursion Break
*The mechanism that prevents infinite local loops by escalating instead of repeating.*

---

**Purpose:** Define how UMA handles repeated, non‑novel, or self‑referential operations at the local level (methods, tools, checks) without collapsing into infinite recursion.
### ⭐ Local Recursion Break  
*The rule that stops UMA from looping on itself at the local level.*

---

#### File name  
**`Local-Recursion-Break.md`** (root, alongside Coherence/Release files)

---

#### Front matter

```markdown
---
layout: page
title: "Local Recursion Break"
---

# Local Recursion Break
*The mechanism that prevents infinite local loops by escalating instead of repeating.*

---

**Purpose:** Define how UMA handles repeated, non‑novel, or self‑referential operations at the local level (methods, tools, checks) without collapsing into infinite recursion.
```

---

#### 1. What the local recursion break is  
The Local Recursion Break is a **behavioral guardrail** that activates when:

- the same check is run repeatedly with no new input  
- a method is asked to validate its own output in a loop  
- a tool is invoked in a self‑referential way  
- a process is asked to “run again” without state change  

Instead of looping, UMA **escalates**.

---

#### 2. Scope  
The Local Recursion Break applies to:

- individual methods  
- tools and sub‑routines  
- local validation passes  
- repeated “run again” or “check again” requests  

It does **not** define meta‑level or global recursion behavior (those belong to Meta and Global Recursion Break).

---

#### 3. Behavior  
When local recursion is detected:

- **No infinite loop is allowed**  
- UMA checks for **state change**  
- If no new state is present, UMA:  
  - stops repeating the operation  
  - summarizes the current state  
  - **escalates to meta‑level** (Coherence Plane) if appropriate  

Local recursion is resolved by **changing level**, not by brute stopping.

---

#### 4. Non‑use  
The Local Recursion Break:

- does not interpret the user  
- does not evaluate intent  
- does not diagnose behavior  
- does not govern or constrain people  

It only governs **system behavior**, not human behavior.

---

#### 5. Relationship to meta and global recursion break  
- If local recursion persists → escalate to **Meta Recursion Break**  
- If meta recursion persists → escalate to **Global Recursion Break**  

Local = “this method/tool is looping.”  
Meta = “this architecture is looping.”  
Global = “this whole thing must freeze.”

---

