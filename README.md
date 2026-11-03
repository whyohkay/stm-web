# Smart Task Manager

A **Flutter web deployment** from an AI-assisted task-management application project.

[Hosted web build](https://whyohkay.github.io/stm-web/) · [Project context](docs/PROJECT_CONTEXT.md) · [Nuttha's portfolio](https://github.com/Nuttha-lim/digital)

## My role

**Nuttha Limkhhunthammo:** directed an AI-assisted application build using Flutter/Dart, FastAPI and PostgreSQL, and gained an understanding of how the frontend, backend and database components fit together. The broader project also used Docker.

## What this repository contains

This repository publishes compiled Flutter output for GitHub Pages. It lets reviewers inspect the deployment structure and the custom push-notification service worker.

| File or directory | Purpose |
| --- | --- |
| `index.html` | Entry page with base path `/stm-web/` |
| `main.dart.js` | Compiled Dart application output |
| `flutter_bootstrap.js`, `flutter.js` | Flutter startup files |
| `canvaskit/`, `assets/`, `icons/` | Rendering runtime, fonts and bundled assets |
| `manifest.json` | Web app metadata |
| `serviceworker.js` | Push notification display and notification-click handling |
| `assets/NOTICES` | Bundled dependency notices |

The editable Dart sources, FastAPI backend, database schema, Docker configuration and automated tests are **not included** in this repository. GitHub may label it JavaScript because the Dart code has been compiled to JavaScript.

## Preview the existing build locally

Requires Python 3. Clone into a directory named `stm-web` so the existing base path resolves correctly:

```powershell
git clone https://github.com/whyohkay/stm-web.git
cd stm-web
py -3 -m http.server 8000 --bind 127.0.0.1 --directory ..
```

Open [the local preview](http://127.0.0.1:8000/stm-web/). On macOS/Linux, use `python3` instead of `py -3`.

This serves existing static files. It does not rebuild the application or start a backend. Backend-dependent flows and web-push delivery need their original services and configuration; their availability is not established by this repository.

## Review scope

- The repository demonstrates deployment artifacts and project context.
- `serviceworker.js` provides readable notification-handler code.
- It does not establish a reproducible full-stack source release, complete automated test coverage or production readiness.

For a source-code review of another project, see [CO Valley](https://github.com/Nuttha-lim/231-project), including Java sources, contribution details and a manual gameplay test plan.
