# Smart Task Manager

Smart Task Manager is a task management application built with Flutter/Dart, FastAPI and PostgreSQL. This repository hosts its compiled Flutter web build on GitHub Pages.

[Web application](https://whyohkay.github.io/stm-web/) · [Source code](https://github.com/Nuttha-lim/smart-task-manager) · [Project details](docs/PROJECT_CONTEXT.md) · [Portfolio](https://github.com/Nuttha-lim/portfolio)

## My contribution

I used AI assistance to build the application and learn how its frontend, API and database connect. I worked with Flutter/Dart, FastAPI, PostgreSQL and Docker during the project.

## Repository contents

| File or directory | Purpose |
| --- | --- |
| `index.html` | Entry page with base path `/stm-web/` |
| `main.dart.js` | Compiled Dart application |
| `flutter_bootstrap.js`, `flutter.js` | Flutter startup files |
| `canvaskit/`, `assets/`, `icons/` | Rendering runtime, fonts and bundled assets |
| `manifest.json` | Web app metadata |
| `serviceworker.js` | Push notifications and notification-click handling |
| `assets/NOTICES` | Dependency notices |

The [source repository](https://github.com/Nuttha-lim/smart-task-manager) contains the editable Flutter application, FastAPI backend, database migrations and tests.

## Local preview

Install Python 3 and clone the repository into a directory named `stm-web`. The existing base path requires this directory name.

```powershell
git clone https://github.com/whyohkay/stm-web.git
cd stm-web
py -3 -m http.server 8000 --bind 127.0.0.1 --directory ..
```

Open the [local preview](http://127.0.0.1:8000/stm-web/). On macOS or Linux, use `python3` instead of `py -3`.

This command serves the static web build. Features that use the API or push notifications require the original backend services and configuration.
