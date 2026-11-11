# Architecture

## Purpose

Store Full Stack Open submissions in the directory structure the course uses for GitHub-based review. Each exercise group is a small standalone application rather than a single unified codebase.

## Layout

```text
part0/              Part 0: notes and diagrams
partN/<app>/        Parts 1+: one app per exercise group
```

Examples for part 1: `courseinfo`, `unicafe`, `anecdotes`. Later parts follow the same pattern with the names given by the course.

The repository root holds documentation and ignore rules only. Application code and `node_modules` live under `partN/<app>/`.

## Boundaries

| Path | Responsibility |
| --- | --- |
| `part0` | Notes and diagrams; typically no `package.json`. |
| `partN` | Work for one course part. |
| `partN/<app>` | One exercise app: dependencies, build, and runtime. |
| Root | Docs and `.gitignore` only. |

Do not add `README.md` (or other repo docs) under `part0/` or `partN/`. The course submission layout is folders plus exercise content only; documentation for the repo lives at the root.

Do not place multiple parts in one app folder or merge unrelated exercises into a single project.

## Dependencies

Each app manages its own dependencies. Allowed libraries are those appropriate to the course part and the exercise. Avoid pulling in tools or patterns from later parts early.

The repository does not use a root workspace, shared `src/`, or cross-part imports.

## Verification

There is no repo-level build or test command. Validate by running the scripts in the app you changed—typically `npm run dev` and any tests that exercise adds.
