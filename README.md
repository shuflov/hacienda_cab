# Hacienda Čab 🚵🍻

A single-page invite site for a farewell cycling party at Hacienda Čab — built as a static HTML page with a bilingual (SK/EN) toggle.

## What it is

A lightweight, no-build landing page for a private event:
- Event details (date, schedule, location)
- Embedded maps (via [mapy.com](https://mapy.com)) for the venue and the Saturday gravel route
- A day-by-day rundown (Friday arrival, Saturday ride, sleeping arrangements)
- One-click RSVP via WhatsApp

## Tech

- Plain **HTML + CSS + vanilla JS** — no build step, no dependencies, no framework
- Google Fonts (`Inter`) loaded via `@import`
- Bilingual content handled with `data-sk` / `data-en` attributes on each element, swapped in by a small `toggleLang()` script
- RSVP button links directly to a pre-filled [WhatsApp click-to-chat](https://faq.whatsapp.com/425247423114725) URL

## Running it locally

No build tools needed — just open the file in a browser:

```bash
open hacienda-cab.html
```

Or serve it locally if you prefer:

```bash
python3 -m http.server
```

## Known issues / TODO

- [ ] Language toggle doesn't initialize on page load (only fires on click) — fix pending
- [ ] Some `data-sk` values are out of sync with the visible fallback text in a few sections — fix pending
- [ ] Verify translation of a few idiomatic Slovak phrases in the English version

## Structure

```
.
└── hacienda-cab.html   # single-file site (HTML/CSS/JS all inline)
```

## License

Personal project — no license specified.
