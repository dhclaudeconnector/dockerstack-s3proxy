# Codex Project Rules (dockerstack-s3proxy)

These rules are mandatory for Codex in this project.

## 1) Always update `.opushforce.message`

- For every completed user task, Codex must update `.opushforce.message` before sending the final response.
- Do not skip this step, even for small edits.
- If no files were changed, still update `.opushforce.message` with a short note.

## 2) Message format

Use commit-ready content:

1. First line: `<type>: <short summary>`
2. Blank line
3. Flat bullet list of key changes

Suggested `type` values: `feat`, `fix`, `refactor`, `docs`, `chore`.

## 3) Completion gate

Codex should treat task as incomplete until `.opushforce.message` is updated to reflect the latest work.
