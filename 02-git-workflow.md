# Git Workflow

## The Three Areas of Git

This is the most important Git concept.

```text
Working Directory
      ↓
Staging Area
      ↓
Repository
      ↓
Remote Repository
```

---

## 1. Working Directory

Where you edit files.

Example:

```bash
vi script.sh
```

This is your live workspace.

---

## 2. Staging Area

Also called:

```text
Index
```

Files prepared for commit.

Add files:

```bash
git add script.sh
```

Think:

> “I want this in my next commit.”

---

## 3. Repository

When you commit:

```bash
git commit -m "Added script"
```

Git saves a snapshot.

---

## 4. Remote Repository

Usually GitHub.

Push:

```bash
git push
```

Pull:

```bash
git pull
```

---

## Common Workflow

Step 1:

Edit files

Step 2:

```bash
git status
```

Check changes.

---

Step 3:

```bash
git add .
```

Stage changes.

---

Step 4:

```bash
git commit -m "message"
```

Save changes.

---

Step 5:

```bash
git push
```

Upload to GitHub.

---

## git status

Shows:

* modified files
* staged files
* untracked files
* branch info

Most used Git command.

---

## git diff

Shows:

> changes between working directory and staging area

Example:

```bash
git diff
```

Useful before committing.

---

## Easy Memory Trick

```text
Edit
 ↓
Add
 ↓
Commit
 ↓
Push
```
