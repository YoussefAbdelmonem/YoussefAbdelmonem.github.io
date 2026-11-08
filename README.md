# Youssef Ramadan — Flutter portfolio

Static site for GitHub Pages (`https://youssefabdelmonem.github.io/`). No build step, no
cookies, no third-party requests (fonts are self-hosted in `fonts/`).

German is the default language; link to `?lang=en` for English applications.

## Add a showcase video

1. Put the MP4 in `videos/` (keep each file < 100 MB; ~10–20 MB is ideal) and a poster
   JPG (first frame or title card) in `posters/`.
2. In `index.html`, find the app in the `APPS` array and fill its `videos` array:

```js
videos: [
  { label: "Deutsch", src: "videos/rakeez-de.mp4", poster: "posters/rakeez-de.jpg", lang: "de" },
  { label: "English", src: "videos/rakeez-en.mp4", poster: "posters/rakeez-en.jpg", lang: "en" },
],
```

- `lang` makes that version play first when the page is in that language.
- Add `vertical: true` to a video (or the app) for 9:16 phone recordings.
- `featured: true` on an app shows it as the large card at the top.

Apps without videos show a "Showcase-Video folgt" placeholder automatically.

## Other files

- `assets/youssef.jpg` — profile photo
- `assets/Youssef_Ramadan_CV.pdf` — CV linked from the page (replace to update)
