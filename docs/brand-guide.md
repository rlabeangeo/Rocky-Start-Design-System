# Rocky Start Exploration Services

Rocky Start Exploration Services is a field-geology and mineral-exploration services company. The brand should feel like a well-kept field book: weathered cream paper, typewritten records, neat notes in the margin, and colours you'd see on a long day out on an outcrop. It's rugged, warm and solid. It's never glossy.

This is a first draft, built from a short brief rather than existing brand files. The logo is a three-peak mountain range beside the name, with a one-colour survey seal and an "RS" mark for small sizes. See [logo guidelines](logo-guidelines.md).

## Voice and content

The motto is **"Geology starts, and ends, in the rocks."** Use it as the tagline under the name on covers, proposals and the website.

- **Plain and exact.** Write the way you'd log core: what was seen, where, how much. "Chalcopyrite-bearing garnet skarn, 112.0–128.4 m" beats "promising mineralisation".
- **Confident, not salesy.** State results and limits honestly. Avoid hype words like *world-class*, *game-changing* or *unlocking value*.
- **Numbers carry units, every time.** Write `1.82% Cu`, `128.4 m` and `Az 245°`, with a space between value and unit, set in `data`.
- **Sentence case** for headings ("Drill program summary"). Capitals only for `label` text.
- A little dry humour is fine in the name ("Rocky Start"), but keep it out of technical text.

## Colour

The palette comes from a hike: iron-stained rock, pine on the ridge, sandstone, cold water, lichen, all on field-book paper.

| Token | Role |
| --- | --- |
| `paper` / `paper-raised` | Grounds. Most of any page is paper. |
| `ink` / `ink-muted` | Text. Ink for content, muted for metadata. |
| `rust` | The brand colour: primary actions, links, key figures. It also marks errors. |
| `pine` | Secondary accent and success. |
| `ochre` | Highlights, warnings and chart fills. Text on ochre uses `ink-on-ochre`; never set ochre text on paper. |
| `slate` | Info states and water in figures. |
| `sage` | Quiet background tint for notes and selected rows. |
| `line` | Hairlines and table rules. |

Rules:
- Keep rust for the one thing on a page that matters most. If everything is rust, nothing is.
- For charts, use the order rust, ochre, slate, pine. Neighbouring series alternate dark and light, so they stay distinct for colour-blind readers. With more than two series, add direct labels too.
- Dark mode ("Headlamp") lifts each hue so it still passes contrast on the dark umber `paper`.

## Typography

There are three families, all free Google Fonts:

- **Alegreya SC** (`smallcaps`) for display titles, the logo name, the seal and RS mark, section headings and subheadings. It's a warm, bookish small-caps serif with the feel of an old survey report, but with crisp, even letters. Headings use weight 500; 700 is there for extra emphasis. Write headings in sentence case: capitals stay full height and the rest set as small caps.
- **Courier Prime** (`typewriter`) for body text, data and labels. It's a typewriter face redrawn for long reading, so reports read like a clean typed log.
- **Kalam** (`hand`) for field notes only: margin annotations and callouts on figures. Don't use it for paragraphs.

Styles: `display`, `heading` and `subheading` (small caps); `body`, `data` and `label` (typewriter); `note` (hand). A page uses one `display` at most.

## Layout and shape

- **Spacing** runs `space-2` 8, `space-4` 16, `space-6` 24 and `space-10` 40. The 24px step doubles as the field-book grid.
- **Corners** are near-square, and on drawn shapes they're slightly irregular rather than truly square. `radius-none` is the default, `radius-sm` (2px) is for controls and `radius-md` (6px) is for cards. Nothing goes rounder than that.
- **Rules over shadows.** Separate things with a `line` hairline or a change to `paper-raised`, not drop shadows.
- **Strata.** The brand's signature shape is stacked horizontal bands of unequal height, like sedimentary layers. Use it for headers, cover bands and section dividers. Draw each layer with a wide chisel marker against a straight edge (see Drawn by hand).

## Drawn by hand

Every illustration on the page should look like it was drawn lightly in the field book, in coloured pencil or alcohol marker. It shouldn't look generated. That covers bands, outlines, figures and icons. Text stays crisp, and so do printed things like dot grids and table rules.

- **Light, translucent colour.** Fill drawn shapes with marker passes at `opacity-marker` (0.62). Each pass is flat and even, with no texture inside it. The translucency keeps the colour from shouting, and where passes overlap, the colour builds up into a darker seam, just as real alcohol marker does.
- **Logo strata match.** The mountain mark uses the same flat strokes and tapering overlap seams, clipped to the near range. The one-colour seal echoes them with faint rust bands.
- **Pencil lines, not pen.** Outlines and traced contacts are thin (about 1px) at `opacity-pencil-line` (0.55). Logo outlines are the one exception: they're heavier, so the mark holds up at small sizes.
- **Strata are ruled with a wide marker.** Each layer is one to three broad chisel-tip strokes depending on its thickness (one up to 12px, two up to 26px, three above that). Each stroke is uniform. The variation lives in the overlaps and the ends:
  - **Overlaps:** each stroke overlaps its neighbour by 1–5px, and the overlap tapers along its length, as if the ruler shifted a hair between passes. So every darker seam is a slightly different width at either end. Layers overlap each other the same way, so their colours mix at the contacts.
  - **Edges:** the long edges are straight, as if drawn against a ruler.
  - **Ends:** slanted chisel starts with a small pool of ink where the nib touched down, and uneven lift-offs at different lengths.
- **Freehand lines drift slightly.** Lines drawn without a straight edge, such as outlines and figure sketches, wander from their true path by up to `rough-wobble` (1px), in long gentle waves.
- **Barely ragged edges.** Use `rough-displace` 1 at `rough-frequency` 0.04 so edges are slightly uneven, never torn. Traced lines run just past the corners they meet (`rough-overshoot`, about 4px). Marker passes end in soft, uneven tips.
- **Dot grids are printed, not drawn.** They're exact, identical dots on the 24px grid, like bought dot paper. They're clearly visible in their corner, at `opacity-dot-max` (0.6), and fade out toward the centre. On the cover, the dot paper runs across the whole page, beneath the strata, so the translucent marker shows the dots through it. The fade edge runs parallel to the title's stepped right edge (the line joining the end of "Rocky Start" to the end of "Exploration Services"), and the dots are gone about 12px before they reach the lettering.
- **Same hand every time.** Generate the variation from a fixed seed, so a figure looks identical every time it's rendered. It should never reshuffle on reload.
- **Keep it legible.** Don't roughen or fade text, chart values or the edges of buttons and inputs.

The cover shows all of this: ruled wide-marker strata in flat strokes with tapering overlap seams and varied ends, light pencil rules along the contacts, and printed dot paper running beneath the strata, fading out just before the title.

## Iconography and imagery

- There's no icon set yet. When you need one, draw or choose single-weight line icons in `ink` that look hand-drawn (see Drawn by hand). Keep them simple and technical: map pins, layers, drill, compass.
- For photography, use real field and core-shed photos in natural light, with no stock imagery. Maps and sections use the palette above. Annotate them in `note` type.
- **Logo:** the three-peak mountain mark beside "Rocky Start" in Alegreya SC, with "EXPLORATION SERVICES" beneath, is the primary lockup. Below 40px, or when you only have one ink, use the rust survey seal or the RS mark. The full rules are in [logo guidelines](logo-guidelines.md).
