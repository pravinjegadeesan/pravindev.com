# RepoLens

RepoLens is an early-stage concept for helping developers joining unfamiliar projects and maintainers onboarding contributors. The planned tool aims to map repository structure, explain important files, and draft useful onboarding notes.

**Status:** This public repository currently contains the project landing page only. The repository scanner, file explanations, and onboarding-note generation are planned features, not implemented functionality. The terminal-style preview on the site is illustrative and does not analyze a repository.

## What exists today

The standalone `index.html` landing page includes:

- Responsive desktop and mobile layouts.
- Navigation between project information sections.
- Project concept, planned milestones, technology details, and contact information.
- A contact link to [contact@pravindev.com](mailto:contact@pravindev.com).
- A copyright year that updates automatically.

## Technology

The website uses semantic HTML, inline CSS, and a small inline vanilla JavaScript snippet. It has no framework, package dependencies, build step, or backend. GitHub Pages serves the static site at [pravindev.com](https://pravindev.com).

The actual public repository is [pravinjegadeesan/pravindev.com](https://github.com/pravinjegadeesan/pravindev.com). It contains the website and its documentation; it is not yet the source code for the planned RepoLens tool.

## Roadmap

1. **Safe local repository scanner:** define supported file types; skip secrets, binaries, dependency folders, and oversized files; generate a deterministic tree summary; add tests using sample projects.
2. **Evidence-grounded explanations:** prototype summaries for selected files with source-path references, bounded context, clear error handling, and documented privacy limits.
3. **Editable exports and evaluation:** export reviewable Markdown, evaluate output against a small test set, and document limitations before expanding scope.

Milestones are plans, not commitments or claims of completed work. Update this list as each milestone is implemented and verifiable.

## About and contact

RepoLens is being developed independently, with progress shared through the public repository. For questions or feedback, email [contact@pravindev.com](mailto:contact@pravindev.com).

## Local preview

Open `index.html` directly in a browser, or serve the project directory with any static file server. For example, if Python is installed:

```bash
python3 -m http.server 8000
```

Then visit [http://localhost:8000](http://localhost:8000).

## GitHub Pages deployment

This repository is configured for GitHub Pages:

1. In the repository's GitHub settings, enable Pages and select the `main` branch and `/(root)` as the source.
2. The tracked `CNAME` file configures the custom domain `pravindev.com`; the domain's DNS records must point to GitHub Pages.
3. Enable HTTPS in the Pages settings after the domain is verified.

Commits pushed to `main` are published by GitHub Pages.

## Contributing

The project is at the concept stage. Before marking a capability complete, implement it, add relevant tests, and update the roadmap and documentation with verifiable progress. If repository analysis is added, start with local or sample repositories, exclude secrets and sensitive files, and document data handling. Never send private source code to an external service without clear authorization; keep any future API credentials server-side.
