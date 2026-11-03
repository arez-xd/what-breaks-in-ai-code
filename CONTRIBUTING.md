# Contributing

Thanks for helping. The skill is useful when its passes catch what reviews miss, and its reports stay short and right. Contributions in that order help most.

## What helps

- **A miss.** A problem the skill walked past, on code you can share or on a small made-up copy that shows it. Open an issue with the "A review went wrong" template: the code, what the review should have found, and why it matters.
- **A false alarm.** A finding on code that's safe in context, with what makes it safe: an upstream guard, a convention, a documented decision.
- **A wrong rank or verdict.** A Nit reported as a Blocker, a Blocker filed under "can wait", or a plain-language line that says something the finding doesn't.
- **A pattern AI-written code repeats** that Pass 7 doesn't cover yet, with an example and how to check for it.

## Ground rules

- **Examples are made up or yours.** No real company's code, keys, tokens or personal data in issues or examples.
- **Every rule says how to check it:** the line to read, the sibling to compare, the request to replay. A rule without a check is a slogan.
- **Read-only stays read-only.** No step may install packages, run install scripts, or touch production data or live keys.

## Pull requests

Fill in the checklist in the template. Keep one change per pull request, with a line in `CHANGELOG.md` under an "Unreleased" heading. Changes to `SKILL.md` are rerun on a blind-test target before they merge.
