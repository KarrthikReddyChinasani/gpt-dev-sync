# 🧠 GPT Dev Sync

Turn GPT into a structured software engineer — not just a code generator.

What started as a small VS Code extension project turned into something bigger.

---

## 📖 Backstory

Last week, I built a VS Code extension to visualize JSON as a mind map and generate TypeScript interfaces. It was a learning experiment — I just wanted to understand how extensions work under the hood.

But while building it, I kept asking GPT to help scaffold things.

That’s when I noticed something strange.

The code GPT gave me looked fine at first… but under the hood?

- ❌ No tests
- ❌ No clear structure
- ❌ No CI/CD awareness
- ❌ No validation or security
- ❌ No long-term maintainability

It could write code — but it couldn’t engineer.

That’s when it clicked:

> GPT doesn’t need better prompts. It needs a process.

---

## 🧠 Introducing GPT Dev Sync

This project defines a set of engineering heuristics — rules and structure — to guide GPTs into producing **reliable, testable, CI-ready software**.

### ✨ Key Features

- ✅ TDD / BDD / PDD enforced
- ✅ Test visibility modes (stealth to battle-ready)
- ✅ CI/CD setup triggers when deployable
- ✅ Output formatted for clean Git extraction
- ✅ Built-in anti-pattern filters
- ✅ Security and validation enforcement
- ✅ Full traceability using checkpoint tags

---

## 🔗 Available Guides

- [Heuristics Guide](./heuristics.md) – Full engineering ruleset and test enforcement

---

Use it. Break it. Refactor it. Ship it. 🚀


---

## 🔗 Additional Links

- 🗂️ [View on GitHub](https://github.com/karrthikreddychinasani/gpt-dev-sync)
- 🧩 [JSON Foundry VS Code Extension](https://marketplace.visualstudio.com/items?itemName=karthikchinasani.json-foundry)



---

❤️ Made with love by [Karthik Reddy](https://github.com/karrthikreddychinasani)
