# repo-posture-audit

I built this as part of my GitHub Developer Program portfolio. It reads a repository through the GitHub API and scores the security posture a maintainer actually controls: whether the default branch is protected, whether a SECURITY.md tells researchers where to report a problem, whether private vulnerability reporting is switched on, and what the secret scanning signals say. One target repo in, one plain report out.

Status: scaffold. The interface is defined and the audit engine is the next build step.

## What it will do

- Read branch protection on the default branch through the GitHub API
- Check for a SECURITY.md and a working private reporting route
- Report the state of private vulnerability reporting and secret scanning where the API exposes them
- Print one scored report, with the evidence behind each line of the score

Built by Gavin Blacklock (Epsilon0xCell).
