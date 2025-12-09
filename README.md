# Slidev Presentations

This repository stores reusable Slidev decks for demos and workshops. Each deck lives in `presentations/<deck-name>/slides.md` and can be run, built, or exported independently.

## Getting Started

```bash
pnpm install
```

Slidev bundles TypeScript and Vue support by default, so no extra tooling is required.

## Running a Deck

Pick one of the presentations (for example, `demo-intro`) and start the development server:

```bash
pnpm slidev presentations/demo-intro/slides.md
```

The server starts on `http://localhost:3030` with hot reloading and presenter view features.

## Creating a New Deck

1. Copy the starter deck:
   ```bash
   cp -r presentations/demo-intro presentations/my-new-deck
   ```
2. Update the frontmatter metadata in `slides.md` (title, description, theme).
3. Run it locally: `pnpm slidev presentations/my-new-deck/slides.md`.
4. Commit the new deck and push.

## Building & Exporting

- Static site build:
  ```bash
  pnpm slidev build presentations/demo-intro/slides.md
  ```
- PDF export (requires Playwright or Chrome):
  ```bash
  pnpm slidev export presentations/demo-intro/slides.md
  ```

## Repository Layout

```
presentations/
  demo-intro/
    slides.md       # Example deck with baseline styles
scripts/             # Helper scripts (if needed later)
```

Add more folders under `presentations/` as your demo catalog grows.
