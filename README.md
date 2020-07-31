# PR-Assigner
Open-source PR code review assignment manager

## Problem Statement
GitHub has a premium [code review assignment](https://docs.github.com/en/github/setting-up-and-managing-organizations-and-teams/managing-code-review-assignment-for-your-team) tool ([acquired from Pull Panda in June 2019](https://github.blog/2019-06-17-github-acquires-pull-panda/)), but it's not available for free accounts. It  requires a GitHub Teams account for members in your organization, which costs $4/user/mo -> $60/mo for a dev team of 15.

PR-Assigner is a free, custom, open-source version of the code review assignment tool, built with GitHub Actions.

## Project Plan (Draft)
- In CODEOWNERS file, assign code ownership of repository directories/files
- Create GitHub Action to run automatically each time a PR is opened
- Assign reviewer based on various factors
  - Ownership of code (already know it/should know it)
  - Previous PR contributions (load balance)
  - Indicated availability (based on team)

### Extensions
- Direct slack message notifications
  - (TBD) Create custom CODEOWNERS-SLACK file, where we map github usernames to slack usernames

