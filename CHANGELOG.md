# Changelog

## 2026-09-29 — Site redesign

Redesigned `index.html` and `stylesheets/styles.css`, inspired by
[vincentheddesheimer.github.io](https://vincentheddesheimer.github.io/) and
[saschariaz.com](https://saschariaz.com/). Developed and reviewed at
`/preview/redesign.html` before being promoted to the homepage.

The pre-redesign version is preserved on the `archive/pre-redesign` branch
(not published — GitHub Pages only serves `master`), so it can be restored
or referenced later:

```bash
git checkout archive/pre-redesign -- index.html stylesheets/styles.css
```

### Changes

- Profile photo: fixed squashed dimensions, added rounded corners, sized up
  (180px → 250px), and boxed the bio text/contact links to the photo's width
- Contact links: monochrome inline-SVG icons (location, email, LinkedIn,
  Bluesky) replacing emoji, colored links replacing plain text/`[in]`
- Horizontal rule under every section heading
- Wider, justified content column with more generous spacing
- New numbered **Publications** section (CV-style, numbered high-to-low via
  `<ol reversed>`), sitting above Working Papers
- Collapsible `[Abstract]` on every paper, using native `<details>` — no
  JavaScript, so adding a new paper or abstract is a plain `index.html` edit
- Publication titles without a confirmed URL yet render in the same link
  color via a `.pending-link` span with a native tooltip ("Link will follow
  soon."), instead of a dead `href="#"` link
- Co-author names as plain text instead of linked
- Dropped the "Hello" heading and remaining in-text emoji
- Font: Lato → Inter
