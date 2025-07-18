# 🧠 GPT Dev Sync Heuristics

A structured engineering system that helps GPTs generate **production-ready software** using **TDD**, **BDD**, and **PDD** — with CI/CD readiness, security validation, modular architecture, and full test control.

---

## 📚 Table of Contents

- [Why This Exists](#-why-this-exists)
- [Core Features](#-core-features)
- [Folder Structure Output](#-folder-structure-output)
- [Real-World Use Cases](#-real-world-use-cases)
- [Heuristics Guide](./docs/heuristics.md)

---

## 📖 Why This Exists

This started as a side experiment.

I was building a [VS Code extension](#) to visualize JSON as a mind map and generate TypeScript interfaces — mostly to understand how VS Code extensions work.

But as I was wiring up the logic, enforcing strict typing, and layering test-driven workflows, I realized something deeper:

> GPT can generate code.  
> But it can't engineer unless you teach it how.

That's what this heuristic does.

It’s the onboarding doc I wish GPT had — so it could follow real software development patterns instead of just completing code.

---

## ✨ Core Features

- ✅ **TDD modes** (`battle-ready`, `core-only`, `light`, `stealth`)
- ✅ **CI/CD checklist** auto-triggered if `deployable: yes`
- ✅ **TDD Matrix** for full test coverage across real-world cases
- ✅ **Checkpoint tagging** for context recovery
- ✅ Extractor-friendly output format (`FILE:`, `MODIFY:`, `COMMIT:`)
- ✅ Built-in safeguards: a11y, XSS, SQLi, input/output validation
- ✅ Clear anti-pattern blocking (test skipping, premature abstraction, etc.)

---

## 📂 Folder Structure Output

```txt
📁 /project
├─ 📄 index.ts
├─ 📄 types.ts
├─ 🧪 __tests__/
├─ 🧪 bdd/
├─ 📄 .env.example
├─ 📄 README.md
└─ ⚙️ .github/workflows/ci.yml
```

---

## 📌 Real-World Use Cases

- Build secure, testable GPT-generated microservices
- Auto-scaffold full-stack features with CI/CD triggers
- Generate clean TypeScript modules with enforced domain logic
- Integrate into any LLM pipeline (Custom GPTs, LangChain, etc.)

---

## 🔗 Also check out

🧩 [JSON Foundry VS Code Extension](#) — Visualize JSON as a mind map and instantly generate TypeScript interfaces

---

## 🛠️ Use it. Break it. Refactor it. Ship it.

---

MIT © 2025 Chinasani Karthik Reddy
