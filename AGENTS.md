# Agent notes for huginn-privacy

- **Repo purpose:** single-file static privacy policy site (`index.html`) referenced by Huginn's Google OAuth consent screen. Not a web app, not a build project.
- **No build, no tests, no CI.** Changes are just HTML edits; there is nothing to run or lint. Don't scaffold a toolchain.
- **Styling convention:** all CSS lives inline in `<style>` inside `index.html`. Do not add `<link>` tags, external stylesheets, JS, fonts, or analytics &mdash; the file must stay self-contained.
- **Keep it semantic:** `<header>`, `<main>`, `<section>` with `aria-labelledby`, `<address>`, `<footer>`. Google's consent screen validator looks for recognizable privacy-policy sections (purpose, data collected, use, sharing, retention, contact).
- **Effective date:** when editing policy content, update the `<time datetime="...">` inside the `.effective` block at the top of `index.html`.
- **Owner contact:** Alex VanLaningham, ajvanlaningham@gmail.com &mdash; this is the authoritative contact string; update everywhere if it changes.
