# Radioactive Duck — Deployment (v3, full catalog)

Site now carries the full 129-piece catalog (RD-001 through RD-129), 15 series.

## If the repo already exists
Replace everything with this folder's contents and commit.
(The images/ folder changed completely — old flat .jpg seal files are gone,
seals now live in images/seals/ and images/seals/thumbs/.)

## If starting fresh
See the earlier steps: public repo → upload these files to the root →
Settings → Pages → deploy from main branch, root folder.

## Domain (after Porkbun transfer completes)
Porkbun DNS records:
  A     (apex)  185.199.108.153 / .109. / .110. / .111.
  CNAME www     YOURUSERNAME.github.io
Then GitHub repo → Settings → Pages → Custom domain: radioactiveduck.com
→ wait for check → Enforce HTTPS.

## Adding a piece later
1. Photo → square crop → save two copies:
   images/seals/rd-NNN-name.jpg (1600px) and images/seals/thumbs/ (480px)
2. Copy any gallery-tile block in gallery.html, update number, name, filenames
3. Commit. Or send Claude the photo and it hands back the files.
