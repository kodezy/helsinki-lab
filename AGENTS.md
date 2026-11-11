# AGENTS.md

## Purpose

Repository map for coding agents helping with Full Stack Open exercises.

## Repository map

- Architecture and dependency rules: `ARCHITECTURE.md`
- Course: https://fullstackopen.com/en/ (Portuguese material: https://fullstackopen.com/ptbr/)

## Commands

There is no root toolchain. From the app directory of the current exercise:

```bash
npm install
npm run dev
```

Use that app’s `package.json` if scripts differ. Do not invent a repo-wide test or lint command.

## Core invariants

- Create `partN` / `partN/<app>` only when starting that work. Do not scaffold unused parts or empty apps.
- Name directories as the course shows (`part0`, `part1/courseinfo`, `part1/unicafe`, …).
- Keep each app self-contained. Do not add a root monorepo or share source across parts.
- Stay inside what the current part has taught, unless the exercise allows more.
- Repo files (code, comments, commits, README) stay in English.
- When solving, reviewing, or explaining an exercise: teach. State the idea, why the code is shaped that way, and how it maps to the course. Do not dump a finished solution with no explanation.
- Match the user’s chat language. Do not skip the explanation because the code is “simple”.

## Context routing

When changing layout, part boundaries, or how apps relate:
read `ARCHITECTURE.md`.

When the task is an exercise:
open the matching Full Stack Open part (English or `ptbr`) and work only on that exercise’s files.

Do not read all documentation before every task.

## Definition of done

- The named exercise works as the course describes.
- The user can explain the solution (agent explained it in the session).
- No leftover empty folders or unused apps.

## Local instructions

User chat in the session wins over this file.
