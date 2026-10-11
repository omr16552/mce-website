# Malvern College Egypt: homepage

The redesigned Malvern College Egypt homepage ("Refined Parent Journey", V2), built as a static site.

## Deploy on Vercel
1. In Vercel, choose **Add New → Project** and import `omr16552/mce-website`.
2. Framework preset: **Other**. Leave the build command and output directory empty.
3. Deploy. Every push to `main` redeploys automatically.

## What is here
- `index.html`: the page shell (fonts, styles, metadata).
- `app.js`: the page itself (layout, scroll animations, interactions, admissions form), bundled with Preact.
- `assets/`: photographs, films, logos and the crest.
- `vercel.json`: long-term caching for assets.

## Notes before launch
- The admissions form validates entries and shows a confirmation, but does not yet send data anywhere. Connect it to the admissions system.
- Apply Now, fees, transport, entry requirements, prospectus and privacy-policy links are placeholders (`#`).
- Yellow dashed "Editor note" boxes mark unconfirmed details. They are hidden on this public build; set `editorNotes` to `true` in `DEFAULTS` at the end of `app.js` to show them for review.
- Helvetica is used where installed (Arial elsewhere). Add the licensed Helvetica web fonts to load it on every device.
