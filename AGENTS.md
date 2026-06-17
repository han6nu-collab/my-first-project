# Project Notes

## Project Overview

This project is a small static personal homepage. It currently consists of a single `index.html` file plus repository metadata.

The page is written with plain HTML and inline CSS. There is no package manager, build step, framework, backend, or test runner.

## Current Structure

- `index.html`: Main and only webpage. Contains the full HTML, CSS, responsive layout, and back-to-top button.
- `.gitignore`: Ignores common OS files, editor settings, logs, dependencies, build output, environment files, coverage, and temporary files.
- `AGENTS.md`: Project-level instructions for Codex and other AI agents.

## GitHub

The repository is connected to:

`https://github.com/han6nu-collab/my-first-project`

The local `main` branch tracks `origin/main`.

## Page Behavior

- The page is a responsive personal homepage.
- It has a dark visual style with CSS variables for colors.
- Layout uses a centered `.page` container and a three-column `main` section on desktop.
- On screens below `820px`, sections stack into a single column.
- A fixed circular `.back-to-top` link points to `#top`.
- Smooth scrolling is enabled with `html { scroll-behavior: smooth; }`.

## Important Implementation Details

- Keep the project simple unless the user explicitly asks for a framework or build tooling.
- Prefer editing `index.html` directly for visual/content changes.
- Do not add `node_modules`, build output, or generated dependency files unless a real build setup is requested.
- Maintain responsive behavior for desktop and mobile.
- Use existing CSS variables and style conventions where possible.
- Cards and UI surfaces use small border radii around `8px`.

## Known Issue

The visible Chinese text in `index.html` currently appears mojibaked, for example text like `涓汉涓婚〉` and `浣犵殑鍚嶅瓧`. This looks like Chinese content that was decoded with the wrong character encoding.

When editing content, preserve UTF-8 and consider replacing the mojibake with readable Chinese copy if the user asks for content cleanup.

## Local Workflow

Open the page directly in a browser:

`C:\Users\zhangcc\Desktop\my-first-project\index.html`

Common Git workflow:

```powershell
git status
git pull
git add .
git commit -m "Describe change"
git push
```

Git may need to use the local proxy configured for GitHub:

`http://127.0.0.1:7890`

## Safety

Before making broad edits, inspect the current file contents and Git status. Do not remove unrelated user changes.
