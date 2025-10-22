<!--
Short, focused instructions for AI coding agents working on this repository.
Keep this file ~20-50 lines. Document only patterns discoverable from the repo.
-->
# Copilot instructions — Devops_Class_ENSI

Purpose
- This is a minimal example repository containing a single Java program `test_hello.java` that prints "Hello, World!". Use these notes to avoid making assumptions about build tooling or repository structure.

Quick start (PowerShell)
- Compile: `javac test_hello.java`
- Run: `java test_hello`

What you can expect from the codebase
- Single-file Java program at the repo root: `test_hello.java`.
- No build tool (no `pom.xml`, `build.gradle`, or `settings.gradle`). Do not introduce a build system without confirming with maintainers.

Project-specific conventions and gotchas
- The main class is declared as `test_hello` (lowercase with underscore). The filename matches the class name exactly. Java convention would use `TestHello` — do NOT rename the class or file without updating both the filename and any package statements.
- Keep changes minimal and self-contained. Because there is no CI or test harness, validate changes locally using the Quick start commands above.

When adding new Java code
- If introducing packages, create matching directories and add package statements at the top of each `.java` file.
- If you add a build tool (Maven/Gradle), include a short README section explaining how to build on Windows PowerShell and add a minimal CI workflow only after maintainers agree.

Files to inspect for context
- `test_hello.java` — the program entrypoint; the simplest example of how this repo runs.
- `README.md` — currently minimal; update if you add build tooling or additional structure.

Behavior expectations for PRs from AI agents
- Small, focused changes only. Run `javac`/`java` locally to verify output.
- Add or update `README.md` when changing developer workflows (for example, adding Maven/Gradle).
- If creating a new top-level directory structure, explain the reason in the commit message.

If unclear, ask the maintainer before
- Converting the project to a multi-module Java project.
- Adding CI workflows, dependency managers, or infrastructure files.

Contact / next steps
- Ask the repo owner which Java style (naming, packaging) they prefer before large refactors.
