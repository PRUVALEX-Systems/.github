<div align="center"><img width="700" height="299" alt="image" src="https://github.com/user-attachments/assets/0562aa0e-d53a-4837-8608-5508637dfa56" />


<img src="https://via.placeholder.com/100/0A0A1A/5B5BFF?text=P" alt="PRUVALEX Logo" width="100" style="border-radius:16px"/>

<h1>PRUVALEX Systems</h1>

<p><strong>The Enterprise Operating System for AI Compliance & Cost Optimization.</strong></p>

<p>
  <a href="https://pruvalex.eu"><img src="https://img.shields.io/badge/Website-pruvalex.eu-5B5BFF?style=flat-square&logoColor=white" alt="Website"/></a>
  <a href="https://marketplace.visualstudio.com/publishers/pruvalex"><img src="https://img.shields.io/badge/VS%20Code-Marketplace-007ACC?style=flat-square&logo=visualstudiocode&logoColor=white" alt="VS Code Marketplace"/></a>
  <a href="https://github.com/PRUVALEX-Systems/pruvagraph"><img src="https://img.shields.io/badge/License-MIT-00E57A?style=flat-square" alt="MIT License"/></a>
  <img src="https://img.shields.io/badge/EU%20AI%20Act-Compliant-5B5BFF?style=flat-square" alt="EU AI Act"/>
</p>

<br/>

<p>
We engineer <strong>mathematically provable AI compliance architectures</strong> and <strong>zero-cost developer tools</strong>.<br/>
Our infrastructure allows high-risk AI systems in regulated sectors to maintain absolute compliance<br/>
while drastically reducing operational overhead.
</p>

</div>

---

## 🚀 Flagship Open-Source — PruvaGraph

> **The 99% LLM Cost Killer.** An MCP server + VS Code extension that converts your codebase into a local AST knowledge graph — so AI tools read the graph, not raw files.

<div align="center">

| | Other Tools | **PruvaGraph** |
|---|---|---|
| 10,000-file repo, daily CI | ~3,300,000 LLM calls/month | **~3,140 calls/month** |
| Monthly cost (Claude Sonnet) | ~$313/month | **~$0.30/month** |
| Re-run on unchanged files | Full LLM scan again | **Instant cache hit** |
| Changed files | Re-scans everything | **Re-scans changed files only** |
| Similar files (e.g. 40 React components) | 40 separate LLM calls | **1 LLM call via MinHash dedup** |
| Code file analysis | API cost per file | **$0.00 — local tree-sitter AST** |
| Data sovereignty | Cloud dependent | **100% local, no server** |

</div>

### How It Saves 99%+ — 4 Layers

```
Layer 1 — SHA-256 Hash Cache     → Unchanged file? 0 API calls.          Saves: 80–90% on re-runs
Layer 2 — Semantic MinHash Dedup → 40 similar files = 1 LLM call.        Saves: 40–60% additional
Layer 3 — Smart Batch Packing    → 10+ files in one API call.             Saves: 5×–10× fewer calls
Layer 4 — 3-Tier Cascade Router  → Ollama (free) → Gemini → Claude        Saves: Always cheapest tier
```

### Cascade Router — LLM Pricing

| Model | Cost per M Tokens | Used For |
|---|---|---|
| Ollama (local) | **$0.000** | Code files < 1,500 tokens |
| Gemini 2.0 Flash | **$0.075** | Medium docs < 8,000 tokens |
| GPT-4o-mini | **$0.400** | Fallback medium tier |
| Claude Sonnet 4.6 | **$3.000** | Complex PDFs / large batches only |

### 6 MCP Tools — for Claude Code & Cursor

| Tool | What You Can Ask |
|---|---|
| `query_graph` | `"How does the auth module connect to the database?"` |
| `get_dependencies` | `"What does AuthService depend on?"` |
| `find_callers` | `"Who calls processPayment()?"` |
| `get_summary` | `"Give me a one-line summary of UserController"` |
| `list_communities` | `"What are the architectural modules of this codebase?"` |
| `cost_report` | `"How much did we save on the last run?"` |

### Supported Languages — 30+ via Tree-sitter (All Free)

