# AGENTS.md

## Purpose

Guide for agents working on Full Stack Open exercises in this repository.

## Repository map

- Layout and constraints: [ARCHITECTURE.md](ARCHITECTURE.md)
- Course material: https://fullstackopen.com/en/

## Commands

This repo has no root `package.json`. Part 0 is usually notes under `part0/` with no npm scripts. From part 1 on, run tooling inside the active exercise folder:

```bash
npm install
npm run dev
```

Other scripts come from that app’s `package.json` (for example `npm test`). Do not assume repository-wide lint or test commands exist.

## Core invariants

- Add `partN` and `partN/<app>` only when the user is starting that exercise. Do not create empty placeholder trees.
- Match course folder names (`courseinfo`, `unicafe`, `anecdotes`, and so on).
- Keep each exercise app self-contained. Do not introduce a monorepo, shared packages, or copy-paste across parts.
- Prefer concepts and APIs already introduced in the course part being worked on, unless an exercise explicitly allows more.
- Source files, comments, commit messages, and in-repo documentation stay in English.

## Working with the user

When helping on an exercise, explain what you are doing and why it fits the exercise—before or alongside the code—not only the final snippet. Use the user’s language in chat; keep repository content in English.

## Context routing

- Repo structure or boundaries → [ARCHITECTURE.md](ARCHITECTURE.md)
- A specific exercise → the matching part and exercise on fullstackopen.com, then only files under that exercise’s folder

## Definition of done

- Behavior matches the exercise as described in the course.
- The user can follow the reasoning for the solution.
- No unused or empty exercise folders were added.

Session instructions from the user override this file when they conflict.
