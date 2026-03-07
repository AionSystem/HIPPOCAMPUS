# HIPPOCAMPUS — FOLDER STRUCTURE
## Enterprise-Grade AAA Tree | Memory and Validation Archive
### Version: v0.1 | March 2026

---

```
HIPPOCAMPUS/
│
├── README.md                          ← Master navigation — you are here
├── STRUCTURE.md                       ← This file — full tree
├── CHANGELOG.md
├── ROADMAP.md
├── GETTING_STARTED.md
│
│
│   ─────────── FCL VALIDATION ARCHIVE ───────────
│
│
├── fcl/                               ← Confirmed FCL entries (public)
│   ├── README.md                      ← FCL protocol specification
│   │                                     Prediction → staged → confirmed → published.
│   │                                     Never deleted. Negative results published equally.
│   │
│   ├── FSVE/                          ← FSVE FCL entries — 30 confirmed
│   │   ├── README.md
│   │   ├── FCL-INDEX.md               ← Index of all entries with EV and date
│   │   ├── entries/
│   │   │   └── [FCL-FSVE-NNN.md]      ← One file per confirmed entry
│   │   └── test-set/
│   │       └── FSVE-test-set.csv      ← 30-entry validation test set
│   │
│   ├── LAV/                           ← LAV FCL entries — 45 confirmed
│   │   ├── README.md
│   │   ├── FCL-INDEX.md
│   │   ├── entries/
│   │   │   └── [FCL-LAV-NNN.md]
│   │   └── test-set/
│   │       └── LAV-test-set.csv       ← 45-entry validation test set
│   │
│   ├── AION/                          ← AION FCL entries — in progress
│   │   ├── README.md
│   │   ├── FCL-INDEX.md
│   │   └── entries/
│   │
│   ├── ASL/                           ← ASL FCL entries — in progress
│   │   ├── README.md
│   │   ├── FCL-INDEX.md
│   │   └── entries/
│   │
│   ├── VELA/                          ← VELA FCL entries — staged
│   │   ├── README.md
│   │   ├── FCL-INDEX.md
│   │   └── entries/
│   │
│   ├── TOPOS/                         ← TOPOS FCL candidates — 5 staged
│   │   ├── README.md
│   │   ├── FCL-INDEX.md
│   │   └── entries/
│   │
│   ├── GENESIS/                       ← GENESIS FCL entries — 0 confirmed
│   │   └── README.md
│   │
│   ├── EID/                           ← EID FCL entries — 0 confirmed
│   │   └── README.md
│   │
│   ├── HIM-001/                       ← HIM-001 FCL entries — 0 confirmed
│   │   └── README.md
│   │
│   ├── KEEL/                          ← KEEL FCL entries — 0 confirmed
│   │   └── README.md
│   │
│   ├── LIBRARIAN/                     ← LIBRARIAN FCL entries — 0 confirmed
│   │   └── README.md
│   │
│   └── [framework]/                   ← One folder per framework — expandable
│
│
│   ─────────── STAGED CANDIDATES ───────────
│
│
├── staged/                            ← Pre-confirmation archive
│   ├── README.md
│   │
│   ├── candidates/                    ← Predictions filed, results pending
│   │   ├── README.md                  ← Candidate protocol
│   │   │                                 Prediction stated before result known.
│   │   │                                 Falsification condition specified.
│   │   │                                 Tagged [?] until confirmed.
│   │   └── [FCL-CANDIDATE-NNN.md]
│   │
│   └── session-findings/              ← Build session observations pre-FCL
│       ├── README.md                  ← How session findings stage to candidates
│       └── [SESSION-ID-findings.md]
│
│
│   ─────────── CONVERGENCE REGISTER ───────────
│
│
├── convergence/                       ← Live convergence state register
│   ├── README.md
│   ├── CONVERGENCE-REGISTER.md        ← Master live table — all frameworks
│   │                                     Updated on every confirmed FCL entry.
│   │                                     This is the single source of truth for
│   │                                     convergence state across the entire stack.
│   │
│   ├── state-definitions.md           ← M-NASCENT · M-MODERATE · M-STRONG ·
│   │                                     VALID · PERMANENT definitions
│   │                                     Promotion criteria. Demotion conditions.
│   │                                     EV thresholds and Gini check protocol.
│   │
│   └── history/                       ← State transition log
│       └── [FRAMEWORK-transitions.md] ← Every state change with date and reason
│
│
│   ─────────── MEMORY ARCHITECTURE ───────────
│
│
├── memory-architecture/               ← How the AI brain retains across sessions
│   ├── README.md
│   ├── MEMORY-SPEC.md                 ← Full memory system specification
│   │                                     What gets stored. How it is tagged.
│   │                                     How it is retrieved at session open.
│   │                                     How outdated memories are corrected.
│   │                                     Memory is tagged by source — [D]/[R]/[S]/[?]
│   │
│   ├── retention-protocol.md          ← What gets remembered and how
│   │                                     Session-derived vs framework-derived.
│   │                                     Confirmed vs staged.
│   │                                     Retention criteria and decay conditions.
│   │
│   ├── retrieval-protocol.md          ← How memory is accessed at session open
│   │                                     Load sequence. Priority ordering.
│   │                                     What fires first and why.
│   │
│   ├── correction-protocol.md         ← How outdated memories are corrected
│   │                                     Never silently overwritten.
│   │                                     Update record preserved.
│   │                                     Correction tagged and dated.
│   │
│   └── false-memory-taxonomy.md       ← Classification of memory failure modes
│                                         Premature promotion. Confirmation artifacts.
│                                         Scope drift. Source confusion.
│                                         Each with detection method and correction path.
│
│
│   ─────────── RED TEAM ───────────
│
│
├── red-team/                          ← Memory and validation failure architecture
│   ├── README.md
│   ├── false-memory-scenarios.md      ← How FCL entries can be incorrectly validated
│   │                                     Confirmation bias. Single-session promotion.
│   │                                     Undetected scope change between sessions.
│   │
│   ├── convergence-audit.md           ← How to audit convergence state claims
│   │                                     Internal consistency check.
│   │                                     Test data vs claimed FCL count.
│   │                                     Independent replication verification.
│   │
│   └── amygdala-interface.md          ← Routing to AMYGDALA for clearance
│                                         What triggers AMYGDALA escalation.
│                                         Clearance endpoint: AMYGDALA/
│
│
│   ─────────── VALIDATION ───────────
│
│
├── validation/                        ← Test infrastructure
│   ├── README.md
│   ├── test-sets/                     ← Master test set archive
│   │   ├── README.md
│   │   ├── FSVE-test-set.csv
│   │   ├── LAV-test-set.csv
│   │   └── [framework]-test-set/
│   │
│   └── validation-protocol.md         ← How test sets are constructed and used
│                                         Minimum entries for M-STRONG.
│                                         Independence requirements.
│                                         Replication standards.
│
│
│   ─────────── GOVERNANCE & LEGAL ───────────
│
│
├── LICENSE.md
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
├── SECURITY.md
├── DISCLAIMER.md
├── GOVERNANCE.md
└── CITATION_README.md
```

