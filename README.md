# Star's Sweet Treats — Website

The live website for Star's Sweet Treats, a home bakery in Belleville, Ontario.
Live at **https://starssweettreats.ca** (GitHub Pages, custom domain via the `CNAME` file).

## Pages

- `index.html` — home: prices, how ordering works, questions (FAQ), contact
- `gallery.html` — photo gallery (38 photos)
- `packages.html` — Party & Event Packages
- `previews/` — internal draft and review pages. Not linked from the site navigation and kept out of search (`robots.txt` + noindex). Do not link these publicly.

## Other files

- `favicon.png`, `og-image.jpg` — site icon and social-share image
- `sitemap.xml`, `robots.txt` — search engine files
- All three pages carry Bakery structured data (JSON-LD) in the page head.

## How orders work

The site does not take orders itself. Every Order button links to the bakery's
order form (Jotform), which is where orders, deposits, and the orders ledger are
handled.

## Making changes

1. Edit the file and commit to `main` — GitHub Pages deploys automatically, usually within a couple of minutes.
2. Check the live site after each change to confirm the deploy landed.

Prices, flavours, packages, and ordering terms have a single source of truth
outside this repo (the project's Current State Brief, kept by the site admin).
Never change a price or term in these pages without it.

## Known issue

`gallery.html` embeds its photos directly in the file (about 4.7 MB total),
which makes the gallery slow on weak connections. Moving the photos to image
files under an `assets/` folder is a planned cleanup; nothing about the
gallery's look needs to change when it happens.
