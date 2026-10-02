# Olivia R. Alonso — Portfolio

A one-page portfolio site. No build tools needed: GitHub Pages serves `index.html` as-is.

## What's in this folder

- `index.html` — the whole site (layout, styles, and all text).
- `images/` — every picture on the site. File names match each piece's caption, with the brand first for case study work, for example `bcnj-billboard.jpg` or `arsa-recruitment-pitch-deck-1.jpg`.

## Editing text

Open `index.html` and find `const cases=[` near the bottom. Each case study (ARSA, Regionelle, BCNJ) has its title, intro, role, story, stats, and work list there. Additional work is in `const more=[` just below.

## Adding or swapping a picture

1. Put the image in `images/` (JPG around 1600–2000px wide keeps the page fast). Use lowercase names with dashes and no spaces.
2. In that case study's `work:[ ... ]` list, add or edit a line:

```js
{src:"images/bcnj-community-event-booth.jpg", label:"Community event booth", alt:"Describe the photo"},
```

Multi-page pieces use `pages:["images/a-1.jpg","images/a-2.jpg"]` instead of `src`. A line with `todo:"..."` shows a "Coming soon" placeholder; replace it with a real `src` when the photo is ready.

Tip: file names on GitHub are case-sensitive, so `Photo.JPG` and `photo.jpg` are different files.
