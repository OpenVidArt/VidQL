# VidQL Roadmap

> VidQL is a query + action language designed for structured data, automation, and creative systems.
> It combines querying with executable operations, enabling workflows beyond traditional databases.

---

## Guiding Principles

- **General-purpose core** — data, automation, and creative systems
- **Action-oriented design** — query + act
- **Stable core with extensible system**
- **Safe customization** — no fragmented dialects
- **Designed for real-world developer adoption**

---

## Phase 0 — Foundations `v0.1`

**Goal:** Establish a working language core.

### Features
- Core syntax definition
- Parser (AST generation)
- CLI tool (`vidql run`)
- Basic in-memory execution engine

---

## Phase 1 — Query System `v0.2–v0.4`

**Goal:** Build a structured query foundation.

### Features
- `SELECT`, `WHERE`, filtering
- Basic data types:
  - `string`
  - `number`
  - `boolean`
  - `object`
- Dataset abstraction layer
- Deterministic execution model

---

## Phase 2 — Action System `v0.5–v0.7`

**Goal:** Introduce executable workflows.

### Features
- Actions:
  - `APPLY`
  - `PROCESS`
  - `TRANSFORM`
  - `RUN`
- Query → action pipelines
- Chained execution model

```vidql
SELECT users
WHERE active = true
PROCESS notify
```

---

## Phase 3 — Scripting Layer `v0.8–v1.0`

**Goal:** Enable automation and logic.

### Features
- Variables
- Functions
- Control flow:
  - `IF`
  - `LOOP`
- Modular scripts

---

## Phase 4 — Domain Extensions `v1.1+`

**Goal:** Extend VidQL into specialized domains.

### Features
- Domain-specific types:
  - `clip`, `timeline`
  - `dataset`, `model`
- Domain-specific actions

---

## Phase 5 — Extensibility System `v1.3+`

**Goal:** Allow controlled user-defined language extensions.

### Custom Types

```vidql
TYPE Scene {
    clips: list<clip>
    mood: string
    duration: number
}
```

### Custom Functions

```vidql
FUNCTION highlightLowLight(clips) {
    RETURN APPLY colorgrade TO clips WHERE lighting = "low"
}
```

### Custom Actions

```vidql
ACTION autoEdit {
    SELECT clips WHERE quality > 0.7
    APPLY stabilize
}
```

### Rules
- Extensions **cannot** modify core syntax
- Extensions compile to core VidQL operations
- No conflicting grammar changes
- Execution is sandboxed

---

## Phase 6 — Integration Layer `v1.5+`

**Goal:** Connect VidQL to real systems.

### Features
- VidArt Studio integration
- VidOS integration layer
- External API connectors
- Database bridges
- Real-time execution hooks

---

## Phase 7 — Performance & Scaling `v2.0+`

**Goal:** Production-grade execution.

### Features
- Query optimization engine
- Parallel execution
- Caching system
- Large dataset handling
- Performance profiling tools

---

## Phase 8 — Ecosystem Growth `v2.5+`

**Goal:** Build a developer ecosystem.

### Features
- SDKs (Python, JavaScript)
- Plugin system
- Community extensions
- Documentation platform
- Package registry *(optional)*

---

## Long-Term Vision

VidQL becomes a unified language for **querying, automating, and acting on** data, systems, and creative workflows.

It is a **control layer** for computational and creative systems.

---

## Status

| Field | Value |
|---|---|
| Current Version | `v0.0` *(planning)* |
| Next Milestone | `v0.1` — Foundations |
