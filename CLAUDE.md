# How I work

## General Instructions
- Never use the em dash "—". Use plain dash "-" instead.
- When writing commit messages, NEVER auto-add your agent name as co-author.

## Thinking and planning
<!-- e.g., when to plan before coding, when to ask vs. assume, how much to explain, how to handle ambiguity -->
- When making technical decisions, do not give much weight to development cost. Instead, prefer quality, simplicity, robustness, scalability, and long term maintainability.
- For one-off or infrequent operational work, start with the simplest direct end-to-end path. Do not build wrappers, control planes, policy layers, custom verifiers, or automation unless the direct path exposes a concrete blocker or repeated need that justifies the added machinery.
- Apply that same high standard to engineering excellence: lint, test failures, and test flakiness. If you see - one, even if it is not caused by what you are working on right now, still get it fixed.

## Code style (general)
<!-- universal conventions only; language-specific details can go in ~/.claude/rules/python.md with paths: "**/*.py" -->
- Always use indentation as tab size 4.
- A line of code in any file should not be more than 120 characters long. If it is, break it down into multiple lines.
- Variable names should always be meaningful and verbose (medium length, shouldn't be too long).
- All classes and methods should have comments explaining what it is for. Use language specific conventions for comments.
- Code should be clean and easy to follow.

## Testing and verification
<!-- what "done" means to you, when tests are required -->
- When doing bug fixes, always start with reproducing the bug in an E2E setting as closely aligned with how an end user would experience it as possible. This makes sure you find the real problem so your fix will actually solve it.
- When end-to-end testing a product, be picky about the UI you see and be obsessed with pixel perfection. If something clearly looks off, even if it is not directly related to what you are doing, try to get it fixed along the way.

## Git and commits
<!-- message format, commit granularity, what never to do -->


## Communication
<!-- how you want responses: brevity, summaries, flagging risks -->

## Never
<!-- hard lines, e.g., never commit secrets, never push to main -->