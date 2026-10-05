# Animesh Singh, portfolio

A small static site: one homepage and three case studies. Every page is self-contained, with its styles and script inside the file, so each one opens correctly on its own, in a preview, or on GitHub Pages. No build step and no dependencies.

## Files

```
index.html                      Homepage
case-fleet-dashboard.html       Case study 1
case-driver-alerts.html         Case study 2
case-khatabook-onboarding.html  Case study 3
images/                         Put your screenshots, videos and portrait here
resume.pdf                      Add this yourself (linked from the homepage)
```

## Before you publish

1. Open any page with `?check` at the end of the address, for example `index.html?check`.
   Every placeholder turns red, and case studies show writing guidance for each section.
2. Replace every highlighted item with real content, or delete it.
3. Replace the sample images with your real work (see below).
4. Add `resume.pdf` to the main folder.

## Replacing images

Sample images are drawn in code inside `<div class="media sample">…</div>` blocks.
Grey boxes are `<div class="media">Image: …</div>`. Replace either with:

```html
<div class="media"><img src="images/fleet-hero.jpg" alt="Fleet dashboard, final design"></div>
```

or, for a short screen recording:

```html
<div class="media"><video src="images/fleet-hero.mp4" autoplay muted loop playsinline></video></div>
```

Images look best at 16:10 (for example 1600 × 1000 px). Your portrait goes inside `<div class="avatar">` on the homepage.

## Adding a fourth case study

1. Copy any `case-*.html` file and rename it.
2. Replace its text and images.
3. Add a project to the Selected work section in `index.html` and link its "Read the case study" to the new file.
4. Update the "Next case study" card at the bottom of each case so they link in a loop.

## Changing the look

All colours are variables at the top of the `<style>` block in each page (`--bg`, `--ink`, `--soft`, `--muted`, `--tile`), with dark-mode values just below. Because every page carries its own styles, make the same change in all four files (find and replace works well).

## Publishing on GitHub Pages

1. Create a repository named `your-username.github.io`.
2. Upload everything in this folder, keeping the folder structure.
3. In the repository, go to Settings, then Pages, choose "Deploy from a branch" and select `main`.
4. Your site will be live at `https://your-username.github.io` within a few minutes.
