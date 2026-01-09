# Repository Guidelines

## Project Structure & Module Organization
This repository is currently minimal and contains a single `README.md`. As the project grows, keep a predictable layout. Recommended defaults:
- `src/` for application or library code.
- `tests/` or `__tests__/` for automated tests.
- `docs/` for longer-form documentation.
- `assets/` for static files (images, fixtures, data).
If you introduce a new top-level directory, add a brief note to `README.md` and update this guide.

## Build, Test, and Development Commands
No build system or scripts are configured yet. If you add tooling (e.g., npm, Make, Poetry), document the exact commands here and in `README.md`. Example formats to include once available:
- `npm run dev` — start the local development server.
- `npm test` — run the full test suite.
- `make build` — produce production artifacts.

## Coding Style & Naming Conventions
There is no formatter or linter configured. Keep new files consistent with existing style and add tooling as the codebase grows. Suggested defaults until a tool is chosen:
- Use spaces (not tabs) and keep indentation consistent within a file.
- Prefer clear, descriptive names: `user_profile.ts`, `TemplateRenderer`, `render_template`.
- Keep line length reasonable (around 100 characters) unless a language standard dictates otherwise.
- 思考、回复、文档与代码注释尽可能使用中文。

## Testing Guidelines
No test framework is currently configured. When adding tests:
- Place tests in `tests/` or alongside modules with `.test` or `.spec` suffixes (e.g., `renderer.test.ts`).
- Keep unit tests fast and deterministic; add integration tests only when needed.
- Document any coverage expectations in this file once established.

## Commit & Pull Request Guidelines
Git history currently contains only “Initial commit,” so no convention is established. Use short, imperative commit messages (e.g., “Add template renderer”) and group related changes. For pull requests:
- Provide a clear description of what changed and why.
- Link related issues or tickets if they exist.
- Include screenshots or examples for user-facing changes.

## Security & Configuration Tips
Do not commit secrets or local configuration. Use environment variables or example config files (e.g., `.env.example`) and document required settings in `README.md`.
