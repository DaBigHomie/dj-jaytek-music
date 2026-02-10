---
applyTo: "**"
---

# Core Coding Directives

> Managed by DaBigHomie/documentation-standards — do not edit in target repos.

## Automation First
Prioritize creating automation scripts over suggesting manual terminal commands.

## FSD Architecture (Required for New Projects)
```
project-name/
├── features/     # Business features (isolated)
├── entities/     # Business entities (shared models)
├── shared/       # Shared utilities, constants, types
├── lib/          # External API wrappers
├── docs/         # Documentation
└── [entry-points]
```

## Portable Paths
- NEVER: `/Users/dame/...` or any hard-coded user path
- ALWAYS: `cd ../`, `./`, `$(pwd)`, `Path.home()`, `~`

## Research Before Planning
Use a research subagent (Plan agent) before creating implementation plans.

## Syntax Safety
Validate that all quotes (single/double) are closed before running shell commands.

## Concurrency
Implement locking or sequential logic to prevent parallel tasks from creating conflicting commits.
