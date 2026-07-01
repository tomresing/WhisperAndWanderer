# Whisper & the Wanderer

A tiny browser game in plain HTML, CSS, and JavaScript — no build tools, no
dependencies. Just open `index.html` in any modern browser and play.

## The idea

The **Wanderer** (the hero) is played by the *AI*. He explores a dreamlike world
on his own and makes his own instinctive decisions.

You are **Whisper**, a tiny fairy. You can't move the Wanderer directly. But at key
moments — a wall of thorns, a forking path, a sleeping guardian, a chasm, a
doubting mirror-self — Whisper flies out, time slows, and you can **nudge the
Wanderer to do things differently**.

If you stay quiet, the timer runs out and the Wanderer follows his own instinct.

## How to play

- Open `index.html` in a browser.
- Watch the Wanderer walk the dream on his own.
- When a prompt appears, click a suggestion (or press **1**, **2**, or **3**) to
  whisper your guidance.
- **Pause** / **Restart** with the buttons below the stage.

## Goal

Guide the Wanderer to the heart of the dream (600m deep) while keeping his **Spirit**
above zero and gathering as much **Wonder** as you can. His instinct is often the
reckless choice — your nudges can save his Spirit or earn more Wonder.

## Tech

Everything lives in a single self-contained `index.html`:

- HTML `<canvas>` for rendering.
- A small game loop driven by `requestAnimationFrame`.
- No external assets, libraries, or build steps.

## Play it online (GitHub Pages)

This repo ships a workflow (`.github/workflows/pages.yml`) that publishes the game
to GitHub Pages automatically.

1. Push to the `main` branch (or run the workflow manually from the **Actions** tab).
2. In **Settings → Pages**, set **Source** to **GitHub Actions**.
3. After the "Deploy to GitHub Pages" workflow finishes, the game is live at:

   `https://<your-username>.github.io/<your-repo>/`

Because `index.html` sits at the repo root, no build step is required — the
whole repository is served as-is.

