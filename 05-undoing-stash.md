# Undoing Changes & Git Stash

## Git Restore

Used to discard file changes.

Example:

```bash
git restore file.txt
```

Meaning:

```text
Throw away my changes
```

---

## Git Reset

Moves Git backwards.

---

## Soft Reset

```bash
git reset --soft HEAD~1
```

Removes commit.

Keeps changes staged.

---

## Mixed Reset

Default:

```bash
git reset HEAD~1
```

Removes commit.

Keeps changes unstaged.

---

## Hard Reset

```bash
git reset --hard HEAD~1
```

Dangerous.

Deletes:

* commit
* staged changes
* working changes

Gone.

---

## Git Revert

Safer than reset.

Creates a new commit that undoes another.

Example:

```bash
git revert commit-id
```

History stays intact.

Best for shared repos.

---

## Git Reflog

Shows every HEAD movement.

Example:

```bash
git reflog
```

Useful for:

* recovering lost commits
* seeing resets
* seeing rebases

Think:

```text
Git safety net
```

---

## Git Stash

Temporarily saves work.

Used when:

* not ready to commit
* need to switch branches

Save:

```bash
git stash
```

---

## View Stashes

```bash
git stash list
```

Example:

```text
stash@{0}
stash@{1}
```

---

## Apply Stash

```bash
git stash apply
```

Restores but keeps stash.

---

## Pop Stash

```bash
git stash pop
```

Restores and removes stash.

---

## Real World Example

Working on feature.

Urgent production issue.

Use:

```bash
git stash
```

Fix issue.

Come back:

```bash
git stash pop
```
