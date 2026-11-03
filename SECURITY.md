# Security

## What the skill does

- It reads the code it reviews and runs only what's already installed: the project's tests, a small script, the type checker. It installs no packages, runs no install scripts, and runs nothing against production data or with live keys.
- Its network reads are the ones a reviewer makes: the pull request through `gh`, and a package's registry entry (`npm view`) when a dependency looks wrong. It posts nothing.
- When a review finds a secret, the report quotes it masked: the first four characters and the length.

## Reporting a problem in this repository

If an instruction could lead an agent to change, send or expose something it shouldn't, report it privately through [GitHub's private vulnerability reporting](https://github.com/arez-xd/what-breaks-in-ai-code/security/advisories/new). Please include the file, the request and what happened. You'll get an answer within a week.

## If a review finds a vulnerability

A review sometimes finds a key in shipped code, a route anyone can call, or data that's exposed. Rotate an exposed key first, fix the code, and keep the details out of public issues until the fix is live.
