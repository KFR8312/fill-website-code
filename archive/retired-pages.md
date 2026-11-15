# Retired pages (2026-11-15)

Taken off the site because no page links to them. They are drafts in Webflow, not deleted, and can be published again. Their full content is in Webflow and in the automatic backup from the publish before this one.

## Static pages (set to draft, moved into the Webflow folder "old")

They now sit in the existing password-protected `old` folder (Webflow folder ID 6772630c34939788e26d4d1c), next to 43 earlier retired pages. The URLs in the table are the ones they had while live.

| URL | Webflow title | Page ID | Why |
|---|---|---|---|
| /home-positioning | Fill \| home — Positioning study (software + operations) | 6ab043a3b700d13cd1ccc73c | Design study for the home page; nothing links to it |
| /task-bundle | Fill \| The task bundle | 6aa58d36642a2ad332ae2344 | Design study; nothing links to it |
| /home-soft-particle-spheres | Home — Soft particle spheres | 6aa48a84f59d5c30e1106299 | Design study; nothing links to it |
| /services | Services | 6772630c34939788e26d4d90 | Old page from 2023; nothing links to it |
| /size/scale-ups | scale ups | 677d2160275500b19ec4d87b | Old page from 2025; not in the menu, nothing links to it |
| /use-case/compliance | compliance | 6772630c34939788e26d4c4e | Old page from 2024; nothing links to it |
| /use-case/save | save | 6772630c34939788e26d4d8d | Old page from 2024; nothing links to it |

## CMS items (archived in the "Content posts" collection)

Old whitepaper download pages under /content-post/. One still had placeholder Latin text as its body.

| URL | Item ID |
|---|---|
| /content-post/selecting-the-right-solution-for-companies-with-contingent-workers | 6772630c34939788e26d5fbd |
| /content-post/the-future-of-hiring-and-its-impact-on-organizations | 6772630c34939788e26d5fb4 |
| /content-post/noba-bank-getting-their-external-talent-in-one-single-place-with-fill | 6772630c34939788e26d5f5a |
| /content-post/state-of-talent-2024 | 6772630c34939788e26d5f58 |
| /content-post/cracking-the-code-writing-the-perfect-job-ad | 6772630c34939788e26d5f5b |
| /content-post/changing-workforce | 6772630c34939788e26d5f59 |

## Kept on purpose although nothing links to them

| URL | Why it stays |
|---|---|
| /pricing | The site's structured data (Offer URLs) points to it; decide before removing |
| /bano-policy, /security/sub-processors-2026-10 | Legal text; stays until legal says otherwise |
| /search | Webflow's site search page |
| /change-log/* | Each entry is shown on the changelog page |

## Code removed from Webflow the same day

- Site scripts switched off: every version of hv2_tm_toggle, pquo_slider and pquo_accordion (their markup is on no page), and nav_v2_scroll_theme 1.0.0 and 1.1.0 (1.2.0 replaces them). Copies in `site-scripts/`.
- Site head code: three Heyflow widget scripts that loaded on every page and were used on none.
- Site footer code: an old Sendinblue chat script that was commented out.
- Footer 2027 component: the two embeds that now live in this repo (copies in `webflow-embeds/`).
