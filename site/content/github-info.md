# GitHub Info

## Mona's editorial angle

Mona's website focuses on practical GitHub guidance backed by official references from:

- docs.github.com
- github.blog
- github.blog/changelog

## Current homepage themes

- GitHub collaboration basics: repositories, branches, pull requests, and merges.
- GitHub Copilot as an AI coding assistant across the IDE, CLI, and GitHub.
- GitHub Actions as the automation layer behind repository workflows.
- Recent GitHub Blog and Changelog stories worth watching.

## Recent updates worth watching

- **Push attribution for commits (limited public preview):** GitHub now records the authenticated user who pushed each commit and shows that pusher identity in the UI and API next to the author and committer. Because author and committer are client-supplied strings, a new ruleset condition, `Committer must match pusher`, can block spoofed commit identities. Source: [GitHub Changelog](https://github.blog/changelog/2026-10-12-push-attribution-public-preview).
- **Copilot client telemetry attribution:** Enterprise admins can use the `telemetry.capture.identity` managed setting to attribute Copilot activity to a user in OpenTelemetry data without collecting prompts, responses, or tool content. All capture classes are off by default. Source: [GitHub Changelog](https://github.blog/changelog/2026-10-12-client-telemetry-user-attribution-and-configurable-capture).
