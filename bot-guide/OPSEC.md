# OPSEC Guide

This repo must stay sanitized.

## Never Post

- hostnames
- machine names
- usernames
- account names
- home directory paths
- local IP addresses
- internal repo names if they are not already public
- private branch names
- tokens
- keys
- screenshots with identifying data

## Always Prefer

- behavior over infrastructure
- failure mode over environment detail
- anonymized wording over exact local context

Bad:

```text
the bot broke access on HOSTNAME for USERNAME in /home/...
```

Good:

```text
the bot argued with the operator about access even after a working path existed
```
