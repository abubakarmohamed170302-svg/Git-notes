# Git Best Practices

## Commit Often

Avoid huge commits.

Bad:

```bash id="y6pbw5"
git commit -m "3 weeks of work"
```

Good:

```bash id="7jv8m4"
git commit -m "Added login validation"
git commit -m "Added password reset page"
git commit -m "Fixed auth bug"
```

Why?

* easier debugging
* easier rollback
* easier review

---

## Use Meaningful Commit Messages

Bad:

```bash id="2m5wqe"
git commit -m "fix"
```

Bad:

```bash id="0a4g7l"
git commit -m "stuff"
```

Good:

```bash id="e8jqb6"
git commit -m "Fixed Docker container startup issue"
```

Rule:

Answer:

```text id="5xoqz6"
What changed?
```

---

## Keep Branches Small

Bad:

```text id="m3r3xw"
One branch for 3 months
```

Good:

```text id="i2d7mw"
Small branch
Quick merge
```

Benefits:

* fewer conflicts
* easier code reviews

---

## Pull Before Push

Before:

```bash id="8jkl4w"
git push
```

Do:

```bash id="bpl0hz"
git pull
```

This reduces merge conflicts.

---

## Check Status Often

Use constantly:

```bash id="v4z3m9"
git status
```

Shows:

* modified files
* staged files
* untracked files
* branch

Very important.

---

## Review Before Commit

Use:

```bash id="d83tx6"
git diff
```

Check:

* mistakes
* secrets
* wrong files

before committing.

---

## Use Feature Branches

Avoid:

```text id="s1h0mz"
working directly on main
```

Use:

```bash id="fh17z2"
git checkout -b feature-name
```

Safer.

---

## Avoid Force Push

Dangerous:

```bash id="w3t9r1"
git push --force
```

Can overwrite team history.

Use only when needed.

---

## Real World Workflow

```text id="ibw04f"
Create branch
 ↓
Make changes
 ↓
git status
 ↓
git add .
 ↓
git commit
 ↓
git pull
 ↓
git push
 ↓
Pull Request
 ↓
Review
 ↓
Merge
```

This is the most common workflow at work.
