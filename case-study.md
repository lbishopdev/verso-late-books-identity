# Verso Late Books: case study

**Status:** self-initiated concept. The client, "Verso Late Books", the address, the staff name, the book title and the handles shown on the boards are all invented. There are no real clients, results, metrics or awards in this piece.

## The brief I set myself

Design a complete identity for a small shop with a point of view, then prove it holds across a mark, a colour system, type, a graphic language and real-world applications. I chose a late-night bookshop because it has a built-in contrast (night and day, dark and light page) that a visual system can actually be built from, instead of decorating a name.

## Concept

*Verso* is the left-hand page of an open book, the reverse of a leaf. A shop that opens at 6 pm and closes at 4 am lives on the other side of the day, so the name and the hours say the same thing.

The mark is one move: an open page split down the gutter. The left page is dark, the right is a light frame. A single disc, centred on the gutter, is read two ways:

- On the dark verso it is cut out, a moon that exists only because the page is dark.
- On the light recto it is filled with amber, a lamp, the only thing lit.

Because both readings share one circle and one centre line, the mark cannot be redrawn without keeping both halves. That constraint is what makes it feel designed rather than assembled.

## Key decisions

**Geometry over illustration.** The mark sits on a 100 x 120 unit grid: pages 50 + 50, frame 7, disc radius 30, gap 13. The disc's arc endpoints land exactly on the gutter, and the outer shape plus both disc halves are drawn as one compound path so no hairline seam can appear at the join. Clear space is x = the disc radius (a quarter of the mark's height).

**A small-size mark, not a shrunk one.** At 16 px the 7-unit frame collapses into a blurry grey line. I rasterised the mark at 1x and looked at the pixels, then built a small variant (frame 10, radius 32) that holds its structure down to 16 px. 16 px is the stated floor; below it the mark is not used.

**Wordmark with one detail.** "verso" is set in Sitka Display, lowercase, tightly tracked. The only intervention is the "o": its left half is the ink colour and its right half is lamp, so the type echoes the mark. In one-colour use both halves are the same ink and the word is still plain type. The "LATE BOOKS" descriptor is a fixed-tracking Bahnschrift line that is dropped below about 120 px wide.

**Mostly night, a little lamp.** Six named colours with ratios: Small Hours 40, Vellum 32, Reading Blue 12, Lamp 8, Dust Jacket 5, Foxing 3. The proportion bar on the colour board is drawn to those numbers. Contrast ratios on the board are computed from the hex values, not estimated, and the board lists which pairings are approved for body text and which are large-text or label only.

**Type with a job each.** Sitka (serif) carries voice: display, italic taglines, text. Bahnschrift (railway-style sans) carries information: hours, numerals, labels, wayfinding. They are system fonts, so the boards render without a network. The board names open-licence stand-ins (Source Serif 4, Barlow Semi Condensed) for production.

**One pattern, three expressions.** The graphic language is the same page-and-disc, tiled. Each tile is a two-page book with the disc drifting across the gutter (dusk to dawn). The phase strip is the same idea reduced to a divider or loader. The spine row is a lateral cousin: shelf spines in the palette with one always lit in amber.

## System rules

1. The disc is the only circle in the identity. Nothing else is round.
2. Lamp is the only light. One use per layout: a disc, a word, a numeral, a spine.
3. Lamp and Foxing never carry body text on Vellum. Lamp is never a large field except as the backdrop for the small mark (avatars, stamps).
4. Pages are always a dark half and a light half. Pattern tiles keep that split even when recoloured with Reading Blue.
5. Sentence case for serif; caps only in Bahnschrift. One italic line per layout.
6. Margins are 96 px on the 1920 x 1080 board grid; every board shares the same running header, page number and footer.

## Applications shown

A shopfront elevation (fascia, lit window, door card), business cards, a carrier bag, two bookmarks, an event ticket, three feed posts (page-split layout, quote card, pattern card), an avatar and highlight covers, a newsletter header and an app icon at six sizes plus a home-screen context. All are flat mockups drawn in HTML/SVG; there are no photographs and no stock assets.

## What I would extend

- A motion system: the disc stepping across the gutter as a loading and transition device.
- A shelf-talker and wayfinding kit using the spine lockup and Bahnschrift numerals.
- A one-page usage guide for non-designers: five do and don't pairs, a web token file and print specs.
- Packaging for tote bags and book wrap using the endpaper tile on Dust Jacket stock.
- A real print proof: the CMYK values on the colour board are naive conversions and would need a press proof.
- Accessibility pass on the app icon and social templates (alt text conventions, minimum text sizes).

## Process note

The boards are generated from code: a shared library builds the mark and lockups from the grid numbers, and each board is an HTML/SVG page rendered to a 1920 x 1080 PNG with headless Edge. I reviewed every board visually and iterated: the first pass had over-tracked descriptors, a hairline seam at the gutter, a clipped caption and a pattern whose light pages disappeared into the board background; those were fixed before this version.
