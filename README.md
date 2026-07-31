# Morgan Pfaff — Personal Site

Built with [Astro](https://astro.build). Four pages: Home, About, Projects, Contact.

## Run it locally

You'll need [Node.js](https://nodejs.org) installed (v18+).

```bash
npm install
npm run dev
```

Then open the URL it prints (usually `http://localhost:4321`).

## Edit content

- `src/pages/index.astro` — Home
- `src/pages/about.astro` — About
- `src/pages/projects.astro` — Projects
- `src/pages/contact.astro` — Contact
- `src/layouts/Layout.astro` — shared nav, footer, and all styling (colors, fonts, spacing)

Add a new page by creating a new `.astro` file in `src/pages/` and adding a link to the `nav` array in `Layout.astro`.

## Deployment

This repo already includes `.github/workflows/deploy.yml`, which builds and deploys the site automatically on every push to `main`.

One-time setup on GitHub (already done for this site, listed here for reference):

1. Repo name must be exactly `<your-github-username>.github.io`
2. In the repo, go to **Settings → Pages**, and under "Build and deployment" set the source to **GitHub Actions**
3. Push access requires a [Personal Access Token](https://github.com/settings/tokens) with both `repo` and `workflow` scopes (the `workflow` scope is specifically required because this repo's push touches a file inside `.github/workflows/`) — use the token in place of your password when Terminal prompts for one

After that, any push to `main` triggers a new deploy automatically — check the repo's **Actions** tab to watch it run. Live site: `https://morganpfaff1.github.io`

If you'd rather use a custom domain later, you can add one under the same Pages settings — you'd just need to buy the domain separately (~$10–15/year) and point its DNS at GitHub.
