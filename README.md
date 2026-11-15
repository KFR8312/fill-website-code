> **Moved.** This code now lives in [askfill/fill-website](https://github.com/askfill/fill-website), and fill.work loads it from there. This copy is archived and no longer used.

# fill-website-code

CSS and JavaScript layered on top of the fill.work Webflow site: glass frames, hero motion, customer logos, agent rule cards and the other polish passes.

Webflow still owns the pages, text and base styles. These two files add to them.

| File | What it holds |
|---|---|
| `css/fill-site.css` | All added styles |
| `js/fill-site.js` | All added behaviour |

The heading type scale is not in here. It lives in its own embed in the Webflow Footer component and stays there.

## How the site loads it

Webflow loads both files from this repo through jsDelivr, pinned to a version tag. They are two registered site scripts (Webflow > Site settings > Custom code > Scripts):

| Script | Where | What it does |
|---|---|---|
| `fill site css` | Head | A tiny loader that adds `https://cdn.jsdelivr.net/gh/KFR8312/fill-website-code@vNN/css/fill-site.css` as a normal stylesheet, so the page renders with it from the start |
| `fill site js` | Footer | Loads `https://cdn.jsdelivr.net/gh/KFR8312/fill-website-code@vNN/js/fill-site.js` with an integrity hash, so the browser refuses a file that does not match |

The site's own head and footer code (consent, trackers, cookie banner, Intercom) is separate and untouched.

## Making a change

1. Edit the files and test on the Webflow staging site.
2. Commit, then tag the commit with the next version (`v23`, `v24` ...) and push the tag.
3. Register new versions of the two Webflow scripts with the new tag in the URLs. The JS needs its new integrity hash: `echo "sha384-$(openssl dgst -sha384 -binary js/fill-site.js | openssl base64 -A)"`.
4. Apply the new versions, remove the old ones, publish staging, test, then publish the live site.

## Undo

Apply the previous versions of the two scripts again and publish. Every version stays in this repo's history, and jsDelivr keeps serving old tags.

## Rules

- Prefix every new class. A short bare class name once collided with a Webflow class and hid a customer story.
- Never italic text. Straight quotes only.
- Nothing secret goes in here: the repo is public, and the same code is readable in any browser on the live site.
