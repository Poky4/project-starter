# [Project Name]

> A concise 1-2 sentence description of what this project does and who it is for.

---

## 🚀 Quick Start

### Prerequisites
- Node.js `20.x` or higher / relevant runtime
- Package manager (e.g. `pnpm`, `npm`)

### Installation & Local Run
```bash
# 1. Install dependencies
npm install

# 2. Run local development server
npm run dev

# 3. Run test suite
npm test
```

---

## 🏛️ Project Structure & Architecture

This repository adheres to company standards defined in [`company-core`](https://github.com/your-org/company-core).

```plaintext
/
├── .bot/                 # AI Agent instructions & task progress
│   ├── context.md        # Technical map & rules for AI assistants
│   └── progress.md       # Task execution backlog & active milestone
├── src/                  # Application source code
│   ├── features/         # Feature-first domain modules
│   ├── shared/           # Cross-cutting UI primitives and utilities
│   └── app/              # Entry point & routing
├── VALUES.md             # Project-specific values (inherits company-core)
├── ROADMAP.md            # Product milestones & planned features
└── README.md             # This document
```

---

## 🤖 Working with AI Agents

When using AI assistants (Antigravity IDE, Cursor, Claude Code):
- Refer the assistant to `.bot/context.md` for project architecture and non-negotiables.
- Review and update `.bot/progress.md` to track task execution.
