# Algo Showdown — Vincere client landing page

A static, single-page site that wraps the **Algo Showdown** trivia game in a glass-style,
Vincere-branded landing page. No build tools, no server. Publish free on GitHub Pages.

## Files
- `index.html` — the landing page (glass hero, "how it works", embedded game, compliant footer). The Vincere crest is embedded directly, so this file is self-contained.
- `algo-showdown.html` — the game itself. The landing page loads this in a frame and links to it for full screen.
- `README.md` — this file.

## Reskin in ~2 minutes
Open `index.html` and edit the values in `:root` at the top of the `<style>` block
(background, gold, blue, text, glass opacity). Everything else inherits from those tokens.

## Swap the game later
Replace `algo-showdown.html` with an updated game (keep the filename) and the page picks it up
automatically. To change the embed height, edit `.game-frame iframe { height: ... }` in `index.html`.

## A note on previewing locally
If you just double-click `index.html`, some browsers block the embedded game frame for local
files. The **Open full screen** link still works. Once the site is on GitHub Pages (served over
https), the embedded game loads normally — so the real test is the published URL below.

---

## Publish free with GitHub Pages

### 1. Create your GitHub account (one time, ~1 min)
- Go to https://github.com/signup
- Use your Gmail, pick a username and password, verify the emailed code.

### 2. Create the repository
- Click **+** (top right) -> **New repository**.
- Name it e.g. `algo-showdown`. Set it **Public** (Pages is free on public repos).
- Click **Create repository**.

### 3. Upload the files
- On the repo page, click **uploading an existing file**.
- Drag in `index.html`, `algo-showdown.html`, and `README.md`.
- Click **Commit changes**.

### 4. Turn on Pages
- **Settings** -> **Pages** (left sidebar).
- Source: **Deploy from a branch**, branch **main**, folder **/ (root)**. **Save**.
- After a minute your site is live at:
  `https://YOUR-USERNAME.github.io/algo-showdown/`

Share that URL with clients. Re-upload changed files anytime to update the site.

---

## Compliance note
The footer keeps Vincere's standard education-only / risk / "software licensor, not a
broker-dealer or fund manager" disclaimers, and the page intentionally contains no performance
figures or guarantees. Keep it that way if you edit the copy.