| Category | Languages |
|---|---|
| **Web** | TypeScript, TSX, JavaScript, JSX, Vue, Svelte, Astro, CSS, HTML |
| **Backend** | Python, Go, Rust, Java, C#, PHP, Ruby, Elixir, Scala |
| **Mobile** | Kotlin, Swift, Dart (Flutter), Objective-C |
| **Systems** | C, C++, Zig |
| **Data / Infra** | SQL, YAML, Terraform/HCL, Dockerfile, Bash |
| **Docs (LLM)** | PDF, DOCX, Markdown, Images |

### Install

```bash
pip install pruvagraph

pruvagraph . --cascade --dry-run   # Estimate cost first (no spend)
pruvagraph install                  # Auto-configure Claude Code + Cursor + VS Code
```

**→ [github.com/PRUVALEX-Systems/pruvagraph](https://github.com/PRUVALEX-Systems/pruvagraph)**

---

## 🛡️ PRUVALEX Compliance OS — Coming Soon

<div align="center">

<img src="https://img.shields.io/badge/Status-In%20Development-FFD166?style=for-the-badge" alt="In Development"/>
&nbsp;
<img src="https://img.shields.io/badge/Regulation-EU%20AI%20Act%202024%2F1689-5B5BFF?style=for-the-badge" alt="EU AI Act"/>
&nbsp;
<img src="https://img.shields.io/badge/Max%20Fine%20Protected-€35%2C000%2C000-FF3355?style=for-the-badge" alt="35M Fine Protection"/>

</div>

<br/>

> **The world's first tool to fully operationalize EU AI Act compliance.**
> Not a checklist. Not a consultant's PDF. A running system that proves your AI is legal — automatically, cryptographically, continuously.

### The Problem: Fines No Company Can Afford to Ignore

The EU AI Act (Reg. 2024/1689) entered into force on **August 1, 2024**. Enforcement is already rolling out in phases — and the penalties are existential:

| Violation Type | Maximum Fine |
|---|---|
| Prohibited AI system deployed | **€35,000,000** or **7% of global annual turnover** |
| High-risk AI obligations violated | **€15,000,000** or **3% of global annual turnover** |
| Incorrect information to authorities | **€7,500,000** or **1.5% of global annual turnover** |

Most companies have **no systematic way to prove compliance** when an audit begins. They rely on internal checklists, manual documentation, and legal teams — all of which fail under scrutiny because they produce no cryptographic, timestamped, court-admissible evidence trail.

**PRUVALEX Compliance OS solves this at the infrastructure level.**

---

### Enforcement Timeline — The Clock Is Running

```
✅  Aug 01, 2024  →  EU AI Act enters into force
⚠️  Feb 02, 2025  →  Prohibited AI practices ban — ACTIVE NOW
⏳  Aug 02, 2025  →  GPAI model rules (GPT-4, Claude, Gemini, etc.)
⏳  Aug 02, 2026  →  High-risk AI systems — Annex III (healthcare, hiring, credit, law enforcement)
⏳  Aug 02, 2027  →  Annex I high-risk systems (medical devices, vehicles, critical infrastructure)
```

If your organization is building or deploying AI in the EU — or for EU users — you are already subject to Article 5 (prohibited practices). **The window to prepare is now.**

---

### What PRUVALEX Compliance OS Does

PRUVALEX Compliance OS is not a documentation helper. It is an **operating layer** that sits between your AI system and the regulator — generating, signing, and storing the evidence your legal team needs before they need it.

#### ⚙️ Three Core Pillars

**`Sovereign AI Vault`** — Cryptographic Proof, Always Ready

Every deployment decision, model version, configuration change, and inference parameter is captured in a **WORM (Write-Once, Read-Many) audit trail**, signed with **ML-DSA-65 (NIST FIPS 204)** post-quantum cryptography. When a regulator asks "what was your system doing on March 14th?" — you answer in seconds, not months.

- Post-quantum signature: ML-DSA-65 (NIST FIPS 204)
- Immutable log: WORM-enforced, tamper-evident
- Court-grade evidence: timestamped, hash-chained, verifiable by any third party

**`Regulatory Time-Traveler`** — Point-in-Time Compliance Snapshots

Your system's compliance state changes every time a model is updated, a threshold is adjusted, or a dataset is retrained. The Regulatory Time-Traveler captures a **complete compliance snapshot** at every significant event — so you can travel back to any moment and prove exactly what your system looked like, who approved it, and what evidence existed at that time.

- Full state reconstruction at any past timestamp
- Approval chain and signatory records preserved
- Designed for litigation, regulatory review, and internal audits

**`Global Law-Sync`** — Automated Regulatory Coverage

EU AI Act is not static — it evolves through implementing acts, delegated regulations, and official guidance. Global Law-Sync continuously monitors regulatory updates and automatically flags when your system's compliance posture needs to change.

- Systematic coverage of Reg. EU 2024/1689 and its delegated acts
- Automated technical gears triggered by regulatory changes
- Maps your AI system's risk classification to current Article obligations

---

### 7-Gate Deployment Verification

Before any AI system goes live, PRUVALEX Compliance OS runs it through **7 automated verification gates**. All 7 must pass. If any gate fails, deployment is blocked and the reason is logged with a cryptographic timestamp.

```
Gate 1 — Risk Classification Verification      Article 6 / Annex III check
Gate 2 — Technical Documentation Completeness  Article 11 requirements met
Gate 3 — Data Governance Audit                 Article 10 training data controls
Gate 4 — Human Oversight Mechanism Check       Article 14 override capability confirmed
Gate 5 — Accuracy & Robustness Baseline        Article 15 performance thresholds
Gate 6 — Transparency Obligation Verification  Article 13 user disclosure confirmed
Gate 7 — Cryptographic Seal & WORM Commit      Deployment evidence locked immutably
```

Only after all 7 gates pass does the system generate a **signed Deployment Certificate** — the document your legal team needs if a regulator comes knocking.

---

### PenaltyShield Dashboard

Real-time visibility into your compliance exposure across every AI system your organization runs.

```
┌─────────────────────────────────────────────────────────────┐
│  PRUVALEX PenaltyShield Dashboard                           │
├───────────────────┬─────────────────┬───────────────────────┤
│  System           │  Risk Class     │  Fine Exposure        │
├───────────────────┼─────────────────┼───────────────────────┤
│  Hiring AI v2.3   │  HIGH RISK      │  Shielded ✅          │
│  Credit Scorer    │  HIGH RISK      │  Shielded ✅          │
│  Chatbot v1.1     │  LIMITED RISK   │  Shielded ✅          │
│  Fraud Detector   │  HIGH RISK      │  Gate 4 Pending ⏳    │
└───────────────────┴─────────────────┴───────────────────────┘
  Total Protected Exposure:  €0  of  potential €47,500,000
```

---

### Who This Is For

| Organization Type | Why They Need It |
|---|---|
| **Banks & FinTech** | Credit scoring, fraud detection — Annex III high-risk by default |
| **Healthcare / MedTech** | AI-assisted diagnosis — strictest obligations under EU AI Act |
| **HR Tech / Hiring Platforms** | Recruitment AI is explicitly listed as high-risk in Annex III |
| **Legal Tech** | AI in judicial/legal decisions — regulated from Feb 2025 |
| **Any company using GPAI** | GPT-4, Claude, Gemini — GPAI rules active from Aug 2025 |
| **Critical Infrastructure** | Water, energy, transport AI — maximum obligation tier |

---

<div align="center">

### 🔔 Join the Waitlist

PRUVALEX Compliance OS is currently in development.<br/>
Enterprise early access opens Q3 2025.

**[→ Contact us at security@pruvalex.eu](mailto:security@pruvalex.eu)**

<sub>We are building this because the fines are real, the timeline is now, and no other tool does this at the infrastructure level.</sub>

</div>

---

<div align="center">

**[pruvalex.eu](https://pruvalex.eu)** &nbsp;•&nbsp; **[VS Code Marketplace](https://marketplace.visualstudio.com/publishers/pruvalex)** &nbsp;•&nbsp; **[security@pruvalex.eu](mailto:security@pruvalex.eu)**

<sub>Open source, MIT licensed. Built for developers who love Claude Code — but not the bill.</sub>

</div>
