# Notes for Claude Code

This repo is the website for Paddles to Progress, a student-run teen pickleball club (ages 13 to 19) that raises money for a local food pantry through tournaments.

## How the site is built

- One self-contained file: `index.html`. CSS is in a `<style>` block, the small script is at the end of `<body>`. No framework, no build step.
- Hosted as a static site (GitHub Pages from `main`, root folder).
- Font: Archivo from Google Fonts. Display text uses `font-stretch:125%` (expanded); body text is normal width.
- Colors (CSS variables in `:root`): court blue `--court`, deeper blue `--courtdeep`, surround green `--grass`, ball yellow `--ball` (#dff23d), ink `#0e1a2e`. Light and dark themes both use `light-dark()`.
- The hero court, ball, paddle and food box are inline SVG. The ball flies along the dashed arc once on load (SMIL `animateMotion`), and stays still if the visitor prefers reduced motion.

## Conventions

- Keep the court look: blue, green, white lines, yellow ball. Don't add new accent colors.
- Sentence case for headings and labels. No all-caps labels, no emoji.
- Check every change at 390px wide (phone) and 1280px (laptop), in light and dark mode. Nothing should scroll sideways.
- Keep buttons at least 44px tall with visible keyboard focus.

## Open items

See "Placeholders to replace" in README.md. The planning doc "Paddles To Progress" in Google Drive has the full website plan and open questions.

## Likely next steps

- Swap in the real logo and Instagram handle.
- Move tournament details into one data array (or `events.json`) so adding a tournament means editing data, not markup.
- Add a donation link once the team decides how donations are collected.
- Add a team section once founders and roles are set (get permission before posting names or photos of minors).
