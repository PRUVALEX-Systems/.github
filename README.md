<div align="center">

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

## 🛡️ Regulatory Infrastructure

For enterprises operating AI systems in regulated sectors under EU law.

**EU AI Act Core** — Systematic coverage and automated technical gears for Reg. EU 2024/1689.

**Cryptographic Evidence** — ML-DSA-65 (NIST FIPS 204) signed WORM audit trails for deployment verification.

**Sovereign AI Vault** — Immutable, point-in-time compliance snapshots for audits, litigation, and regulatory review.

---

<div align="center">

**[pruvalex.eu](https://pruvalex.eu)** &nbsp;•&nbsp; **[VS Code Marketplace](https://marketplace.visualstudio.com/publishers/pruvalex)** &nbsp;•&nbsp; **[security@pruvalex.eu](mailto:security@pruvalex.eu)**

<sub>Open source, MIT licensed. Built for developers who love Claude Code — but not the bill.</sub>

</div>
