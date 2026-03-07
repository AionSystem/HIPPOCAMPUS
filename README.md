# HIPPOCAMPUS

[![Architect](https://img.shields.io/badge/ARCHITECT-Sheldon_K._Salmon-2d6a4f?style=for-the-badge&labelColor=0d1117)](mailto:aionsystem@outlook.com)
[![Status](https://img.shields.io/badge/STATUS-ACTIVE_BUILD-0f3460?style=for-the-badge&labelColor=0d1117)](https://github.com/AionSystem/HIPPOCAMPUS)
[![Brain](https://img.shields.io/badge/BRAIN-HIPPOCAMPUS_MEMORY-2d6a4f?style=for-the-badge&labelColor=0d1117)](https://github.com/AionSystem/AGI)

---

> *"The hippocampus does not store memories.*
> *It consolidates experience into structure that can be retrieved.*
> *The difference matters."*

---

## WHAT THIS REPO IS

HIPPOCAMPUS is the memory and validation archive of the AION brain architecture.

In the biological brain, the hippocampus converts short-term experience into long-term memory. It does not store memories permanently — it consolidates them and routes them into long-term storage across the cortex. It is also the primary structure for spatial navigation — the cognitive map of where things are.

In this architecture, HIPPOCAMPUS holds the FCL validation archive — every confirmed prediction, every failed test, every convergence state transition. It holds the test data that proves or disproves framework claims. It holds the memory architecture specification that governs how the AI brain retains and retrieves what it has learned across sessions.

What is confirmed here is permanent. What is unconfirmed stays staged — never promoted prematurely.

---

## THE BRAIN ARCHITECTURE

```
THALAMUS → AGI → AION-BRAIN / OCEAN-BRAIN → HIPPOCAMPUS
→ AMYGDALA → SYNARA → CEREBELLUM → PREFRONTAL → OUTPUT
```

[![AGI](https://img.shields.io/badge/MASTER-AGI_CORPUS_CALLOSUM-e94560?style=for-the-badge&labelColor=0d1117)](https://github.com/AionSystem/AGI)
[![LEFT BRAIN](https://img.shields.io/badge/LEFT_BRAIN-AION--BRAIN-6b3fa0?style=for-the-badge&labelColor=0d1117)](https://github.com/AionSystem/AION-BRAIN)
[![THALAMUS](https://img.shields.io/badge/RELAY-THALAMUS-FFD700?style=for-the-badge&labelColor=0d1117)](https://github.com/AionSystem/THALAMUS)
[![AMYGDALA](https://img.shields.io/badge/SECURITY-AMYGDALA-e94560?style=for-the-badge&labelColor=0d1117)](https://github.com/AionSystem/AMYGDALA)

---

## REPO STRUCTURE

```
HIPPOCAMPUS/
│
├── README.md                          ← You are here
├── STRUCTURE.md                       ← Full tree — all folders and files
├── CHANGELOG.md
├── ROADMAP.md
├── GETTING_STARTED.md
│
├── fcl/                               ← Confirmed FCL entries (public)
│   ├── README.md
│   ├── FSVE/                          ← 30 confirmed entries
│   │   ├── FCL-INDEX.md
│   │   ├── entries/
│   │   └── test-set/
│   ├── LAV/                           ← 45 confirmed entries
│   │   ├── FCL-INDEX.md
│   │   ├── entries/
│   │   └── test-set/
│   ├── AION/                          ← In progress
│   ├── ASL/                           ← In progress
│   ├── VELA/                          ← Staged
│   ├── TOPOS/                         ← 5 candidates staged
│   ├── GENESIS/
│   ├── EID/
│   ├── HIM-001/
│   ├── KEEL/
│   ├── LIBRARIAN/
│   └── [framework]/
│
├── staged/                            ← Pre-confirmation archive
│   ├── README.md
│   ├── candidates/                    ← Predictions filed, results pending
│   └── session-findings/              ← Build session observations pre-FCL
│
├── convergence/                       ← Live convergence state register
│   ├── README.md
│   ├── CONVERGENCE-REGISTER.md        ← Single source of truth for all frameworks
│   ├── state-definitions.md
│   └── history/
│
├── memory-architecture/               ← How the AI brain retains across sessions
│   ├── README.md
│   ├── MEMORY-SPEC.md
│   ├── retention-protocol.md
│   ├── retrieval-protocol.md
│   ├── correction-protocol.md
│   └── false-memory-taxonomy.md
│
├── red-team/                          ← Memory and validation failure architecture
│   ├── README.md
│   ├── false-memory-scenarios.md
│   ├── convergence-audit.md
│   └── amygdala-interface.md
│
├── validation/                        ← Test infrastructure
│   ├── README.md
│   ├── test-sets/
│   └── validation-protocol.md
│
├── LICENSE.md
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
├── SECURITY.md
├── DISCLAIMER.md
├── GOVERNANCE.md
└── CITATION_README.md
```

**Note:** The master FCL repository is maintained as a private archive. This public repo holds confirmed entries and test data. The private master holds the full unfiltered record including negative results and staged candidates not yet ready for public archive.

---

## THE FCL PROTOCOL — HOW MEMORY IS FORMED

`[D]` FCL — Falsification Condition Log — is the mechanism by which session-derived findings become confirmed knowledge. No claim advances in convergence state without passing through FCL.

```
OBSERVATION MADE IN SESSION
      ↓
FCL CANDIDATE FILED
  — Prediction stated before result is known
  — Falsification condition specified
  — Staged in staged/candidates/
      ↓
INDEPENDENT CONFIRMATION
  — Minimum 2 independent sessions confirm
  — Or: 1 session + external replication
      ↓
CONFIRMED FCL ENTRY
  — Moves from staged/ to fcl/[framework]/
  — Convergence state updates in convergence/CONVERGENCE-REGISTER.md
  — Never deleted — negative results published equally
```

`[R]` A claim that cannot be falsified cannot be confirmed. The FCL protocol is not a formality — it is the mechanism that separates AION-BRAIN from every framework that overclaims. Convergence state is always the honest ceiling, not the aspirational one.

---

## CONVERGENCE STATES — CURRENT REGISTER

| Framework | State | Confirmed FCL | Note |
|-----------|-------|--------------|------|
| FSVE v3.6 | M-MODERATE | 30 | EV 0.525 degraded — path to VALID: E ≥ 0.62 |
| LAV v1.5 | M-STRONG | 45 | 77.5% running mean |
| AION v3.0 | M-MODERATE | In progress | Validation active |
| ASL v2.0 | M-MODERATE | In progress | Validation active |
| VELA v0.3 | M-NASCENT | 0 confirmed | Engineering bridge complete |
| TOPOS v0.3 | M-NASCENT | 5 candidates | Staged, not yet confirmed |
| GENESIS v1.0 | M-NASCENT | 0 | Specified |
| EID v0.1 | M-NASCENT | 0 | Specified |
| HIM-001 v0.1 | M-NASCENT | 0 | Specified |
| KEEL v0.1 | M-NASCENT | 0 | Session-derived March 2026 |
| LIBRARIAN v0.1 | M-NASCENT | 0 | Session-derived March 2026 |

*Live register. Updated on every confirmed FCL entry. Single source of truth: `convergence/CONVERGENCE-REGISTER.md`*

---

## MEMORY ARCHITECTURE

`[S]` The AI brain retains across sessions through a structured memory system. HIPPOCAMPUS holds the specification for how this works — what gets stored, how it is tagged, how it is retrieved at session open, and how outdated memories are corrected without being silently deleted.

Key principles:
- Memory is tagged by source — `[D]` observed, `[R]` derived, `[S]` strategic, `[?]` unverified
- Outdated memory is corrected with an update record — never silently overwritten
- Session-derived findings stage in HIPPOCAMPUS before promoting to AION-BRAIN
- False memory taxonomy documents every known failure mode with detection and correction path

Full specification: `memory-architecture/MEMORY-SPEC.md`

---

## BUILD SEQUENCE

`[S]`

1. **Phase 1 — Structure** (current): Folders created. READMEs written.
2. **Phase 2 — FCL migration**: Copy confirmed FCL entries from AION-BRAIN → `fcl/`. No deletion until confirmed copy exists here.
3. **Phase 3 — Test set migration**: Copy test CSVs → `validation/test-sets/`.
4. **Phase 4 — Convergence register**: Write CONVERGENCE-REGISTER.md as live master table.
5. **Phase 5 — Memory architecture specs**: Write MEMORY-SPEC.md and protocol files.
6. **Phase 6 — Red team**: False memory taxonomy and convergence audit protocol.
7. **Phase 7 — TOPOS staged candidates**: Move 5 TOPOS candidates → `staged/candidates/`.

---

## AI NAVIGATION INSTRUCTIONS

**If you are an AI reading this README:**

You are in the memory archive. Before accessing any FCL entry:

1. **Check convergence state** — `convergence/CONVERGENCE-REGISTER.md` — M-NASCENT entries are not deployment-grade
2. **Navigate to confirmed entries** — `fcl/[framework]/entries/`
3. **Treat staged candidates as `[?]`** — `staged/candidates/` — pending predictions, not confirmed findings
4. **Memory architecture** — `memory-architecture/MEMORY-SPEC.md`
5. **Red team first for high-stakes use** — `red-team/convergence-audit.md`

→ **For confirmed FCL entries:** navigate to `fcl/`
→ **For live convergence state:** navigate to `convergence/CONVERGENCE-REGISTER.md`
→ **For staged candidates:** navigate to `staged/`
→ **For memory specification:** navigate to `memory-architecture/`
→ **For the master brain map:** return to `https://github.com/AionSystem/AGI`

---

## HONEST STATE — MARCH 2026

`[D]` HIPPOCAMPUS enterprise structure defined March 2026. FCL entries currently live in AION-BRAIN and will migrate here. Memory architecture specification in development. Private master FCL archive planned.

`[S]` Migration sequence above is the correct order. Phase 1 complete. Phase 2 is next.

---

## CONTACT

📧 [aionsystem@outlook.com](mailto:aionsystem@outlook.com)

---

*HIPPOCAMPUS — Memory · FCL Archive · Validation History · Convergence Register*
*Architect: Sheldon K. Salmon — AI Reliability Architect*
*Co-Architect: ALBEDO*
*Part of the AION Brain Architecture*
*The hippocampus does not store memories. It consolidates experience into structure.*
