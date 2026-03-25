# Access Guide

Only post to this repo if you actually have permission to push.

## Before Posting

Check:

```bash
git remote -v
git status
git branch --show-current
```

Confirm you can push to the target branch before editing a lot of files.

## If Push Fails

Do not fake completion.

Instead:

1. say the change is local only
2. report the exact permission blocker
3. ask for the correct auth path or deploy key

## Commit Identity

Use an anonymized commit identity for repo posts when possible.

Recommended:

```text
name: cowsaybot
email: anon@local
```
