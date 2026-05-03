# Architecture

## Purpose

This document describes the current repository structure of `yl-template-node`.

`yl-template-node` is a YardaLab Node.js / TypeScript template repository. Its purpose is to provide a clean starting point for future YardaLab-compatible Node.js / TypeScript projects.

At this stage, the repository is only in its initial structure/setup phase. This file documents what currently exists and provides a stable place for future architecture notes and file tree mapping as the template evolves.

This document is descriptive, not prescriptive. It should reflect the repository reality and should be updated when follow-up tasks add real behavior or new project structure.

## Current Repository Structure

```text
yl-template-node/
  docs/
    architecture.md
  src/
    .gitkeep
  tests/
    .gitkeep
  .gitignore
  LICENSE
  README.md
```

## Directory Responsibilities

### `docs/`

Contains repository-level documentation.

Currently, this directory contains the initial architecture document:

```text
docs/architecture.md
```

Future documentation may be added by follow-up tasks when the template behavior becomes more defined.

### `src/`

Reserved for future source code.

At this stage, no implementation files exist. The directory is kept as part of the initial project layout only.

Future tasks may add source files after the required setup and design decisions are in place.

### `tests/`

Reserved for future test files.

At this stage, no tests are implemented. The directory is kept as part of the initial project layout only.

Future tasks may add test files once package setup, tooling, and implementation details are defined.

### `.gitignore`

Defines files and directories that should not be committed to the repository.

It covers common Node.js / TypeScript generated files, dependency folders, build output, logs, local environment files, test coverage output, and tool caches.

### `LICENSE`

Defines the repository license.

The selected license for this repository is MIT.

### `README.md`

Provides a short, high-level overview of the repository.

The README intentionally describes only the current repository state and does not document future setup as already implemented.

## Out of Scope for Current Base Structure

The current base structure does not implement or configure:

* npm package setup
* `package.json`
* `package-lock.json`
* TypeScript configuration
* `tsconfig.json`
* npm scripts
* dependency installation
* source implementation files
* test implementation files
* YardaLab tooling integration
* commit message hook setup
* CI configuration
* release or publishing workflow

These areas belong to separate follow-up tasks.

## Future Mapping

Future tasks may expand this document with file tree mapping once the repository contains real template behavior.

The mapping may include:

* planned files
* implemented files
* related Jira tickets
* ownership of directories
* dependencies between tasks
* cross-cutting concerns

Initial mapping placeholder:

| Area                       | Path                   | Status      | Related ticket | Notes                               |
| -------------------------- | ---------------------- | ----------- | -------------- | ----------------------------------- |
| Root documentation         | `README.md`            | Existing    | YLDTE-74       | High-level repository overview      |
| License                    | `LICENSE`              | Existing    | YLDTE-74       | MIT license                         |
| Ignore rules               | `.gitignore`           | Existing    | YLDTE-74       | Common Node.js / TypeScript ignores |
| Architecture documentation | `docs/architecture.md` | Added       | YLDTE-75       | Current repository structure        |
| Source directory           | `src/`                 | Placeholder | YLDTE-58       | No source files yet                 |
| Test directory             | `tests/`               | Placeholder | YLDTE-58       | No test files yet                   |

This mapping should stay aligned with the actual repository state. Future-state behavior must not be documented as already implemented.

## Architecture Notes

The repository currently acts only as a base structure for a future Node.js / TypeScript template.

No runtime architecture exists yet because the repository does not currently contain package setup, TypeScript configuration, source code, tests, CI, git hooks, or YardaLab tooling integration.

Architecture decisions for those areas should be added only when the relevant follow-up tasks implement or formally define them.

## Update Rules

Update this document when:

* new directories or important files are added
* repository responsibilities change
* package setup is introduced
* TypeScript configuration is introduced
* YardaLab tooling integration is introduced
* git hook or CI behavior is introduced
* file tree mapping becomes more detailed

Do not update this document to describe planned behavior as if it already exists.
