# IceLimited SNS Media Downloader

This source repository is for a locally operated web application for downloading and processing media for a single user on macOS, Windows, and Linux.

It is part of the `sns-media-downloader-workspace`, which maintains CONTEXT.md, agent instructions, feature plans, and meeting records at the workspace root. Read the main context before starting work.

When checked out through the workspace, read [CONTEXT.md](../../CONTEXT.md), [AGENTS.md](../../AGENTS.md), and [MODEL-ROUTING.md](../../MODEL-ROUTING.md) at its root. If this repository is cloned separately, open the workspace repository `git@github.com:ice-limited/sns-media-downloader-workspace.git` to read those documents.

## Status

The project is in init planning; there is no application implementation or test evidence yet. In the workspace, [plan 001](../../plans/001-init-scope-architecture.md) is approved and its documentation is `done` after owner acceptance; the other 18 plans remain unapproved stubs. See the [plan index](../../plans/README.md) and [init roadmap](../../docs/init-project-roadmap.md). Acceptance of 001 does not approve those plans for implementation. The proposed structure has `apps/web` for Next.js Web+API and `apps/worker` for background jobs in one repository; neither directory nor actual dependencies have been created or selected.

**Do not create Git commits unless explicitly instructed.** Before each user-instructed commit, update the workspace and source repository CHANGELOG.md files as relevant to the changes.

The multilingual requirement starts UI and app-owned messages in EN/TH and allows additional languages later. See [019](../../plans/019-multilingual-en-th.md) and the [language architecture](../../docs/internationalization.md). The language foundation precedes the UI shell; no library has been selected and source implementation has not begun.

## Documentation language

English is the primary language for all project-authored documentation in this source repository, including future README, CONTRIBUTING, CHANGELOG, guides, API references, and documentation in other formats. Preserve technical identifiers, commands, original error text, quoted original names, and literal examples; Thai UI text and EN/TH examples need not be translated. Workspace documents remain in Thai under the [workspace policy](../../CONTEXT.md#นโยบายภาษาเอกสาร).

The owner selected the [MIT License](LICENSE) for the project. The app license does not grant rights to downloaded media; dependencies, binaries, and fonts have separate licenses that must be reviewed.
