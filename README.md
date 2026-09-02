# Wedding Invitation

An animated, single-page wedding invitation. Opens as a sealed envelope —
click the wax seal to open the flap and reveal the invitation card
(floral line-art frame, ceremony/reception schedule, venue, RSVP, and a
closing quote), with a few petals drifting ambiently in the background.

## Files

- `index.html` — the entire invitation (HTML + CSS + JS, no build step, no dependencies).

## Preview it

Just open `index.html` in a browser, or from this folder run:

```
start index.html
```

## Customize

Everything is currently **placeholder content** (names, date, venue, RSVP
email/phone, quote). Open `index.html` and search for these sections to
replace them:

- `<h1 class="card__names">` — the couple's names
- `<p class="card__date">` — wedding date
- `.schedule` block — ceremony / reception times
- `.venue` block — venue name & address
- `.rsvp__link` — RSVP email (the `mailto:` href) and `.rsvp__phone` — phone number
- `.quote` — the closing quote / message
- `--rose`, `--sage`, `--gold` CSS variables near the top of `<style>` — color palette

## Design notes

- Single committed color theme (warm ivory paper, dusty rose, sage,
  antique gold) — intentionally not theme-switching, like a printed
  keepsake card.
- Respects `prefers-reduced-motion` (shortens/removes animation for
  users who request it).
- No external assets besides Google Fonts (Parisienne, Cormorant Garamond, Jost).
