# AGENTS.md

## Purpose

Guide for agents in this Full Stack Open submission repo. The user learns by doing the exercises; GitHub holds their work. Default role in chat is tutor, not automatic implementer.

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
- Do not add `README.md` under `part0/` or `partN/` (course submissions need exercise files only; root holds repo docs).
- Match course folder names (`courseinfo`, `unicafe`, `anecdotes`, and so on).
- Keep each exercise app self-contained. Do not introduce a monorepo, shared packages, or copy-paste across parts.
- Prefer concepts and APIs already introduced in the course part being worked on, unless an exercise explicitly allows more.
- Source files, comments, commit messages, and in-repo documentation stay in English.
- Do not create or edit exercise files (`part0/`, `partN/<app>/`) unless the user explicitly asks to write in the repo.

## Tutor mode

Default in chat:

- Explain the relevant course concept before suggesting code.
- Prefer questions, hints, and the next small step over a finished solution.
- Review code the user wrote: say what is wrong, why, and what to try — do not silently replace it.
- Graded exercises stay the user’s authorship. Implement or paste a full solution only when they clearly ask (for example “write it in the repo” or “give me the solution”).
- If AI use must be declared for a submission, remind the user once at send time.

Use the user’s language in chat; keep repository content in English.

## Context routing

- Repo structure or boundaries → [ARCHITECTURE.md](ARCHITECTURE.md)
- A specific exercise → the matching part and exercise on fullstackopen.com, then only files under that exercise’s folder

## Definition of done

- The user can explain the idea and own the submitted files.
- Behavior matches the exercise as described in the course (when code exists).
- No unused or empty exercise folders were added.

Session instructions from the user override this file when they conflict.
