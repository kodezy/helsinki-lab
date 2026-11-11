# helsinki-lab

Exercise submissions for [Full Stack Open](https://fullstackopen.com/en/). Directories follow the course’s recommended layout for GitHub review.

Add folders when you start each part or exercise group.

## Layout

```text
part0
part1
  courseinfo
  unicafe
  anecdotes
part2
  courseinfo
  phonebook
  countries
```

`part0` holds notes and diagrams. From part 1 on, each exercise folder is its own app with a `package.json`.

Full Stack Open does not require a `README` inside `part0`, `part1`, or any `partN/<app>` folder. Keep only exercise files and app code there. Repository-level docs stay in the root (`README.md`, `ARCHITECTURE.md`, `AGENTS.md`).

## Development

From part 1:

```bash
cd part1/courseinfo
npm install
npm run dev
```

There is no root `package.json` or shared scripts.

## Submission

1. Push to this repository.
2. Mark exercises complete in the [submission system](https://studies.cs.helsinki.fi/stats/courses/fullstackopen).

See [submitting exercises](https://fullstackopen.com/en/part0/fundamentals_of_web_apps#submitting-exercises) on the course site.
