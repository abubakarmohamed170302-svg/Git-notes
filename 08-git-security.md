# Git Security & Secrets Hygiene

## Never Commit Secrets

Never push:

* passwords
* API keys
* tokens
* SSH private keys
* database credentials

Bad:

```bash id="p2w5g9"
AWS_SECRET_KEY=abc123
```

Dangerous.

---

## Why Is This Dangerous?

Git keeps history.

Even if deleted later:

```text id="3z8mle"
the secret may still exist in old commits
```

Attackers can find it.

---

## Use Environment Variables

Instead of:

```bash id="r4l2vn"
PASSWORD="secret123"
```

Use:

```bash id="y7w1qp"
PASSWORD=$PASSWORD
```

Better security.

---

## Use .gitignore

Prevent sensitive files being tracked.

Example:

```gitignore id="s4p8dk"
.env
credentials.txt
secrets.json
*.log
```

Git ignores them.

---

## Scan for Secrets

Many teams scan repositories for:

* AWS keys
* passwords
* API tokens
* private keys

This helps stop leaks.

---

## Principle of Least Privilege

If a credential is stolen:

```text id="8w7rjh"
it should have minimal permissions
```

Never give full admin access unless needed.

---

## Before Every Push

Ask:

```text id="f8zq3m"
Did I commit passwords?
Did I commit API keys?
Did I commit tokens?
Did I commit private keys?
```

Always check.

---

## Security Rule

Think:

```text id="2v1wpa"
Git history is permanent
```

Treat it seriously.
