# Creating a Recticode challenge

This guide explains how to create and submit a new Recticode challenge.

Recticode challenges are intentionally broken systems that users must debug and fix themselves.

---

## Required repository structure

Your challenge repo must follow this structure:
```
src/
challenge.json
README.md
```

---

## src/

All application code must live inside the `src/` directory.

This is the **broken system** that users will run and fix.

Rules:
- All code must be inside `src/`
- Keep the system small and focused on one bug
- Avoid unnecessary complexity
- **Do not include tests, and definitely don't commit them do your repository**

Example:

```
src/
    main.py
    db.py
    queue.py
```

---

## challenge.json

This file contains the name of the challenge, so the CLI recognises the challenge when the user is in the directory.

Example:

```json
{
  "name": "job-queue"
}
```

---

## Tests

**You must NOT include tests in your repository, or commit them to your repository.**

Recticode uses internal private tests to validate all challenges.

Why:
- prevents users from seeing the solution
- ensures fair gameplay
- allows hidden edge cases and concurrency checks
- keeps difficulty consistent

You only describe behaviour of the bug, not test logic.

## README.md

You need to include a section in your README describing intended behaviour, for example:
- What the system should do when correct
- Known edge cases which break

This is the README users will see when they attempt your challenge, so make sure it is brief and clear.

## Submission process

- While creating your challenge, make sure you commit often so the users can see the process of the code being developed
- Push your repo to github 
- Submit it via the [Recticode "Create Challenge" form](https://www.recticode.com)
- We will then manually review your challenge, write internal tests, and approve or reject 
- If approved, your challenge will be added to Recticode

## Rules

Your challenge must:
- Run locally without external services
- Contain a real bug (not cosmetic or trivial)
- Be solvable without guessing
- Avoid network calls or external APIs

Do NOT:
- Include malicious code
- Include hidden dependencies
- Rely on randomness without control
- Include test suites
- Include commits in the repository which reveals the bug, or how to solve it

---

## summary
- You provide broken code.
- We defines correctness.
- Tests are always private and owned by Recticode (so don't write them, or commit them to your repo).
- Challenges must be small, focused, and reproducible

Good luck building a challenge, and we look forward to reviewing it!
