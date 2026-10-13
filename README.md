# RepoLens

RepoLens is an early-stage project exploring ways to help developers understand unfamiliar codebases. This repository currently contains its responsive project landing page; the repository-scanning and documentation features described on the site are planned, not implemented.

## Project status

The landing page introduces the problem RepoLens hopes to address and outlines a possible path toward an MVP:

1. Build a safe repository scanner and test it against sample projects.
2. Explore contextual explanations with references to source files.
3. Evaluate the output and support editable documentation exports.

The terminal-style preview on the page is illustrative only. It does not analyze a repository or represent a working RepoLens tool.

## Landing page

The page is a standalone `index.html` file built with HTML, CSS, and a small inline script. It has no build step, package dependencies, or backend. Its current features include:

- Responsive layout for desktop and mobile.
- Navigation links to sections of the page.
- A copyright year that updates automatically.

### Preview locally

Open `index.html` directly in a browser, or serve the project directory with any static file server. For example, if Python is installed:

```bash
python3 -m http.server 8000
```

Then visit [http://localhost:8000](http://localhost:8000).

## Deployment

This repository is set up for GitHub Pages. To publish it:

1. In the repository's GitHub settings, enable Pages and select the `main` branch and `/(root)` as the source.
2. The tracked `CNAME` file configures the custom domain `pravindev.com`. Configure the matching DNS records with your domain provider if they are not already set up.
3. Enable HTTPS in the Pages settings once the domain configuration is verified.

Any new commit pushed to `main` will be published by GitHub Pages.

## Contributing

The project is at the concept stage. Before treating a proposed capability as complete, implement it, add relevant tests, and update the roadmap and documentation to reflect verifiable progress.

If repository analysis is added, begin with local or sample repositories, exclude secrets and sensitive files, and document what data is processed. Do not send private source code to an external service without clear authorization. Any future API credentials must remain server-side and must not be included in browser code.
