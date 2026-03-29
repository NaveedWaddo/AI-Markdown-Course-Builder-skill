# 🧠 AI Markdown Course Builder

> A Claude skill that turns any software topic into a complete, GitHub-ready learning course — from zero to architect level.

---

## ✨ What It Does

You say:
> *"I want to go from zero to hero in Kubernetes"*
> *"I want to learn Go from beginner to advanced"*

Claude responds with:

- 📋 A **full syllabus** — Phases → Topics → Subtopics (beginner to architect)
- 📊 A live **`PROGRESS-TRACKER.md`** — tracks exactly where you are, with a built-in AI resume prompt
- 📁 A **GitHub-ready folder structure** — one `.md` file per topic, organized by phase
- 📝 **Deep notes per topic** — concept explanations, architecture diagrams, code examples, interview Q&A, scenario problems, quick revision cards
- 🤖 An **AI Resume Prompt** — if your context resets or you switch AI tools, paste it to continue seamlessly

---

## 🚀 Trigger Phrases

The skill activates **only** on explicit full-course requests:

| ✅ Triggers the skill | ❌ Does NOT trigger |
|---|---|
| "I want to go from zero to hero in X" | "How does X work?" |
| "I want to learn X from beginner to advanced" | "Explain X to me" |
| "Create a full course on X" | "What is X?" |
| "Build me a learning path for X from scratch" | "Help me fix my X error" |
| "I want to master X from the ground up" | "Quick question about X" |

Casual questions and single-topic queries are answered directly — the skill doesn't interrupt them.

---

## 📦 Installation

### Option 1 — Install the `.skill` file (Claude.ai)

1. Download [`ai-markdown-course-builder.skill`](./ai-markdown-course-builder.skill)
2. In Claude.ai, go to **Settings → Skills**
3. Click **Install Skill** and upload the file
4. Done — the skill is now active in your Claude workspace

### Option 2 — Manual copy

Copy the contents of [`SKILL.md`](./SKILL.md) into your Claude skill configuration directly.

---

## 🗂️ What a Generated Course Looks Like

```
my-kubernetes-course/
├── README.md
├── PROGRESS-TRACKER.md          ← Live tracker + AI resume prompt
├── phase-1-fundamentals/
│   ├── 01-what-is-kubernetes.md
│   ├── 02-architecture-overview.md
│   └── 03-installation-setup.md
├── phase-2-intermediate/
│   ├── 04-pods-and-deployments.md
│   └── ...
├── phase-3-advanced/
│   └── ...
├── phase-4-senior-production/
│   └── ...
├── phase-5-architect/
│   └── ...
└── resources/
    └── project-ideas.md
```

Each `.md` file contains:
- 🧠 Concept Overview
- 📖 In-Depth Explanation (with subtopics)
- 🏗️ Architecture diagrams (Mermaid)
- 🔄 Flow / Lifecycle diagrams
- 💻 Code examples (basic → real-world → anti-patterns)
- ⚙️ Configuration & Options
- 🧩 Patterns & Best Practices
- 🔗 How It Connects (mental map)
- 🎯 Interview Questions with model answers
- 🧠 Scenario-Based Interview Problems (senior/architect level)
- ⚡ Quick Notes — revision card
- 🔖 References & Further Reading

---

## 🔄 The Progress Tracker

`PROGRESS-TRACKER.md` is the most important file in any generated course. It:

1. Shows the full syllabus as a table with ⬜ / 🔄 / ✅ status per topic
2. Tracks your current position (Phase N · Topic X of Total)
3. Contains a copy-paste **AI Resume Prompt** — if your Claude context resets or you switch to another AI, paste it in and continue exactly where you left off

Example of the resume prompt inside the tracker:

```
I am learning Kubernetes using the AI Markdown Course Builder format.
- Last completed: Topic 4 — Pods and Deployments (04-pods-and-deployments.md)
- Next topic: Topic 5 — Services and Networking (05-services-networking.md)
Please generate the full .md notes file for Topic 5 in the standard format.
```

---

## 📄 Sample Output

See the [`sample-output/`](./sample-output/) folder for an example of a generated topic note.

---

## 🛠️ Skill File

The core skill logic lives in [`SKILL.md`](./SKILL.md). It defines:
- The 5-phase course structure
- The full `.md` topic template
- The `PROGRESS-TRACKER.md` format
- The "next" command behaviour
- Behavioral rules and edge cases

---

## 📝 License

MIT — use it, fork it, share it.

---

## 🤝 Contributing

Pull requests welcome. If you have ideas for improving the topic template, tracker format, or trigger logic, open an issue or submit a PR.
