---
description: Create a git commit following conventional commits format
---

## Context

- Current git status: !`git status -uall`
- Current git diff (staged and unstaged changes): !`git diff HEAD`
- Recent commits for style reference: !`git log --oneline -5`

## Your task

Create a git commit following conventional commits format based on the changes shown above.

**Conventional Commits Format:**
`type(scope): description`

**Common types:**
- `feat`: new feature
- `fix`: bug fix
- `docs`: documentation changes
- `style`: formatting, missing semicolons, etc
- `refactor`: code change that neither fixes bug nor adds feature
- `test`: adding missing tests
- `chore`: maintain, deps, config changes
- `perf`: performance improvements
- `ci`: continuous integration changes
- `build`: build system changes

**Instructions:**
1. Analyze all staged and unstaged changes
2. Stage relevant files with `git add` if needed
3. Create a commit message with:
   - Type and optional scope
   - Imperative mood description (under 50 chars)
   - Optional body for complex changes (wrap at 72 chars)
4. Create the commit using a heredoc format
5. Verify success with `git status -uall`
6. Add ticket ID and title in the body of the commit message if applicable

**Arguments:** Optional commit message hint can be provided as `$ARGUMENTS`