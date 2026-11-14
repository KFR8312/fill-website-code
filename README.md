# fill-website-code

CSS and JavaScript layered on top of the fill.work Webflow site: glass frames, hero motion, customer logos, agent rule cards and the other polish passes.

Webflow still owns the pages, text and base styles. These two files add to them.

| File | What it holds | Where Webflow loads it |
|---|---|---|
| `css/fill-site.css` | All added styles | Site settings > Custom code > Head |
| `js/fill-site.js` | All added behaviour | Site settings > Custom code > Footer (before `</body>`) |

## How the site loads it

Webflow loads the files from this repo through jsDelivr, pinned to a version tag:

```html
<!-- Head -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/KFR8312/fill-website-code@v21/css/fill-site.css">
<!-- Footer -->
<script src="https://cdn.jsdelivr.net/gh/KFR8312/fill-website-code@v21/js/fill-site.js" defer></script>
```

## Making a change

1. Edit the files and test on the Webflow staging site.
2. Commit, then tag the commit with the next version (`v22`, `v23` ...).
3. Change the tag in the two Webflow lines and publish.

## Undo

Point the two Webflow lines back at the previous tag and publish. Every version stays in this repo's history.

## Rules

- Prefix every new class. A short bare class name once collided with a Webflow class and hid a customer story.
- Never italic text. Straight quotes only.
- Nothing secret goes in here: the repo is public, and the same code is readable in any browser on the live site.
