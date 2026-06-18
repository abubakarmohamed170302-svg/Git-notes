# Git History & Rebase

## Viewing Git History

Git stores every commit in history.

Think of it like:

```text
Project timeline
```

Every commit is a checkpoint.

---

## Why History Matters

History helps you:

* track changes
* see who changed what
* restore old versions
* debug problems

---

## git log

View full history:

```bash
git log
```

Shows:

* commit ID
* author
* date
* commit message

Example:

```text
commit abc123
Author: Abu
Added backup script
```

---

## git log --oneline

Shorter view:

```bash
git log --oneline
```

Example:

```text
abc123 Added backup
def456 Added calculator
ghi789 Initial commit
```

Much easier to read.

---

## git log --graph

Shows branch history visually:

```bash
git log --graph --oneline --all
```

Example:

```text
* abc123 Added feature
|\
| * def456 Bug fix
|/
* ghi789 Initial commit
```

Useful for understanding merges.

---

## What is Rebase?

Rebase means:

> moving your commits onto another base.

Used for cleaner history.

---

## Why Rebase?

Without rebase:

```text
A---B---C main
     \
      D---E feature
```

After merge:

```text
A---B---C
     \   \
      D---E Merge Commit
```

Messy.

---

With rebase:

```text
A---B---C---D---E
```

Cleaner.

---

## Rebase Command

Switch branch:

```bash
git checkout feature
```

Rebase:

```bash
git rebase main
```

Moves feature commits on top of main.

---

## Interactive Rebase

Used to edit commits.

Example:

```bash
git rebase -i HEAD~3
```

Used for:

* squash commits
* rename commits
* remove commits

---

## Squash

Combines commits.

Before:

```text
Add script
Fix typo
Fix typo again
```

After:

```text
Add script
```

Cleaner history.

---

## Merge vs Rebase

Merge:

* keeps full history
* safer

Rebase:

* cleaner history
* rewrites commits

Beginner rule:

Use merge first.

Learn rebase after.
