# Caligari Title Cards

A browser tool for making title cards in the style of *The Cabinet of Dr. Caligari* (1920): jagged, cut-paper
lettering over spiky shapes, in the film's tinted colours. Type a title, adjust a few settings, and download
the card as a PNG.

## How it works

The film's title cards were cut by hand, so no two letters match and nothing sits quite straight. To capture
that, the page doesn't type with a font. It draws every letter itself, from an original set of letterforms
called Holstenwall (after the film's fictional town). Each letter is stored as a few straight-edged paper
shapes, and every copy on the card is cut again with its own variation.

The letterforms were drawn from scratch as polygons, following rules taken from the film's cards: stems are
wedges that taper to a point, bowls are pennants, counters are slivers rather than circles, and arms rise to
the right. No existing font's outlines were traced or reused.

Each card is painted in layers: background shapes, film grain, the glowing letters, and uneven light like a
projector's.

## Settings

| Setting | What it does |
| --- | --- |
| Line alignment | Left, centred or staggered |
| Shrink grammar words | Sets words like *the*, *of* and *und* smaller, in twelve European languages |
| Line scaling | Grows shorter lines toward the width of the longest |
| Max size | Caps how large the text can be |
| Angle | Tilts the text, bending the lines into a wave as it steepens |
| Jumble | Moves lines, words and letters off their places |
| Distortion | Varies each letter's shape |
| Card color | Green, blue, yellow or red, after the film's tinted prints |
| Card background | Four compositions of shapes from the film's cards; press again for a new one |

**Download PNG** saves the card at 1920 × 1440 pixels. The page's **How it works** button explains the
settings and tells the story of the project in more detail.

## Built with Claude

This project was designed and directed by Brett Rowley and built by [Claude](https://claude.ai), Anthropic's
AI model, using Claude Code. Claude studied the film's title cards, drew the letterforms, and wrote the page.

## Running it

The tool is a single HTML file, [`docs/index.html`](docs/index.html), with no build step, no dependencies and no
outside requests. Open it in a browser, or serve the `docs` folder from any static host.

## Credits

- The film stills in the page's story are title cards from *The Cabinet of Dr. Caligari* (1920), which is in
  the public domain. The image is via [Art of the Title](https://www.artofthetitle.com/title/the-cabinet-of-dr-caligari/).
- The panel text is set in [Jost](https://github.com/indestructible-type/Jost) by Owen Earl, embedded in the
  page under the SIL Open Font License 1.1. See [`LICENSE-Jost.txt`](LICENSE-Jost.txt).
