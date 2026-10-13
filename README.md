# RepoLens portfolio starter

A minimal, responsive landing page for RepoLens, a proposed open-source developer tool concept.

## Important before publishing
This site intentionally distinguishes proposed capabilities from shipped functionality. Do not claim that the product is live, that it has users, or that it uses Claude until those claims are true.

## Customize first
1. Replace `REPLACE_WITH_YOUR_EMAIL` in `index.html` with your public contact email.
2. Add your real GitHub repository link after you create it. Do not link to a repository that does not exist.
3. Update the roadmap as work is completed, and link to evidence (commits, tests, releases, demo).
4. If you choose a different project name, update the title, metadata, and page copy.
5. Add a privacy notice before collecting user data or accepting repository uploads.

## Preview locally
Open `index.html` in a browser. No build tools or dependencies are required.

## Deploy
- GitHub Pages: push `index.html` to a repository and enable Pages in repository settings.
- Netlify or Vercel: import the repository and deploy it as a static site.

## Suggested MVP implementation
- Start with a local scanner for public/sample repositories.
- Ignore secrets, environment files, binaries, dependency folders, and large files.
- Add deterministic repository structure output and tests before adding an LLM.
- Add Claude API calls only after defining input limits, error handling, privacy boundaries, and cost controls.
- Use an environment variable for the API key on the server; never expose a secret API key in browser JavaScript.
- Evaluate generated explanations for factual accuracy and source-path grounding.

## Program applications
A portfolio can explain your project, but it does not guarantee acceptance into a startup program or free credits. Apply using accurate information and follow the program's current eligibility terms.
