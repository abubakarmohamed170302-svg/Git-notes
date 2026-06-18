# Real World Git Workflow

## What Git Looks Like at Work

Most teams use:

```text id="9t2mfw"
Feature Branch
 ↓
Commit
 ↓
Push
 ↓
Pull Request
 ↓
Review
 ↓
Merge
```

This is the standard workflow.

---

## Branch Protection

Many companies protect:

```text id="tx5pr0"
main
```

Meaning:

* no direct pushes
* PR required
* approvals required

Safer.

---

## Pull Requests

A Pull Request (PR) is:

> asking the team to review and merge your work.

Benefits:

* code review
* discussion
* quality control

---

## Code Reviews

Another engineer checks:

* code quality
* bugs
* security issues
* best practices

This improves code.

---

## CI/CD Integration

After push:

```text id="l0q8aw"
Build
 ↓
Test
 ↓
Scan
 ↓
Deploy
```

Git triggers automation.

Examples:

* GitHub Actions
* Jenkins
* GitLab CI

---

## Pre-Commit Hooks

Before commit:

```text id="6r0m7y"
Run checks
 ↓
Block bad commits
```

Examples:

* formatting
* linting
* secret scanning

---

## Team Collaboration Rules

At work:

Always:

* pull before pushing
* use feature branches
* write clean commit messages
* review code
* avoid force push

---

## Production Fix Example

Production issue:

```text id="w6gh7d"
Website down
```

Workflow:

```text id="0b5mfz"
git checkout -b hotfix
 ↓
Fix issue
 ↓
Commit
 ↓
Push
 ↓
PR
 ↓
Merge
 ↓
Deploy
```

Fast and safe.

---

## Real World Truth

Most Git work is:

```text id="v4nq2a"
small changes
small commits
small branches
frequent merges
```

This keeps everything stable.

---

## Golden Rule

Think:

```text id="w94bse"
Git is not just commands.
Git is teamwork.
```

That mindset matters most in DevOps.
