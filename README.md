# 📄 PDF Merger — Free & Private

A zero-backend PDF merger that runs 100% in the browser. No uploads. No server. No subscriptions.

## ✨ Features

- **Drag & drop** multiple PDFs onto the page
- **Reorder files** by dragging cards up/down
- **Select page ranges** per file (e.g. `1-3, 5, 7-9`)
- Quick buttons: All pages, First page, Last page, First half, Second half
- Live page count preview
- **Merge & download** in seconds
- Works offline after first load

## 🚀 Deploy to GitHub Pages (5 minutes)

### Option A — New repo from scratch

1. Create a new repo on GitHub (e.g. `pdf-merger`)
2. Upload `index.html` to the root of the repo
3. Go to **Settings → Pages**
4. Under *Source*, select **Deploy from a branch → main → / (root)**
5. Hit **Save** — your app is live at `https://yourusername.github.io/pdf-merger`

### Option B — Clone & push

```bash
git clone https://github.com/yourusername/pdf-merger
cd pdf-merger
cp /path/to/index.html .
git add index.html
git commit -m "Add PDF merger app"
git push origin main
```

Then enable GitHub Pages in Settings as above.

## 🔒 Privacy

- Files are **never uploaded** to any server
- All processing happens in your browser via [pdf-lib](https://pdf-lib.js.org)
- The only external requests are loading fonts (Google Fonts) and libraries (cdnjs) — all read-only

## 🛠 Tech Stack

| Library | Purpose |
|---|---|
| [pdf-lib](https://pdf-lib.js.org) | PDF parsing, page extraction, and merging |
| [SortableJS](https://sortablejs.github.io/Sortable/) | Drag-to-reorder file list |
| Google Fonts (Unbounded + IBM Plex) | Typography |

## 📝 Page Range Syntax

| Input | Meaning |
|---|---|
| *(blank)* | All pages |
| `3` | Page 3 only |
| `1-5` | Pages 1 through 5 |
| `1-3, 7, 9-11` | Pages 1–3, then 7, then 9–11 |

## License

MIT — free to use, fork, and modify.
