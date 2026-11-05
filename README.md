# huginn-privacy

Static privacy policy site for **Huginn**, a self-hosted single-user personal
automation application. The published page at `index.html` is the privacy policy
URL supplied to Google's OAuth consent screen (and any other third-party API
providers that require one).

The repo intentionally ships a single file:

- `index.html` &mdash; semantic HTML5 privacy policy. Inline CSS only, no
  external dependencies, no JavaScript, no analytics, responsive across mobile,
  tablet, and desktop viewports.

## Why this exists

Google's OAuth verification process requires applicants to host a public
privacy policy that describes how user data is handled. Even a single-user
homelab deployment must point its consent screen at a reachable URL. This repo
is that URL's source of truth.

## Editing

Open `index.html`, edit the content, update the effective date at the top of
the `<header>`, and commit. There is no build step.

## Contact

Andrew Van Laningham &mdash; ajvanlaningham@gmail.com
