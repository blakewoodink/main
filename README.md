# Blake Wood Ink

Astro site with a Markdown blog. Deploys to Vercel with zero config.

## Run it

    npm install
    npm run dev

## Deploy

Push to GitHub, import the repo in Vercel. It detects Astro automatically.
Update `site` in `astro.config.mjs` once your domain is connected.

## Your details

Edit `src/site.js` (email, Instagram, rate, tagline).

## Write a post

Add a Markdown file to `src/pages/blog/`. The file name becomes the URL
(`studio-news.md` → `/blog/studio-news`). Start it with:

    ---
    layout: ../../layouts/Post.astro
    title: Your title
    description: One line for the blog list and link previews.
    date: 2026-10-01
    draft: false
    ---

Set `draft: true` to keep a post off the lists while you work on it.
Images go in `public/` and are referenced as `/images/name.jpg`.

## Add work photos

Put photos in `public/work/`, then fill in `src` and `alt` for each piece in
`src/components/WorkGrid.astro`.
