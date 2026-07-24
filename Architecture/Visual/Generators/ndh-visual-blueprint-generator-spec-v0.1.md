# NDH Visual Blueprint Generator Spec v0.1

## 1. Purpose

The NDH Visual Blueprint Generator converts **ASCII blueprints** into **SVG/PNG diagrams** for NDH’s visual architecture suite.

It is grounded in:

- NDH Visual Roadmap Generation Model v1.0  
- Blueprint Suite  
- Trauma-Informed Design Systems (TIDS)  

Goal: make visual artifacts **gentle to author**, **rigorous in structure**, and **easy to render**.

---

## 2. Inputs

### 2.1 ASCII Blueprint Files

- Plain text, `.ndhbp` or `.txt`
- Contain diagram definitions using a small DSL:

Examples:

```text
DIAGRAM linear-roadmap-v1
NODE MathSpine "Math Spine Foundation"
NODE Sneks "SNEK Runtime Operators"
NODE Ecosystem "Ecosystem Envelope"
NODE Accessibility "Accessibility Kawaii Layer"
NODE Governance "Trans-Orbital Governance"
NODE Publication "Publication & Outreach"

EDGE MathSpine -> Sneks
EDGE Sneks -> Ecosystem
EDGE Ecosystem -> Accessibility
EDGE Accessibility -> Governance
EDGE Governance -> Publication
```

```text
DIAGRAM layered-architecture-v1
LAYER Deterministic "Deterministic Layer"
LAYER Expressive "Expressive Layer (SNEKs)"
LAYER Formal "Formal Layer"
LAYER Governance "Orbital Governance Layer"
LAYER Ecosystem "Ecosystem Envelope"
LAYER Accessibility "Accessibility Kawaii Layer"
```

```text
DIAGRAM orbital-v1
CORE NDH "NDH Core"
ORBIT MathSpine "Math Spine"
ORBIT Sneks "SNEK Operators"
ORBIT Ecosystem "Ecosystem Envelope"
ORBIT Accessibility "Accessibility Layer"
ORBIT Governance "Orbital Governance"
ORBIT Publication "Publication & Outreach"
```

---

## 3. Outputs

For each diagram:

- **SVG:**  
  `NDH-Platforms/Architecture/Visual/Diagrams/<diagram-name>.svg`
- **PNG:**  
  `NDH-Platforms/Architecture/Visual/Diagrams/<diagram-name>.png`
- Optional: **ASCII snapshot:**  
  `.../Diagrams/<diagram-name>.ascii.txt`

---

## 4. Core Design Principles

- **Trauma-informed:**  
  - Text-first, low-pressure authoring.  
  - No requirement to “draw” to think structurally.  
- **Blueprint-first:**  
  - ASCII is the canonical source of truth.  
  - SVG/PNG are render targets, not primary artifacts.
- **Expressive + rigorous:**  
  - Every visual element maps to NDH concepts: manifolds, envelopes, operators, governance.  
  - Diagrams must remain emotionally accessible (kawaii cues allowed at render stage).

---

## 5. Generator Responsibilities

- **Parse DSL:**
  - `DIAGRAM`, `NODE`, `EDGE`, `LAYER`, `CORE`, `ORBIT`.
- **Validate against NDH Visual Roadmap Model:**
  - Linear diagrams must have a single left-to-right flow.
  - Layered diagrams must respect layer ordering.
  - Orbital diagrams must maintain concentric structure.
- **Render:**
  - Generate SVG with:
    - consistent NDH color palette,
    - readable labels,
    - clear arrows/edges.
  - Export PNG from SVG for convenience.

---

## 6. Integration Points

- **Blueprint Suite:**
  - Generator can be a Blueprint Suite module:
    - `blueprint.visual.ndh_roadmaps`
- **Trauma-Informed Design Systems:**
  - Documented as a **gentle visualization pipeline**:
    - text → ASCII → SVG → polished visual.
- **NDH Visual Roadmap Generation Model:**
  - This spec implements that model programmatically.

---

## 7. Roadmap v0.1 → v0.2

- v0.1:
  - Support three diagram types:
    - `linear-roadmap-v1`
    - `layered-architecture-v1`
    - `orbital-v1`
- v0.2:
  - Add:
    - per-node metadata (stability, envelope, manifold),
    - accessibility annotations,
    - theme variants (dark/light, kawaii emphasis).

```



