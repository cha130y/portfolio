# Portfolio Site

The personal portfolio of **Chanon Sawaengphon** — a full-stack web developer transitioning from six years in quality and process engineering (Thai Bridgestone, Thai Toray Synthetics) into TypeScript full-stack development after completing DevNest Tech School's Advanced Fullstack Bootcamp.

Single page, single file ([`index.html`](index.html)), no build tooling — see [Tech stack](#tech-stack) below.

## What's on the page

- **Hero** — name, role, tagline, and core stack badges (Next.js, React, NestJS, PostgreSQL, Prisma, Socket.IO, Docker), with links to email, GitHub, and LinkedIn.
- **About** — the career pivot from manufacturing QA/process engineering into software, plus quick facts (location, degree, certifications, languages).
- **Projects** — the two flagship projects:
  - **CBeave Auction Platform** — a solo-built, end-to-end real-time auction platform (Next.js, NestJS, Prisma, PostgreSQL, Socket.IO). Highlight: concurrency-safe bidding via per-auction WebSocket rooms + serializable DB transactions, plus anti-sniping clock extensions.
  - **BidNest — Auction & Marketplace** — a 5-developer team project where Chanon owns the real-time bidding module and acts as project-setup lead (pnpm monorepo, Dockerized 24-module NestJS backend, CI/CD).
- **Skills** — grouped by frontend, backend/API, database/ORM, auth/validation, testing, and DevOps/tooling.
- **Experience & Training** — timeline from the DevNest bootcamp back through the QA and process engineering roles.
- **Contact** — email, phone, GitHub, LinkedIn.

## Tech stack

- Plain HTML5 + CSS (custom properties for theming, CSS Grid/Flexbox for layout)
- No JavaScript, no framework, no bundler
- One external asset: the `Inter` font from Google Fonts

## Project structure

```
portfolio/
├── index.html   # Entire site: markup, CSS (in <style>), content
├── README.md
└── .gitignore
```

## Customizing content

Everything is in `index.html`, with the CSS in a `<style>` block at the top of `<head>`. To change content, search for the text you want to edit directly — it's plain HTML, no templating. The color palette is defined once as CSS custom properties near the top of the stylesheet (`--navy`, `--blue`, etc.) if you want to adjust the look. Update the "Live Demo" / "Source Code" links if either project's URL changes.

## Running & deploying

No build step required. Open `index.html` directly, or serve it locally with `npx serve .` / `python -m http.server`. Deploy as a static site on [Vercel](https://vercel.com) or [GitHub Pages](https://pages.github.com) — both work out of the box.
