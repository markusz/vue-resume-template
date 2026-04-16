# vue-resume-template

Personal resume site built on [Ryan Balieiro's vue-resume-template](https://github.com/ryanbalieiro/vue-resume-template).

## Run locally

```bash
npm install
npm run dev
```

## Deploy to Vercel

Push to `main` — Vercel picks it up automatically. No build config needed; Vite's default output (`dist/`) and `base: '/'` in `vite.config.js` are already correct for Vercel.

To deploy manually:

```bash
npm run build
vercel deploy --prod
```

## Making content changes

All content lives in `public/`:

| What | Where |
|---|---|
| Bio, social links | `public/data/sections/cover.json` |
| Work experience | `public/data/sections/experience.json` |
| Education | `public/data/sections/education.json` |
| Skills | `public/data/sections/skills.json` |
| Talks & papers | `public/data/sections/thoughtleadership.json` |
| Portfolio | `public/data/sections/portfolio.json` |
| Name, photo, contact | `public/data/info/profile.json` |
| Company logos & names | `public/data/info/places.json` |
| Profile photo | `public/images/pictures/` |
| Company logos | `public/images/places/` |

Sections reference companies via `@link{places.<id>}` — add new employers to `places.json` first.
