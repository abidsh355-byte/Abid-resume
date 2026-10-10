# Abid Karim Shaikh — Resume Website

A single-page resume built with plain HTML and CSS (no images, no PDF). All resume text lives in `index.html`, so it is visible with Ctrl + U on the live site.

## How to update the site

Every change you commit on GitHub is picked up by Vercel and goes live in about a minute.

1. Open this repository on github.com and click `index.html`.
2. Click the pencil icon (Edit this file).
3. Press Ctrl + F to find the part you want to change (see below).
4. Make the change, then click **Commit changes**.
5. Wait about a minute and refresh your live site.

## Adding certifications and coursework

Search for `CERTIFICATIONS & COURSEWORK`. You'll find a hidden block under Education.

**First time only, to switch the block on:**
- Delete the line that says `<!-- HIDDEN-START`
- Delete the line that says `HIDDEN-END -->`

**Then fill in one entry per certificate or course:**

```html
<div class="cert rv">
  <div class="cert-name">NISM Series VIII: Equity Derivatives</div>
  <div class="cert-by">NISM</div>
  <div class="cert-when"><span class="n">2026</span></div>
  <div class="cert-status"><span>Completed</span></div>
</div>
```

- Replace the example text with your real certificate, issuer and year.
- For something you are still doing, write `Pursuing` instead of `Completed`.
- To add another, copy the whole `<div class="cert rv"> … </div>` block and paste it right below the last one.

## Other common edits

| To change… | Search for… |
|---|---|
| A skill | `class="chip"` inside the Skills section |
| Work experience bullet | the first few words of the bullet |
| Email address | `mailto:` (it appears in several places — change all) |
| Highlight tiles under your name | `class="tile` |

## Rules for this site

- No phone number, address or photo.
- No images or PDF embeds; text only.
- Keep every edit as plain text inside `index.html` so it shows up with Ctrl + U.
