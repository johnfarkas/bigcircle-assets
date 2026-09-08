# Big Circle Auctions — Brand Assets

The asset library for **Big Circle Auctions**, a round-based auction platform for
higher-value assets. A wholly owned subsidiary of CoSpark, and a daughter brand of the
[CoSpark design system](https://cospark.farkas.design/).

## What is here

| Page | Contents |
| --- | --- |
| `index.html` | Hub, and the mark in brief |
| `logo/` | Horizontal and stacked lockups, and the icon — SVG + PNG, full color, reversed on dark, all ink, all white |
| `color/` | Four tiers, hex values, roles, and the contrast rules |
| `typography/` | Familjen Grotesk and IBM Plex Sans — downloads, embed code, type scale |
| `buttons/` | Four button types, three sizes, every state, with CSS |

Raw files live in `assets/logo/`.

## The mark

Six members, each with its own color and its own angle onto the same center, held inside
one unbroken circle. Every member is the size of every other, and the circle closes when
all six are present. The space they leave between them resolves into a fan turning the
same way they do.

Drawn on a 100-unit square. Every edge is a circle or a piece of one.

| Value | Role |
| --- | --- |
| `45.5` | Ring radius, at stroke weight `7` — giving an inner edge at `42` |
| `38` | Member envelope, four units clear of the ring |
| `27` · `11` | Head distance from center, and head radius |
| `7.2` | Tail radius at the hub |
| `60°` | Rotational symmetry, six times over |

The members turn **clockwise**, in the direction of rounds advancing toward Best & Final.
The mark is never rotated, mirrored, or recolored. The four-unit clearance between the
members and the ring is what holds it together small.

Scale floors: full color holds to **32 px**; single ink to **24 px**.

Clear space: a quarter of the mark's height on all four sides.

## Palette

Four tiers. The six colors of the mark keep their meaning only while they stay attached
to the idea of membership.

| Tier | Name | Hex | Role |
| --- | --- | --- | --- |
| 1 | Ink | `#11202A` | Text, the ring, dark grounds |
| 1 | White | `#FFFFFF` | The default ground |
| 2 | Patina | `#008C76` | Signature accent — fills and large areas |
| 2 | Patina Deep | `#00705E` | Links, buttons, accent text on white |
| 3 | Cinnabar | `#C24138` | Member 1 · error and destructive states |
| 3 | Copper | `#D4792F` | Member 2 · AUCTIONS in the lockup · shared with CoSpark |
| 3 | Brass | `#E0A32B` | Member 3 · warning states |
| 3 | Patina | `#008C76` | Member 4 |
| 3 | Oxide | `#1F6C8C` | Member 5 · informational states |
| 3 | Mulberry | `#8A3A52` | Member 6 |
| 4 | Slate 700–100 | `#43505C` → `#EDF2F7` | Text, rules, grounds |

Member order is fixed, clockwise from the top. Copper stays inside the mark, where it
carries the family resemblance to CoSpark; Patina does the interface work, which keeps
the two brands from looking alike in use.

## The wordmark

Archivo ExtraBold 800, caps, tracked to **−0.022em**. That value is fixed: the horizontal
lockup measures 376.5 × 100 units, and in the stacked lockup the wordmark is set at
17.356 so its width matches the mark exactly at 100 units.

AUCTIONS is offset 2.9 units right of the wordmark anchor so its **A** aligns optically
with the flat stem of the **B** — sidebearings scale with font size, so sharing an anchor
would leave the smaller line overhanging. In HTML that offset is `margin-left: 0.206em`
on the descriptor.

## Typefaces

**Familjen Grotesk** 600/700 for display and large figures.
**IBM Plex Sans** 400/500/600 for every working word.
Both SIL OFL.

The wordmark is drawn artwork, not a font setting. Use the lockup files.

## Notes on the files

The one-color lockups are genuinely single-color, descriptor included. The lockup SVGs
carry the wordmark as live text in Archivo — install the font or use the PNG. Every text
element sets `textLength` to its true measured width, so a fallback font normalizes to
the same box rather than reflowing. Outlined SVG and vector EPS for print vendors are in
production.

PNGs are transparent: the horizontal lockups are 2000 px wide, the stacked lockups
1400 px, and the icons 1024 px square.

## Local preview

```
python3 -m http.server 8000
```

Then open <http://localhost:8000/>.

## Publishing

Files sit at the repository root, so GitHub Pages serves them with no build step:
Settings → Pages → Source: *Deploy from a branch* → `main` / `/ (root)`.
