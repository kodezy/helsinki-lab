# Architecture

## Purpose

Hold Full Stack Open submissions in the directory layout the course uses for GitHub review. Each exercise app is independent.

## System map

**Planned** (created only when that part is in progress):

```text
part0/                 diagrams and notes for part 0
partN/<app>/           one app per exercise group (courseinfo, unicafe, ...)
```

**Implemented:**

```text
README.md
AGENTS.md
ARCHITECTURE.md
.gitignore
```

No shared `src/`, `apps/`, or root `package.json`.

## Boundaries

- `partN` — one course part. Do not mix parts in the same app folder.
- `partN/<app>` — one exercise group. Owns its own dependencies, scripts, and build.
- Root docs — repo purpose, agent rules, and this map. Not application code.

## Dependency direction

Allowed:

- An app depends on libraries introduced by that part (or allowed by the exercise).

Forbidden:

- Root workspace linking apps together.
- Sharing source across parts to “save time”.
- Libraries the current part has not introduced, unless the exercise says so.

## Verification

Architecture checks:
none

Fast check:
whatever `package.json` scripts exist in the app being edited (typically `npm run dev` / `npm test`)

Tests:
per-app, only when that app has tests
