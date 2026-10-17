# Publishing the Full Website Code to This Repo

The complete website source (2,493 files, ~284 MB — all pages, 354 blog posts, assets, tools) is too large for automated upload, so it needs one manual push. You already have the zip (`obaid-website-replica.zip`).

## Option A — GitHub Desktop (easiest)

1. Unzip `obaid-website-replica.zip` → you get a `site/` folder
2. Open GitHub Desktop → **File → Clone repository** → choose `obaidmughal14/obaid-mughal-cv`
3. Copy everything from `site/` into the cloned folder
4. GitHub Desktop will show ~2,493 new files → write a commit message like "Add full website source code" → **Commit** → **Push origin**

## Option B — Command line

```bash
# unzip the code
unzip obaid-website-replica.zip
cd obaid-mughal-cv                       # your local clone of this repo

# copy the site files in
cp -r /path/to/site/* .

# commit and push
git add .
git commit -m "Add full website source code"
git push origin main
```

## Notes

- No single file exceeds GitHub's 100 MB limit — the push will go through fine.
- The live site stays hosted at https://obaidasiaone-obaid-mughal-website.static.hf.space regardless.
- `Obaid-Mughal-Resume.pdf` at the site root is the CV served by the homepage's "My Resume" button.
