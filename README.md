# Cursor Rules Repository

This repository contains a comprehensive set of rules, guidelines, and feature documentation for development projects. The rules are organized in the `.cursor/rules/` directory and cover all aspects of development, including project structure, environment variables, UI, backend, AI/LLM integration, and major features.

## Table of Contents
- [Repository Overview](#repository-overview)
- [Project Structure](#project-structure)
- [Rules Organization](#rules-organization)
- [Key Features](#key-features)
- [Development Guidelines](#development-guidelines)
- [Environment Variables](#environment-variables)
- [Testing](#testing)
- [Task Management](#task-management)

---

## Repository Overview
This repository defines rules and best practices for efficiently managing and developing modern applications using automation, AI, and productivity tools. The rules are written in Markdown with a `.mdc` extension and are intended to be referenced by both developers and AI agents.

## Project Structure
- Uses Turborepo with pnpm workspaces
- Main app is in `apps/web`
- Packages are in the `packages` folder
- Server actions are in `apps/web/utils/actions`
- All rules are in `.cursor/rules/`

Example structure:
```text
.cursor/
  └── rules/
      ├── core-rule.mdc
      ├── features/
      │   ├── cleaner.mdc
      │   ├── knowledge.mdc
      │   └── reply-tracker.mdc
      └── ...
```

## Rules Organization
- **Core & General**: Project structure, package installation, environment variables, logging, utilities, and task list management.
- **Frontend & UI**: Page structure, UI components (Shadcn, Tailwind), form handling, data fetching (SWR), and custom hooks.
- **Backend & API**: API routes, server actions, Prisma, Gmail API integration.
- **AI / LLM**: LLM implementation, prompt design, schema validation, logging, and dual LLM architecture for cost-effective and high-quality AI features.
- **Testing**: Vitest-based testing, colocated test files, and AI/LLM test guidelines.
- **Features**: Major features like Inbox Cleaner, Knowledge Base, and Reply Tracker are documented in `rules/features/`.

## Environment Variables
- Add new variables to `.env.example`, `apps/web/env.ts`, and `turbo.json` as described in `environment-variables.mdc`.
- Client-side variables must be prefixed with `NEXT_PUBLIC_`.

## Testing
- Use `vitest` for all tests.
- Colocate tests next to the tested file, except for AI/LLM tests, which go in `apps/web/__tests__/`.
- Follow best practices for mocking, test independence, and descriptive naming. See `testing.mdc` and `llm-test.mdc`.

## Task Management
- Track progress using markdown task lists (e.g., `TASKS.md`).
- Update task lists as you progress, marking completed tasks and adding new ones as needed.
- Document implementation details and relevant files. See `task-list.mdc` for guidelines.

---

## Contributing
1. Follow the rules and guidelines in `.cursor/rules/`.
2. Add new rules as `.mdc` files with clear descriptions and examples.
3. Update the rule index and relevant documentation as needed.

## License
This repository is provided for documentation and internal use. See individual files for more details. 
