# Advanced Git

## Git Cherry-Pick

Copies one specific commit.

Example:

```bash
git cherry-pick commit-id
```

Used when:

* you only want one commit
* not whole branch

---

## Git Amend

Fix your last commit.

Change message:

```bash
git commit --amend -m "New message"
```

Add forgotten file:

```bash
git add file.txt
git commit --amend --no-edit
```

Useful for quick fixes.

---

## Forking

A fork is:

> your own copy of someone else’s repository.

Used in open-source.

Workflow:

```text
Original Repo
     ↓
Fork
     ↓
Make Changes
```

---

## Pull Requests (PR)

A Pull Request means:

> asking to merge your changes.

Workflow:

```text
Branch
 ↓
Commit
 ↓
Push
 ↓
Open PR
 ↓
Review
 ↓
Merge
```

Used in nearly all teams.

---

## Trunk-Based Development

Main branch is the trunk.

Developers:

* make small changes
* merge quickly

Benefits:

* fewer conflicts
* faster releases

Rule:

```text
Small branches
Short-lived branches
Fast merges
```
