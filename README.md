# Bar Inventory API

Backend service for **Bar Inventory**, an agentic software development project.

This repository will hold the REST API that backs the Bar Inventory mobile apps
(Android / iOS). No application code has been generated yet. It will be added
through the project's agentic workflow.

## Technology stack

- Language: Kotlin
- Framework: Spring Boot
- Database: PostgreSQL

## Branch strategy

- `main`: production / release branch
- `dev`: integration branch
- `feat/*`: feature branches, created from `dev` and merged back into `dev` via pull request

Releases are promoted from `dev` to `main`.

## Related repositories

| Repository | Purpose |
| --- | --- |
| [bar-inventory](https://github.com/kaanf/bar-inventory) | Central workspace: product design, PRD, architecture and shared CI/workflow |
| [bar-inventory-api](https://github.com/kaanf/bar-inventory-api) | Kotlin + Spring Boot backend (this repository) |
| [bar-inventory-kmp](https://github.com/kaanf/bar-inventory-kmp) | Kotlin Multiplatform mobile app (Android / iOS) |

Each repository is independent with its own Git history. Product and
architecture decisions live in the central workspace repository. This
repository implements the backend side of those decisions.

## Secrets

Never commit credentials, tokens, keystores or environment files. Provide
configuration through environment variables or a local, git-ignored config.
