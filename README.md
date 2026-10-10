# Qiutong Wang — Academic homepage

A simple static academic website: black top navigation, white background, serif text, and dark red headings and links. The About homepage has a photo area on the left and a biography on the right; phones show them vertically. No build step, external fonts, or JavaScript is required.

## Preview locally

From this folder, run:

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Open http://127.0.0.1:8000 in a browser. Stop the server with Ctrl+C.

## Update content

- `index.html`: About homepage, biography, email, CV link, and photo area.
- `research.html`: publications and talks with DOI, arXiv, slides, and notes links.
- `links.html`: useful links, accessible from the top navigation.
- `style.css`: shared typography, colors, navigation, and mobile layout.
- `assets/CV.pdf`: downloadable CV, including the complete education and teaching history.
- `assets/portrait.jpg`: the original seaside portrait used on the About homepage.
- `assets/tianyuan-2025-slides.pdf`: slides for the August 11, 2025 talk at Tianyuan Mathematics Research Center.
- `assets/yale-gss-2026-notes.pdf`: notes for the October 9, 2026 talk at the Yale Graduate Student Seminar.

The About homepage displays `assets/portrait.jpg` in a vertical 4:5 frame. The original 1920 × 1440 image is preserved; CSS controls the displayed crop and enlarges the person slightly. The current crop corresponds to the original image region at x=730, y=300, width=880, height=1100. Adjust `.portrait` width, left, and top in `style.css` to change the framing. The frame is 320 × 400 on larger desktops and up to 280 × 350 on phones.

The content is based on the supplied CV and talk materials. The DOI and arXiv links were verified in the initial version. Keep the navigation links consistent in all three HTML files when changing them.

## GitHub Pages

Commit and push to the repository, then choose **Settings → Pages → Deploy from a branch → main → /(root)**. `.nojekyll` makes the site publish as static files.
