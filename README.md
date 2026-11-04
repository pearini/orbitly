# Orbitly — project and task management platform

A working web app for managing projects and tasks: dashboard, projects, kanban board with drag-and-drop, backlog, list, timeline (Gantt), all-tasks view, reports, a task drawer with checklist, comments and activity log, bulk actions, and an Armenian / English interface.

**Live demo:** https://pearini.github.io/orbitly/ (after enabling GitHub Pages, see below)

## Run it

Open `index.html` in any modern browser — no build step, no server, no dependencies. Data is stored in the browser (localStorage); the reset button next to the user avatar restores the sample data.

## Contents

| Path | What it is |
| --- | --- |
| `index.html` | The complete standalone app (markup, styles, logic, translations) |
| `design/App.dc.html` | The same app as a Claude Design canvas artboard |
| `design/*.dc.html` | Static reference screens (dashboard, board, timeline, projects, task drawer) |
| `design/canvas.json` | Canvas layout for the design file |

## Design system

- Font: Poppins (400, 500)
- Primary #6B5CE7 · Primary 700 #4A3DBB · Secondary gold #F7D84E
- Success #1E9E5A · Error #E2503B · Ground #F4F4F8 · Line #E4E4EC

## Publish with GitHub Pages

1. Push this repository to GitHub.
2. In the repository go to **Settings → Pages**.
3. Under **Build and deployment** choose **Deploy from a branch**, branch `main`, folder `/ (root)`, then **Save**.
4. After about a minute the app is live at `https://pearini.github.io/orbitly/`.

## Adding a language

All interface strings live in the `T` object in `index.html` (`T.en`, `T.hy`). Add a new key block (for example `T.ru`) with the same keys and extend the `toggleLang` function to cycle through it.
