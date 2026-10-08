[README.md](https://github.com/user-attachments/files/33212382/README.md)
# Olivia R. Alonso — Portfolio

A one-page portfolio site. No build tools needed: GitHub Pages serves `index.html` as-is.

## What's in this folder

- `index.html` — the whole site (layout, styles, and all text).
- Image files (`.jpg`) — every picture on the site, saved next to `index.html`. File names match each piece's caption, with the brand first for case study work, for example `bcnj-billboard.jpg` or `arsa-recruitment-pitch-deck-1.jpg`.

## Editing text

Open `index.html` and find `const cases=[` near the bottom. Each case study (ARSA, Regionelle, BCNJ) has its title, intro, role, story, stats, and work list there. Additional work is in `const more=[` just below.

## Adding or swapping a picture

1. Upload the image next to `index.html` (JPG around 1600–2000px wide keeps the page fast). Use lowercase names with dashes and no spaces.
2. In that case study's `work:[ ... ]` list, add or edit a line:

```js
{src:"bcnj-community-event-booth.jpg", label:"Community event booth", alt:"Describe the photo"},
```

Multi-page pieces use `pages:["a-1.jpg","a-2.jpg"]` instead of `src`. A line with `todo:"..."` shows a "Coming soon" placeholder; replace it with a real `src` when the photo is ready.

Tip: file names on GitHub are case-sensitive, so `Photo.JPG` and `photo.jpg` are different files.

## Planned updates (copy-and-paste ready)

Edit `index.html` right on GitHub: click the file, then the pencil icon. Use Ctrl+F (Cmd+F on Mac) to find the line, replace it, then click **Commit changes**. Upload the image first, with exactly the file name shown.

**BCNJ community event booth photos (done).** Two photos are already in `index.html`: `bcnj-community-event-booth-1.jpg` (the booth setup, retouched and leveled) and `-2.jpg` (visitors at the booth, showing the staff T-shirt). To swap one, upload a new photo with the same file name.

**Gender-affirming surgeon recruitment brochure.** Upload `gender-affirming-surgeon-recruitment-brochure-1.jpg` and `-2.jpg` (front and inside), then replace
`{cat:"Print", label:"Gender-affirming surgeon recruitment brochure"},`
with
`{cat:"Print", pages:["gender-affirming-surgeon-recruitment-brochure-1.jpg","gender-affirming-surgeon-recruitment-brochure-2.jpg"], alt:"Gender-affirming surgeon recruitment brochure", label:"Gender-affirming surgeon recruitment brochure"},`
(One-page version: use `src:"gender-affirming-surgeon-recruitment-brochure.jpg"` instead of `pages:[...]`.)

**New ARSA conference booth photo.** No code change needed: upload the new photo named exactly `arsa-conference-exhibitor-booth.jpg` and GitHub replaces the old one. If your computer still shows the old photo, do a hard refresh (Ctrl+Shift+R or Cmd+Shift+R).

**Practice-match kiosk lead number (after its first conference).** In `index.html`, find `captures leads at the booth.` and change the end of that sentence to `captured [X] surgeon leads at its first conference.` If the number is strong, it can also replace the `["15", "recruitment events led since 2023"]` stat in the ARSA `results` line.

**NCPS pieces (when they sign).** Upload the four files from `ncps-originals.zip`, then in `index.html` change `arsa-practice-recruitment-one-pagers-3.jpg` → `arsa-practice-recruitment-one-pagers-ncps-front.jpg` and `-4.jpg` → `arsa-practice-recruitment-one-pagers-ncps-back.jpg`. The program ad and pitch deck slide keep the same names, so uploading them replaces the current versions.

## Design notes (share these with Claude if you rebuild or redesign)

- **Palette:** navy `#16233B`, sand `#D8C9B0`, sage `#9CA487`, white. Name in the hero: "Olivia" and "Alonso" in sand, "R." in sage. ORA monogram: sand O and A, sage R.
- **Fonts:** Cormorant Garamond (italic serif headings) and Instrument Sans (body), both from Google Fonts.
- **Case studies:** ARSA, then Regionelle, then BCNJ. Each has intro, My role, Timeline, four stats (strongest result first, ordered by impact), then challenge, insight, approach, all in past tense. Spell out each brand with its acronym the first time it appears in the intro.
- **Captions:** topic + format, with the audience only when it's the point (e.g. "Resident recruitment email"). File names match the captions, with the brand first in case studies.
- **Thumbnails:** fill the frame, anchored top-left.
- **Case study galleries tell a story:** ARSA moves from recruitment to the partnership win to onboarding and internal work. BCNJ moves from website and awareness to patient materials to events.
- **More work (All tab):** digital and print alternate. Each format appears once before any repeats: digital runs ad/deck, email, social; print runs banner, brochure, card. Keep matching colors and brands from touching.
- **Digital and Print tabs** use their own order (see `filterOrder` in `index.html`).
- **Honesty rules:** label copywriting-only work "(copywriting)". Don't show work she didn't do. Keep NCPS's name and logo off the site until they sign. Don't call Regionelle "trademarked" unless that's confirmed. Keep the intranet's website name, workspace name, and email blurred.
- **Numbers that must match the resume:** 121 physicians in the network (up from 40 in 2023), 81 physicians and 8 practices joined since 2023, Summit grew from 130 to 320 attendees, 37 BCNJ launch events, 57 Regionelle event RSVPs in 2 days.
- **Mobile line breaks:** a case study `title` with ` | ` in it breaks onto two lines on phones only (desktop shows one line). Case study names break using `short`, and the hero tagline uses `<span class="mbr">`.

## Keep private

The `ncps-originals` folder that came in this zip (next to the `website` folder, not inside it) holds the NCPS versions of four pieces. Don't upload them to GitHub until NCPS signs; then follow the NCPS steps above.
