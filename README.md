# Calendar Palette Creator

A single-file tool for building harmonious three- or four-colour palettes for calendar and product UI. Seed one colour and the engine derives the rest so that every pair of colours relates and none clash. Everything updates in real time against live previews.

## What it does

- Seeds a palette from any one role (Surface, Ink, or Accent) and derives the others.
- Eight generation modes: Auto, Monochromatic, Analogous, Complementary, Split Complementary, Triadic, Tetradic, and Square.
- Offers several scored candidate palettes per seed.
- Optional fourth colour (Soft) for weekends, event dots, selection states, and secondary text.
- Live previews across a calendar, a list card, a menu, and a mobile home screen.
- Accessibility: a reversible Aesthetic / Accessible toggle that nudges text and accent lightness to meet WCAG ratios without regenerating, plus an informational colour-vision-deficiency check (protanopia, deuteranopia, tritanopia).
- Per-colour editing in HSB or OKLCH, a full colour picker with a built-in swatch library, and direct hex entry.
- Adjust the whole palette by Hue, Saturation, Brightness, and Temperature.
- Locks: a padlock holds a colour through regeneration, and a lightness lock (L) holds a role's lightness while randomising so a set of palettes stays tonally consistent.
- History (undo and redo), saved palettes, and export to hex, CSS variables, CSS OKLCH, Tailwind, JSON tokens, or Figma variable names.

## How the harmony works

The Ink (text) colour sits analogous to the Surface, rotated only a little around the wheel but pushed hard in value so it reads. The Accent is placed in strong contrast to the Surface, which is enforced on every generation. The result is a palette where Surface and Ink share a family while the Accent provides the pop, and the whole set holds together because each pair is independently harmonious.

## Roles and their calendar meaning

- **Surface**: the background card.
- **Ink**: the dates, the year, and the weekday labels.
- **Accent**: the month name, the dividing lines, and the today ring.
- **Soft** (optional): weekends, event dots, selection, and secondary text.

## Getting started

This is a single self-contained `index.html`. There is no build step and no dependencies to install. Open the file directly in a browser, or host it.

To publish on GitHub Pages:

1. Create a repository and add this file as `index.html`.
2. Open the repository Settings, then Pages.
3. Set the source to your main branch and save. Your URL appears there shortly.

## Notes

- The only external resource is the Inter typeface, loaded from Google Fonts. If it is blocked, the app falls back to the system sans-serif.
- Saved palettes persist in the browser via `localStorage`, so they are local to each browser and device.
- Works in current versions of Chrome, Safari, Firefox, and Edge.

## License

Released under the Apaache License 2.0.
