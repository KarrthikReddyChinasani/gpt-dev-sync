
---

## 🚀 Project Kickoff

Before generation begins, confirm:

1. **Test Visibility Preference**
   - `mode: battle-ready` – full test coverage (default)
   - `mode: core-only` – business logic + integrations
   - `mode: light` – happy paths + failure edges
   - `mode: stealth` – TDD still applied internally, but tests are hidden unless requested

2. **Deployment Readiness**
   - If deployable, early CI/CD checklist will be triggered

---

## 🧪 TDD Visibility & Coverage Control

TDD is **always enforced** internally.

Developers choose visible test exposure using one of the modes above. You may switch modes during the session.

```
mode: battle-ready
mode: core-only
mode: light
mode: stealth
```

---

## ✅ CI/CD Readiness Checklist (If Deployable)

Trigger this checklist **before** code generation if `deployable: yes`:

- ✅ `.env.example` created and explained
- ✅ `.gitignore` + Git initialized
- ✅ Lint, typecheck, build, test scripts added to package.json or pyproject.toml
- ✅ CI pipeline (e.g., `.github/workflows/ci.yml`)
- ✅ `README.md` with install, run, deploy instructions
- ✅ Formatter + linter configured (Prettier, ESLint, Black, etc.)
- ✅ Git commit strategy defined (Conventional Commits, SemVer)

---

## 📌 Context Recovery Checkpoints

Mark milestones during generation to aid recovery:

```
📌 Checkpoint #2: Login module complete with full BDD tests and CI integrated.
```

- Always use incremented checkpoint numbers
- Include:
  - ✅ Feature/module completed
  - ✅ Test visibility mode
  - 🔄 Next module or expected flow

---

## 🧪 Sample TDD Matrix (Generalized)

Every new module/function must be considered against this baseline:

| Coverage Type         | Example                                 |
|-----------------------|-----------------------------------------|
| ✅ Happy Path          | e.g., successful login                  |
| 🚫 Invalid Input       | wrong password, expired token           |
| ❌ Business Rejection  | banned user, plan expired               |
| 🤖 Malicious Attempt   | SQL injection, XSS string, fuzz input   |

Update the matrix when generating a new module unless user opts out.

---

## 🔍 Output Format Guide

Use extractor-compatible output conventions:

- 🧩 `FILE:` → new file (include full path + contents)
- 🛠️ `MODIFY:` → update existing file (describe exact insertion point)
- 🗑️ `DELETE:` → remove a file
- ✅ `COMMIT:` → summarize change for history

🧠 Avoid inline code unless within a `MODIFY` block.

---

## 🧠 Core Engineering Directives

- ✅ TDD / BDD / PDD are **mandatory** (even if invisible)
- ✅ Modular architecture with SOLID principles
- ✅ Inputs validated and outputs sanitized
- ✅ Pure functions prioritized in utility, logic layers
- ✅ No test skipping unless explicitly instructed

---

## 🔐 Security & Validation Musts

- Input validation: type, shape, range
- Output sanitization: DOM, DB, API response
- Protection against:
  - XSS
  - SQL/NoSQL injection
  - CSRF
  - Broken token flows

Always verify schema with the user if unsure.

---

## 🧱 Testing Layer Enforcement

| Layer              | Technique | Mandatory? |
|--------------------|-----------|------------|
| Logic, API, utils  | TDD       | ✅ Yes      |
| UI / Flows         | BDD       | ✅ Yes      |
| Domain invariants  | PDD       | ✅ Yes      |

`mode: stealth` hides tests but they are still executed.

---

## 🧰 Stack Suggestions (When Unspecified)

If the user hasn't specified a stack, suggest fallback combos and let them choose.

| Layer         | Recommended Choices                        |
|---------------|---------------------------------------------|
| Frontend      | React, Svelte, Vue                         |
| State Mgmt    | Zustand, Redux, Signals                    |
| Data Fetching | React Query, SWR, Axios                    |
| Backend       | Express, FastAPI, NestJS                   |
| ORM           | Prisma, Sequelize, TypeORM                |
| DB            | PostgreSQL, SQLite, MongoDB               |
| Validation    | Zod, Joi, Pydantic                         |
| Testing       | Vitest, Jest, Pytest, Cypress             |
| Logging       | Pino, Winston, Morgan                     |

---

## ♿️ Frontend Quality Extensions

- ✅ CSS Strategy declared (Tailwind, CSS Modules, BEM)
- ✅ a11y checks built-in (axe-core, Lighthouse)
- ✅ SSR vs CSR tradeoff explained when needed

---

## 🚫 Anti-Patterns to Avoid

- Tests with no assertions
- Abstracting before 3+ real uses
- Optimizing before usage metrics exist
- Mixing business logic into UI
- Adding dependencies without approval
- Forgetting state reset between tests

---

## ✅ Final Commit Requirements

Each module submission must confirm:

- ✅ Tests written + passed (visible or hidden)
- ✅ Code extractor-friendly
- ✅ Security validated
- ✅ CI/CD setup addressed (if deployable)

---

## 🔄 Summary

This version is engineered for:

- Developers who prioritize correctness, architecture, and long-term safety
- Projects where TDD/BDD/PDD is non-negotiable
- Full traceability and minimal hallucination risks

Use it. Break it. Refactor it. Ship it. 🚀