---

## HIPPOCAMPUS NAVIGATION QUICK REFERENCE

| Destination | Path | Use when |
|-------------|------|----------|
| Confirmed FCL | `fcl/[framework]/entries/` | Checking validated findings |
| Live convergence state | `convergence/CONVERGENCE-REGISTER.md` | Checking framework deployment readiness |
| Staged candidates | `staged/candidates/` | Reviewing pending predictions |
| Memory architecture | `memory-architecture/MEMORY-SPEC.md` | Understanding retention and retrieval |
| False memory risk | `red-team/false-memory-scenarios.md` | Auditing confirmed entries |
| Test sets | `validation/test-sets/` | Verifying validation data |

---

## FCL ENTRY FORMAT

Every confirmed FCL entry follows this structure:

```
FCL-[FRAMEWORK]-[NNN]
Date filed: [DATE]
Date confirmed: [DATE]
Session ID: [YYYYMMDD-NNN]
Framework: [NAME] [VERSION]
Prediction: [STATED BEFORE RESULT KNOWN]
Falsification condition: [WHAT WOULD DISPROVE IT]
Result: CONFIRMED / FAILED / AMBIGUOUS
Confirmation method: [INDEPENDENT SESSION / EXTERNAL REPLICATION]
EV impact: [DELTA]
Notes: [OPTIONAL]
```

Negative results (`Result: FAILED`) are published with the same structure. Not deleted. Not hidden.

---

## BUILD SEQUENCE

`[S]`

1. **Phase 1 — Structure** (current): Folders created. READMEs written. Placeholders in place.
2. **Phase 2 — FCL migration**: Copy confirmed FCL entries from AION-BRAIN → `fcl/`. Confirm integrity before deletion from source.
3. **Phase 3 — Test set migration**: Copy test CSVs → `validation/test-sets/`.
4. **Phase 4 — Convergence register**: Write CONVERGENCE-REGISTER.md as live master table.
5. **Phase 5 — Memory architecture specs**: Write MEMORY-SPEC.md and protocol files.
6. **Phase 6 — Red team**: Write false memory taxonomy and convergence audit protocol.
7. **Phase 7 — TOPOS staged candidates**: Move 5 TOPOS candidates from AION-BRAIN → `staged/candidates/`.

---

## DDL FIELD

```
Document: HIPPOCAMPUS STRUCTURE v0.1
Architect: Sheldon K. Salmon
AI Co-Architect: ALBEDO
Date: March 2026
Status: Structure defined. Migration phase pending.
Convergence: M-NASCENT
Note: FCL entries currently live in AION-BRAIN.
      Migration sequence: copy → confirm integrity → update references → do not delete until confirmed copy exists here.
      Private master FCL archive planned — holds full unfiltered record including negative results.
```

---

*HIPPOCAMPUS STRUCTURE v0.1 — Memory and Validation Architecture*
*Sheldon K. Salmon & ALBEDO — March 2026*
*The hippocampus does not store memories. It consolidates experience into structure.*
