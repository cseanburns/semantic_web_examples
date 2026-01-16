# Repository Guidelines

## Project Structure & Module Organization
- Root HTML pages live in the repository root (e.g., `index.html`, `news.html`, `tables_forms.html`). These are standalone examples for the course.
- Shared styles live under `css/` (currently `css/style.css`). Keep reusable styles here rather than inlining.
- Media assets (images, audio, video) live under `media/` and are referenced from the HTML pages.

## Build, Test, and Development Commands
- `python3 -m http.server 8000`: Serve the repository as a static site for local testing. Visit `http://localhost:8000/index.html`.
- Open a single file directly in a browser for quick checks (e.g., `index.html`). Use a server when testing relative paths to `media/` or `css/`.

## Coding Style & Naming Conventions
- HTML: 4-space indentation, one element per line, and lower-case tags/attributes.
- CSS: 4-space indentation for properties and consistent brace placement.
- File names: lower-case with underscores for multiword examples (e.g., `two_column_flex.html`).
- Keep example pages focused: one concept per file when possible, and include semantic HTML5 structure (`header`, `nav`, `section`, `article`, `footer`).

## Testing Guidelines
- There is no automated test suite in this repo.
- Validate changes by opening the affected page(s) in a browser and checking layout, links, and media loading.
- If you add JSON-LD examples, verify correctness with a schema/JSON-LD validator before committing.

## Commit & Pull Request Guidelines
- Commit messages are short, imperative, and lower-case (e.g., “added flex examples”, “removed unused css”). Avoid trailing periods.
- PRs should describe the learning goal of the change, list the files touched, and note which page(s) to review.
- Include screenshots for visual/layout changes so reviewers can quickly confirm appearance.

## Configuration & Content Notes
- Keep external dependencies minimal; examples should run offline after cloning.
- Prefer relative links within the repo and avoid hard-coding absolute paths.
