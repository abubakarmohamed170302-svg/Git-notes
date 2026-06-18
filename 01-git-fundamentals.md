# Git Fundamentals

## What is Git?

Git is a Version Control System (VCS).

Think of Git as:

> a time machine for your code.

Git allows you to:

* track changes
* save versions of your work
* go back to previous versions
* collaborate with others
* avoid losing work

---

## What is Version Control?

Version Control means:

> keeping track of changes made over time.

Example:

Today:

```bash
echo "Hello"
```

Tomorrow:

```bash
echo "Hello Abu"
```

Without Git:

* old version is lost

With Git:

* every version is saved

---

## Who Created Git?

Git was created by:

**Linus Torvalds** in 2005.

He also created:

**Linux**

Git was built to manage the Linux Kernel.

---

## Centralised vs Distributed Version Control

### Centralised

```text
Developer
   ↓
Server
```

Problems:

* single point of failure
* internet required

Examples:

* SVN
* CVS

---

### Distributed

Git is distributed.

Every developer has:

* full history
* all commits
* complete project

Example:

```text
Developer A ←→ Developer B
```

Benefits:

* works offline
* safer
* faster

---

## Git Tracks Changes, Not Files

Git does NOT track files.

Git tracks:

```text
Changes to files
```

Example:

Before:

```bash
echo "Hello"
```

After:

```bash
echo "Hello World"
```

Git records:

* what changed
* when
* who changed it

---

## Repository (Repo)

A repository is:

> a Git project.

Example:

```text
my-project/
```

Contains:

* files
* commits
* branches
* history

---

## Commit

A commit is:

> a snapshot of your project.

Think:

```text
Save game
```

but for code.

---

## Branch

A branch is:

> an independent line of development.

Used for:

* features
* bug fixes
* testing

---

## Clone

Clone means:

> downloading a repository.

Example:

```bash
git clone URL
```

---

## Push

Push means:

> upload local commits to remote repository.

Example:

```bash
git push
```

---

## Pull

Pull means:

> download and merge latest changes.

Example:

```bash
git pull
```

---

## Remote

A remote is:

> an external copy of your repository.

Usually GitHub.

Check remotes:

```bash
git remote -v
```

---

## The .git Directory

Created when you run:

```bash
git init
```

Contains:

* commit history
* branches
* configuration
* logs
* references

Think of it as:

```text
Git's brain
```

Never manually edit it.
