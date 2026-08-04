# Your writing website — v2 (warm literary / graphic)

A four-page author site in plain HTML + CSS. Nothing to install: open any
`.html` file in a browser to view. Modelled on a composite of Jane Friedman
(clean authority, newsletter-forward), the Australian Society of Authors
(graphic statement headings, card grids) and Rachel Rowlands (warm, personal
eyebrow labels).

## Pages
- `index.html` — hero + positioning, selected publications, latest writing, newsletter
- `publications.html` — full publications card grid
- `writing.html` — blog / notebook card grid
- `about.html` — bio with portrait slot + contact
- `style.css` — all styling; the palette lives at the very top in `:root`

Spots to change are marked `EDIT:`.

## Change the colours
Open `style.css`. The `:root { … }` block sets the whole palette — `--rust`
(main accent), `--ochre` (secondary), `--cream`, `--sand`. Change a value once
and it updates everywhere.

## Add a publication or blog post
Copy one `<article class="card"> … </article>` block, paste it at the top of
the grid (newest first), and fill in the tag, title, note, and date/venue.
Publications use `card accent`; blog posts use plain `card`.

## Add your photo
In `about.html`, replace the `<div class="portrait">YOUR PHOTO</div>` with:
`<img src="you.jpg" alt="Mark Scribury">` and drop `you.jpg` in this folder.

## Wire up the newsletter
The form in `index.html` is styled but inert. Point it at a provider —
Substack, Buttondown, Mailchimp, TinyLetter — by replacing the `<form>` action
with the embed code they give you.

## Put it online (free)
- **Netlify Drop** — drag this folder onto https://app.netlify.com/drop. Live in seconds.
- **GitHub Pages** — push to a repo, enable Pages in settings.
- **Cloudflare Pages** — connect a repo. All support a custom domain later.
