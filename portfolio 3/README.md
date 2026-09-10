# Ramalakshmi Saravanan — Portfolio

A single self-contained site: `index.html` (all CSS/JS is inline, no build step needed).

## How to view it
Just double-click `index.html` to open it in any browser. To deploy it for free, drag the folder into [Netlify Drop](https://app.netlify.com/drop), or push it to a GitHub repo and enable GitHub Pages.

## How to add your photo
Open `index.html`, find this block (Ctrl+F for `avatar`):

```html
<div class="avatar" aria-hidden="true">RS</div>
```

Replace it with:

```html
<div class="avatar">
  <img src="assets/your-photo.jpg" alt="Ramalakshmi Saravanan">
</div>
```

Then drop your photo file into the `assets` folder and update the filename above to match. A square, well-lit headshot works best (the frame is a 1:1 square).

## How to add your resume
Find the `Download Resume` area (there isn't one yet since no PDF was provided). To add it:
1. Put your resume PDF in the `assets` folder, e.g. `assets/resume.pdf`.
2. In the hero section, add a third button next to "View my work":
   ```html
   <a href="assets/resume.pdf" class="btn btn-ghost" download>Download Resume</a>
   ```

## How to add real project links
Search for `proj-link disabled` in `index.html` — there are 4 of them, one per project. Replace each with a real link once ready, e.g.:

```html
<a class="proj-link" href="https://github.com/Lakshmi-02-05/isl-translator" target="_blank" rel="noopener">View on GitHub →</a>
```

## Editing content
Everything is plain HTML — search for the text you want to change (e.g. your tagline, stats, skills) and edit it directly. No frameworks, no dependencies to install.

## Colors (if you ever want to tweak the palette)
All colors are defined once at the top of the `<style>` block under `:root`, so changing `--gold` will re-color every accent across the whole site consistently.
