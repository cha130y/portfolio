# Portfolio Site

A single-file, self-contained portfolio page (`index.html`) — no build step, no dependencies beyond one Google Fonts stylesheet. Content pulled directly from your resume and both project repos, so nothing here overclaims what's in CBeave/BidNest.

## Deploy it — pick one

### Option A: Vercel (recommended, free, ~5 minutes)
1. Create a new GitHub repo (e.g. `cha130y/portfolio`) and push this folder to it:
   ```bash
   git init
   git add .
   git commit -m "Initial portfolio site"
   git branch -M main
   git remote add origin https://github.com/cha130y/portfolio.git
   git push -u origin main
   ```
2. Go to [vercel.com](https://vercel.com), sign in with GitHub, click **Add New → Project**, and import the `portfolio` repo.
3. Vercel auto-detects it as a static site — just click **Deploy**. No framework preset or build command needed.
4. You'll get a URL like `portfolio-cha130y.vercel.app`. You can rename the project (Settings → General → Project Name) to get a cleaner subdomain, e.g. `chanon-dev.vercel.app`, or attach a custom domain later if you buy one.

### Option B: GitHub Pages (also free)
1. Push this folder to a GitHub repo named exactly `cha130y.github.io` (your GitHub Pages user site), or to any repo and enable Pages for it in Settings → Pages → Deploy from branch → `main` / root.
2. Your site will be live at `https://cha130y.github.io` (or `https://cha130y.github.io/<repo-name>` for a project repo).

Either option is fine — Vercel is slightly faster to set up and matches the stack you already use for CBeave/BidNest.

## After it's live

- Add the link to your resume's contact line (next to GitHub) and to your LinkedIn profile.
- Update the "Live Demo" / "Source Code" links in `index.html` if either project's URL ever changes.
- If you get a LinkedIn URL you want listed, add it next to the GitHub link in the header CTA row and the footer contact row.

## Customizing

Everything is in one file, `index.html`, with plain CSS in a `<style>` block at the top — no build tools involved. To change content, search for the text you want to edit directly. The color palette is defined once at the top of the CSS as CSS variables (`--navy`, `--blue`, etc.) if you want to adjust the look.
