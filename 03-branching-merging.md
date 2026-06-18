# Branching & Merging

## What is a Branch?

A branch is:

> a pointer to a commit.

Think:

```text
Safe workspace
```

Used to:

* build features
* fix bugs
* test changes

without touching main.

---

## Why Use Branches?

Without branches:

```text
Break production
```

With branches:

```text
Experiment safely
```

---

## View Branches

```bash
git branch
```

Shows:

```text
* main
  feature-branch
```

`*` = current branch

---

## Create Branch

```bash
git branch login-feature
```

---

## Switch Branch

```bash
git checkout login-feature
```

or:

```bash
git switch login-feature
```

---

## Create and Switch

```bash
git checkout -b login-feature
```

Creates and switches.

---

## Merge

Merging means:

> combining changes from one branch into another.

Example:

Switch to main:

```bash
git checkout main
```

Merge:

```bash
git merge login-feature
```

---

## Merge Workflow

```bash
git checkout -b login-feature

# make changes

git add .
git commit -m "Added login"

git checkout main

git merge login-feature
```

---

## Merge Conflicts

Happen when Git cannot decide which version to keep.

Example:

Main:

```bash
echo "Hello"
```

Feature:

```bash
echo "Hello World"
```

Git asks you to choose.

---

## Visual Branching

```text
main
 │
 ├── login-feature
 │
 └── bug-fix
```

---

## Why Branches Matter in Real Life

At work:

Never work directly on:

```text
main
```

Always:

* create feature branch
* commit
* push
* create pull request
* merge after review
