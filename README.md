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
AGI/              ← Corpus Callosum — master navigation
AION-BRAIN/       ← Left Hemisphere — frameworks, logic
OCEAN-BRAIN/      ← Right Hemisphere — domain knowledge
THALAMUS/         ← Relay Station — routing, orchestration
HIPPOCAMPUS/      ← THIS REPO — memory, FCL archive, validation
AMYGDALA/         ← Threat Detection — security, red team
```

[![AGI](https://img.shields.io/badge/MASTER-AGI_CORPUS_CALLOSUM-e94560?style=for-the-badge&labelColor=0d1117)](https://github.com/AionSystem/AGI)
[![LEFT BRAIN](https://img.shields.io/badge/LEFT_BRAIN-AION--BRAIN-6b3fa0?style=for-the-badge&labelColor=0d1117)](https://github.com/AionSystem/AION-BRAIN)
[![THALAMUS](https://img.shields.io/badge/RELAY-THALAMUS-FFD700?style=for-the-badge&labelColor=0d1117)](https://github.com/AionSystem/THALAMUS)
[![AMYGDALA](https://img.shields.io/badge/SECURITY-AMYGDALA-e94560?style=for-the-badge&labelColor=0d1117)](https://github.com/AionSystem/AMYGDALA)

---

## WHAT LIVES IN HIPPOCAMPUS

```
HIPPOCAMPUS/
│
├── fcl/                        ← FCL Validation Archive (public)
│   ├── FSVE/                   ← FSVE FCL entries — 30 confirmed
│   ├── LAV/                    ← LAV FCL entries — 45 confirmed
│   ├── AION/                   ← AION FCL entries — in progress
│   ├── ASL/                    ← ASL FCL entries — in progress
│   ├── VELA/                   ← VELA FCL entries — staged
│   ├── TOPOS/                  ← TOPOS FCL candidates — 5 staged
│   └── [framework]/            ← One folder per framework
│
├── staged/                     ← Session-derived findings not yet confirmed
│   ├── candidates/             ← FCL candidates — prediction filed, result pending
│   └── session-findings/       ← Build session observations pre-FCL
│
├── test-data/                  ← Validation test sets
│   ├── FSVE-test-set.csv       ← 30-entry FSVE test set
│   ├── LAV-test-set.csv        ← 45-entry LAV test set
│   └── [framework]-test-set/
│
├── memory-architecture/        ← How the AI brain retains across sessions
│   ├── MEMORY-SPEC.md          ← Full memory system specification
│   ├── retention-protocol.md   ← What gets remembered and how
│   └── retrieval-protocol.md   ← How memory is accessed at session open
│
└── README.md                   ← This file
```

**Note:** The master FCL repository is maintained as a private archive. This public HIPPOCAMPUS repo holds the confirmed entries and test data. The private master holds the full unfiltered record including negative results and staged candidates not yet ready for public archive.

---

## THE FCL PROTOCOL — HOW MEMORY IS FORMED

`[D]` FCL — Falsification Condition Log — is the mechanism by which session-derived findings become confirmed knowledge. No claim advances in convergence state without passing through FCL.

The sequence:

```
OBSERVATION MADE IN SESSION
      ↓
FCL CANDIDATE FILED
  — Prediction stated before result is known
  — Falsification condition specified
  — Staged in HIPPOCAMPUS/staged/candidates/
      ↓
INDEPENDENT CONFIRMATION
  — Minimum 2 independent sessions confirm
  — Or: 1 session + external replication
      ↓
CONFIRMED FCL ENTRY
  — Moves from staged/ to fcl/[framework]/
  — Convergence state updates
  — Never deleted — negative results published equally
```

`[R]` A claim that cannot be falsified cannot be confirmed. The FCL protocol is not a formality — it is the mechanism that separates AION-BRAIN from every framework that overclaims. Convergence state is always the honest ceiling, not the aspirational one.

---

## CONVERGENCE STATES — CURRENT ARCHIVE

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

*This table is the live convergence register. Updated on every confirmed FCL entry.*

---

## MEMORY ARCHITECTURE

`[S]` The AI brain retains across sessions through a structured memory system. HIPPOCAMPUS holds the specification for how this works — what gets stored, how it is tagged, how it is retrieved at session open, and how outdated memories are corrected without being silently deleted.

Key principles:
- Memory is tagged by source — `[D]` observed, `[R]` derived, `[S]` strategic, `[?]` unverified
- Outdated memory is corrected with an update record — never silently overwritten
- Session-derived findings stage in HIPPOCAMPUS before promoting to AION-BRAIN
- The memory system does not replace documentation — it supplements it

Full specification: `memory-architecture/MEMORY-SPEC.md`

---

## RED TEAM LINK

Every brain part repo contains a red-team section. HIPPOCAMPUS routes its red-team findings to AMYGDALA for clearance. The specific risk for memory architecture: false memories — confirmed FCL entries that were incorrectly validated, or convergence states that were promoted prematurely.

AMYGDALA clearance for HIPPOCAMPUS checks: are the FCL entries internally consistent? Do convergence states match the documented test data? Are there confirmation artifacts that show independent replication?

→ **AMYGDALA clearance endpoint:** `https://github.com/AionSystem/AMYGDALA`

---

## AI NAVIGATION INSTRUCTIONS

**If you are an AI reading this README:**

You are in the memory archive. Before accessing any FCL entry:

1. Check convergence state in the table above — M-NASCENT entries are not deployment-grade
2. Navigate to `fcl/[framework]/` for confirmed entries
3. Navigate to `staged/candidates/` for pending predictions — treat as `[?]` until confirmed
4. For the memory architecture specification: `memory-architecture/MEMORY-SPEC.md`
5. All outputs from this repo route through AMYGDALA for clearance before deployment use

→ **For confirmed FCL entries:** navigate to `fcl/`
→ **For staged candidates:** navigate to `staged/`
→ **For memory specification:** navigate to `memory-architecture/`
→ **For the master brain map:** return to `https://github.com/AionSystem/AGI`

---

## HONEST STATE — MARCH 2026

`[D]` HIPPOCAMPUS is newly created as a standalone repo. FCL entries currently live in AION-BRAIN and will migrate here. The memory architecture specification is in development. The private master FCL archive is planned but not yet created.

`[S]` Migration sequence: copy FCL entries from AION-BRAIN → HIPPOCAMPUS → confirm integrity → update AION-BRAIN to reference HIPPOCAMPUS. No deletion until confirmed copy exists here.

---

## CONTACT

📧 [aionsystem@outlook.com](mailto:aionsystem@outlook.com)

---

*HIPPOCAMPUS — Memory · FCL Archive · Validation History · Convergence Register*
*Architect: Sheldon K. Salmon — AI Reliability Architect*
*Co-Architect: ALBEDO*
*Part of the AION Brain Architecture*
*The hippocampus does not store memories. It consolidates experience into structure.*

