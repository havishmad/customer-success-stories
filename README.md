# HMC Customer Stories

Showcase page for Havish M Consulting's 42 client case studies. Each one is available as an interactive HTML case study, a PDF and a short video.

## Structure
- `index.html`: the showcase page (search, function filters, company filter, thumbnail/list view, in-page viewer)
- `html/`: interactive case studies
- `pdf/`: PDF versions
- `video/`: MP4 videos
- `thumbs/`: card thumbnails
- `stories.csv`: index of all stories with their original file names

## Publish on GitHub Pages
1. Create a new public repository and upload everything in this folder, keeping the folders as they are.
2. Go to Settings → Pages → Build and deployment → Source: "Deploy from a branch", Branch: `main`, folder `/ (root)` → Save.
3. After a minute or two the page is live at `https://<your-username>.github.io/<repo-name>/`.

The GitHub website takes at most 100 files per upload, so upload one folder at a time, or use GitHub Desktop to push everything at once.

## Embed on Wix
Add → Embed Code → Embed a Site → paste the GitHub Pages URL. Stretch the block to full width and give it a tall height (about 1600–2000 px on desktop).

Or use Add → Embed Code → Embed HTML and paste:

```html
<iframe src="https://<your-username>.github.io/<repo-name>/" style="width:100%;height:1800px;border:0" loading="lazy" allow="fullscreen; autoplay"></iframe>
```

## Deep links
Any story can be linked directly, e.g. `index.html#amber-manufacturing-gantry-3d-model/video` (format: `html`, `pdf` or `video`).

## Adding a new story
1. Add `html/<slug>.html`, `pdf/<slug>.pdf`, `video/<slug>.mp4` and `thumbs/<slug>.jpg` (640×400).
2. Add an entry to the `STORIES` array at the top of the script in `index.html` (company, org, function, title, desc, slug, base). If the function is new, add it to one of the `FAMILIES`.
