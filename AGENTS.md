# Repository Guidelines

## Project Structure & Module Organization

This repository is currently a clean starting point. Keep the root focused on project metadata, documentation, and build configuration. As code is added, prefer a predictable layout:

- `src/` for application or library source code.
- `tests/` for automated tests that mirror `src/` structure.
- `assets/` for static files such as images, sample data, or fixtures.
- `docs/` for extended design notes, API references, or setup guides.

Avoid placing generated files, local caches, or editor-specific output in the repository.

## Build, Test, and Development Commands

No build system is configured yet. When one is introduced, document the exact commands here and keep them runnable from the repository root. Suggested examples:

- `npm test` or `gradlew test`: run the full test suite.
- `npm run build` or `gradlew build`: compile/package the project.
- `npm run lint` or `gradlew lint`: run static checks and formatting validation.

Prefer scripts or tasks with clear names so contributors do not need to memorize tool-specific flags.

## Coding Style & Naming Conventions

Follow the conventions of the language and framework selected for this project. Until a formatter is added, use consistent indentation, descriptive names, and small files with single responsibilities. Recommended defaults:

- Use 2 spaces for JavaScript/TypeScript/JSON/YAML and 4 spaces for Java/Kotlin/Python.
- Name files after the main class, component, or feature they contain.
- Use `camelCase` for variables/functions and `PascalCase` for classes/components.

Add formatter and lint configuration before the codebase grows beyond a few files.

## Testing Guidelines

Place tests under `tests/` or the framework-standard test directory. Test names should describe behavior, for example `creates_user_when_input_is_valid` or `UserServiceTest`. Cover new features, bug fixes, and edge cases before opening a pull request.

## Commit & Pull Request Guidelines

This directory has no Git history yet, so no existing commit convention is available. Use concise, imperative commit messages such as `Add initial user model` or `Fix validation error handling`.

Pull requests should include a short summary, the reason for the change, testing performed, and screenshots or logs when behavior or UI changes. Link related issues when available.

## Agent-Specific Instructions

Before making changes, inspect the current repository state and preserve user-created files. Keep edits narrowly scoped to the requested task, and update this guide when build tools, tests, or project structure are added.
