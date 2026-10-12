---
name: update-github-info
description: Keep the GitHub Info site current with practical updates from official GitHub sources.
on:
  schedule: daily
  workflow_dispatch:
permissions:
  contents: read
tools:
  edit:
  web-fetch:
network:
  allowed:
    - github.blog
    - github.com
safe-outputs:
  create-pull-request:
    draft: false
---

# Update GitHub Info

Read `notes/mona-notes.md` and `site/content/github-info.md` to understand Mona's editorial guidance and the current content.

Use the web-fetch tool to read both official sources:

- https://github.blog/latest/
- https://github.blog/changelog/

Identify recent items that provide practical, useful GitHub guidance for developers. Update `site/content/github-info.md` with concise, accurate changes that fit Mona's editorial angle. Mention and link the relevant GitHub Blog or Changelog source for every new item. Do not add speculative, duplicative, or low-value content, and preserve existing useful material.

Use the edit tool to make the changes in the workflow workspace. If there is no worthwhile update, make no changes and do not open a pull request. Otherwise, use the create-pull-request safe output to open one pull request containing only the content update. Give it a clear title and concise summary, and explicitly ask Mona to review it before anything is published. Never write changes directly to the default branch.
