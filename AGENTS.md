# AGENTS.md

This file provides guidance to AI agents when working with
code in this repository.


## Project Overview

This project was created from the Scaffold template and provides a foundation
for Shell scripts, PHP CLI applications, and/or NodeJS projects with integrated
testing, code quality tools, and CI/CD workflows.


## Documentation

If using the documentation site (Docusaurus):

```bash
cd docs
npm install
npm start # Local dev server
npm run build # Production build
npm run spellcheck # CSpell validation
```

Documentation deploys automatically on releases via GitHub Actions.


## Updating from the template

This project was generated from a template and can pull the template's latest
infrastructure (CI workflows, linting and test configuration, Docker, and docs)
at any time. When you are asked to "update scaffold", fetch the updater skill
from the template repository into the local `.claude/skills/` directory, then
invoke it:

1. Create the target directory if it does not exist:

   ```bash
   mkdir -p .claude/skills/update-consumer-scaffold
   ```

2. Download the skill:

   ```bash
   curl -sSL https://raw.githubusercontent.com/AlexSkrypnyk/scaffold/main/.scaffold/skills/update-consumer-scaffold/SKILL.md -o .claude/skills/update-consumer-scaffold/SKILL.md
   ```

3. Invoke the `update-consumer-scaffold` skill and follow its steps.

The skill directory is fetched on demand and is git-ignored - it is not
committed to the project.
