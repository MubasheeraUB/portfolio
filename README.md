# Mubasheera U B — Portfolio

Personal portfolio built with **Next.js 16**, **React 19** and **Tailwind CSS 4**.
Single page: Hero · About · Skills · Projects · Experience · Contact.

## Edit the content

All text, links, skills, projects and experience live in one file:

```
src/data/profile.ts
```

Other files you may want to change:

| What | Where |
| --- | --- |
| Resume PDF | `public/Mubasheera_UB_Resume.pdf` (replace, keep the name) |
| Project screenshots | `public/projects/*.svg` (placeholder mockups) |
| Colours / font | `src/app/globals.css` (`--color-brand-*`) |
| SEO title / description | `src/app/layout.tsx` |

### Replace the project screenshots (recommended)

The images in `public/projects/` are placeholder mockups. Take real screenshots
(1280×800 works best), save them as e.g. `public/projects/blitzcart.png`, and
update the `image` path for that project in `src/data/profile.ts`.

## Run locally

Requires Node.js 20.9+.

```bash
npm install
npm run dev
```

Open http://localhost:3000

## Deploy for free on Vercel

1. Create a new repository on GitHub (e.g. `portfolio`) and push this folder:
   ```bash
   git init
   git add .
   git commit -m "Initial portfolio"
   git branch -M main
   git remote add origin https://github.com/MubasheeraUB/portfolio.git
   git push -u origin main
   ```
2. Go to https://vercel.com and sign up with GitHub (Hobby plan is free).
3. Click **Add New → Project**, pick the `portfolio` repo, keep the defaults, click **Deploy**.
4. After about a minute the site is live at `https://<project-name>.vercel.app`.
   Rename the project in **Settings → General** to get `mubasheera.vercel.app` if it is free.
5. Put the final URL in `siteUrl` in `src/data/profile.ts`, then commit and push.
   Every push to `main` redeploys automatically.

Optional: add a custom domain later in **Settings → Domains**.
