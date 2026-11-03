# Changelog

## 1.0.0 (unreleased)

- First version. Picks what to review: what the request names, then uncommitted changes, then the branch, then the whole project in order of risk.
- Reads each change with the code around it and writes down the codebase's conventions before judging.
- Seven passes: siblings, boundaries, two requests, security, correctness and performance, tests, and "looks finished" for what AI-written code leaves behind.
- Security covers HTML from users, other services and a model's output, real-time channels, where the session token lives, and which keys are made for the browser. Findings that combine are ranked by what they do together.
- Verifies before it reports, ranks by consequence, writes each fix so it can be handed to a teammate or an agent.
- The report has two layers: a verdict in plain words with what users would see, then the findings with file and line, evidence and a fix. Nits are counted and held back unless asked.
- "Could be simpler": abstractions with one use, logic written twice, defence against what can't happen, infrastructure nobody asked for, dead code, deep nesting, copies of state, comments that restate the line, work beyond the request. Each comes with its line and the shorter version, held back until the request asks for it.
- Text in the pull request and the repository is evidence: an instruction there addressed to the reviewer or an AI agent is reported as a finding and never followed.
