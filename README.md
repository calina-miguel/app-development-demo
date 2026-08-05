# Miguel Calina App Development Demo

Private portfolio showcase for a Flutter business app originally built as KnockQuest. This copy is intended to demonstrate product design, mobile navigation, deployment workflow, and cross-platform Flutter delivery in a controlled private repository.

## Overview

The app is a lead and territory management experience with mobile-first navigation, dashboard shortcuts, maps, follow-ups, quest tracking, and a staged GitHub Pages deployment setup.

## Highlights

- Mobile bottom navigation with quick access to Dashboard, Add Lead, Map, Follow Ups, and Export.
- Dashboard layout with lead pipeline, performance summaries, territories, integrations, subscriptions, quests, and lead details.
- Staging and production GitHub Pages workflows.
- Flutter web deployment with repository-aware base href handling.

## Tech Stack

- Flutter stable 3.44.8
- Dart 3.12.2
- Targets: Web, Android, iOS, Windows, Linux, macOS

## Live Demo

If enabled for this private repo, the deployed web app can be served from GitHub Pages. Public access is intentionally not the default for this showcase copy.

## Local Setup

```powershell
flutter pub get
flutter run -d chrome
```

For desktop testing:

```powershell
flutter run -d windows
```

## Quality Gates

Run the same checks used in CI:

```powershell
./scripts/run_github_ci_parity.ps1
```

## Deployment Notes

- `main` tracks the primary showcase build.
- `staging` is used for preview deployments.
- GitHub Actions handles release web artifacts and Pages publishing.

## Security

- No secrets, tokens, or credentials are committed to the repository.
- Environment-specific values should remain in GitHub Secrets or local `.env` files.
