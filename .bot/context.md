# AI Context & Codebase Map

> **Instruction for AI Agents**: Read this file first before executing any tasks. This file establishes the operational boundaries, technical stack, and architecture of this repository.

---

## 1. Project Purpose
- **Description**: [Brief 1-2 sentence description of what this project does and the main problem it solves].
- **Primary Audience / Users**: [e.g. Internal operators / B2B customers / mobile users].

---

## 2. Technical Stack & Tooling
- **Language**: TypeScript (strict mode enabled, zero `any`)
- **Framework**: [e.g. Next.js 14 / Vite React / Node Fastify]
- **Styling**: [e.g. Vanilla CSS / Tailwind CSS / Design System Tokens]
- **Validation**: Zod (all external data must be validated)
- **Testing**: [e.g. Vitest / Playwright]
- **Package Manager**: [e.g. npm / pnpm / yarn]

---

## 3. Directory Map & Boundaries
```plaintext
/
├── src/
│   ├── features/       # Feature-first domain modules (components, hooks, api, types)
│   │   └── [feature]/  # Isolated feature domain with explicit index.ts exports
│   ├── shared/         # Reusable primitives ONLY (Button, Modal, dateUtils)
│   └── app/            # Route configuration & global providers
├── .bot/
│   ├── context.md      # This file
│   └── progress.md     # Active task tracker and completion history
```

---

## 4. Non-Negotiable Rules for AI Agents
1. **Show, Don't Tell**: When writing code or refactoring, provide complete, working implementations with zero placeholders or `// TODO` stubs.
2. **Strict Type Safety**: Never use `any`. Define explicit interfaces or Zod schemas.
3. **No Hidden Errors**: Never write empty `catch {}` blocks. Every failure must be explicitly handled or logged.
4. **Colocation**: Keep feature-specific components, tests, and types inside their feature folder. Do not pollute `shared/` with one-off code.
5. **Always Update Progress**: When completing a task, immediately update `.bot/progress.md`.

---

## 5. Key Commands
- **Dev Server**: `npm run dev`
- **Type Check**: `npx tsc --noEmit`
- **Lint**: `npm run lint`
- **Test**: `npm test`
- **Build**: `npm run build`
