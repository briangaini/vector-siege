# Vector Siege

A neon arcade survival shooter — pilot a hero rocket, dodge dragons, and climb through
progressively harder levels. Built with React (via CDN, no build step needed) and the
Canvas API, with fully synthesized sound and voice lines.

**[Play it live](#)** ← replace with your GitHub Pages URL once deployed (see below).

## Run it locally

No install required — it's a single self-contained `index.html`. Just open it in a
browser, or serve the folder:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy to GitHub Pages (free, public URL in ~2 minutes)

1. Create a new repo on GitHub (or use an existing one) and push these files:
   ```bash
   git init
   git add index.html README.md
   git commit -m "Add Vector Siege"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git push -u origin main
   ```
2. On GitHub, go to **Settings → Pages**.
3. Under **Source**, select **Deploy from a branch**, pick **main** and the **/ (root)**
   folder, then **Save**.
4. GitHub gives you a live URL, typically:
   `https://<your-username>.github.io/<repo-name>/`
   It can take a minute to go live the first time.
5. Share that link — it works for anyone, no login, on desktop or mobile.

## Notes

- High scores are saved locally in the visitor's own browser (`localStorage`), not shared
  between players.
- Sound effects and the "Monster incoming" / "Monster defeated" voice lines use the
  Web Audio API and the browser's built-in speech synthesis — no audio files needed.
- Everything (React, the icon library) loads from CDNs at runtime, so there's nothing to
  install or build — just the one HTML file.
