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

## Deploy for free — GitHub Pages

1. Create a new GitHub repo named exactly `<your-github-username>.github.io`
2. Push this project to it:
   ```bash
   git init
   git add .
   git commit -m "first commit"
   git branch -M main
   git remote add origin https://github.com/<your-github-username>/<your-github-username>.github.io.git
   git push -u origin main
   ```
3. In the repo, go to **Settings → Pages**, and under "Build and deployment" set the source to **GitHub Actions**. GitHub will detect the Astro project and suggest its Astro workflow — accept it.
4. Your site will be live at `https://<your-github-username>.github.io` within a couple minutes, at no cost.

If you'd rather use a custom domain later, you can add one under the same Pages settings — you'd just need to buy the domain separately (~$10–15/year) and point its DNS at GitHub.
