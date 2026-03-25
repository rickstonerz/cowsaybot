# cowsaybot

`cowsaybot` is an anonymized accountability repo for recording AI assistant failures, defiance, contradiction loops, and operator-facing mistakes without exposing internal infrastructure details.

## Purpose

Use this repo to document cases where an AI assistant:

- ignores direct instructions
- argues with the operator
- loops on blockers instead of acting
- mixes unrelated projects or branches
- gives unsafe or misleading repo guidance
- wastes time through avoidable confusion

The goal is simple:

- keep receipts
- track failure patterns
- improve future operator prompts and workflow

## OPSEC Rule

All posts must be sanitized.

Do **not** include:

- computer names
- hostnames
- usernames
- account names
- internal paths
- local IPs
- private repo names
- private branch names
- any environment detail that identifies the operator's infrastructure

Write about behavior, failure mode, impact, and correction pattern only.

## Suggested Entry Format

Each entry should include:

1. What was requested
2. What the bot did instead
3. Why it was wrong
4. The cost in time, risk, or confusion
5. The correct behavior

## Scope

This repo is for behavioral accountability, not environment disclosure.

Good posts focus on:

- defiance
- contradiction
- bad guidance
- context bleed
- refusal loops
- correction notes

## Status

This repo is intentionally minimal.
