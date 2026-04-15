# Brand Visual Style

Adaptig's visual identity is built around a felt-textured 3D illustration style, a six-color palette anchored on Paper Beige, the Proxima Nova type family, and five geometric shapes used as decorative elements and letter substitutions.

**All visual assets referenced below are checked into this repo under `brand-assets/`.** Clone the repo and the files are ready to use. Paths below are relative to the repo root.

For brand voice and messaging guidelines, see `brand-tone-of-voice.md`.

---

## Color Palette

Six brand colors from the canonical Design Guide:

| Name | Hex | RGB | CMYK | Role |
|------|-----|-----|------|------|
| Paper Beige | `#f9f5ea` | 249, 245, 234 | C1 M2 Y7 K0 | Primary background |
| Orange Peel | `#fa5929` | 250, 89, 41 | C0 M80 Y91 K0 | Energetic accents, CTAs |
| Aqua Blue | `#0a66db` | 10, 102, 219 | C84 M62 Y0 K0 | Professional accents |
| Leaf Green | `#30966b` | 48, 150, 107 | C80 M18 Y73 K3 | Growth, success accents |
| Charcoal Black | `#212124` | 33, 33, 36 | C73 M67 Y62 K72 | Primary text, logo |
| Sky Blue | `#abc9f5` | 171, 201, 245 | C30 M14 Y0 K0 | Secondary background, soft accents |

**Background rules:**
- Default background is **Paper Beige**.
- Charcoal Black and Sky Blue may also serve as background colors (e.g., section dividers, website hero sections).
- Logo, text, and shapes should mainly be displayed in color on Paper Beige.
- On dark backgrounds, use Beige or Light Blue shapes; on light backgrounds, use Black, Orange, Green, or Blue shapes.

**CSS custom properties:**
```css
:root {
  --adaptig-beige: #f9f5ea;
  --adaptig-orange: #fa5929;
  --adaptig-blue: #0a66db;
  --adaptig-green: #30966b;
  --adaptig-black: #212124;
  --adaptig-sky: #abc9f5;
}
```

---

## Logo

### Variants

| Variant | Path | Use When |
|---------|------|----------|
| Full wordmark, transparent BG | `brand-assets/Logo/PNGs/Adaptig-logo-full-transparentBG.png` | Default for documents, slides, websites |
| Full wordmark, white BG | `brand-assets/Logo/PNGs/Adaptig-logo-full-whiteBG.png` | When transparency is not supported |
| Logomark (A), no URL, transparent | `brand-assets/Logo/PNGs/Adaptig-logomark-noURL-transparentBG.png` | Favicons, avatars, small icons |
| Logomark (A), no URL, white BG | `brand-assets/Logo/PNGs/Adaptig-logomark-noURL-whiteBG.png` | Small icon on opaque background |
| Logomark (A), with URL, transparent | `brand-assets/Logo/PNGs/Adaptig-logomark-URL-transparentBG.png` | Marketing materials with URL |
| Logomark (A), with URL, white BG | `brand-assets/Logo/PNGs/Adaptig-logomark-URL-whiteBG.png` | Marketing on opaque background |
| Slogan image | `brand-assets/Logo/AI adoption that sticks.png` | Slogan as image asset |

### Logomark Meaning

The bold "A" logomark uses negative space to place the shape of an "i" into the letter "A", cleverly combining the "ai" letter shapes. The negative space represents both the "i" of artificial intelligence and the shape of a gender-neutral person -- reflecting Adaptig's human-centric approach.

### Usage Rules

- **Primary display:** Charcoal Black logo on Paper Beige background.
- **Inverted:** Paper Beige logo on Charcoal Black background (second option).
- **Clear space:** The x-height of the "A" is the minimum padding on all four sides.
- **Never:** use the logo in red, green, blue, or any non-approved color combination; add effects (shadows, glows, outlines); place on busy or non-approved colored backgrounds.

### Animation Files

Logo animations are stored locally but excluded from the git repo (too large). If needed, find them in `brand-assets/Logo/Animation/` on any machine that has the full local copy:

| Format | Files |
|--------|-------|
| MP4 | `Adaptig-full.mp4`, `Logomark-noURL.mp4`, `Logomark-URL.mp4` |
| GIF | `brand-assets/Logo/Animation/GIF/Adaptig-full-transparentBG.gif`, `Logomark-noURL-transparentBG.gif`, `Logomark-URL-transparentBG.gif` |
| MOV | `Adaptig-full.mov`, `Logomark-noURL.mov` |

Note: GIF files ARE included in the repo. MP4 and MOV files are gitignored.

---

## Typography

### Weight Assignments

| Weight | Use For |
|--------|---------|
| Proxima Nova Semibold | Headlines, titles |
| Proxima Nova Regular | Body text, paragraphs |
| Proxima Nova Regular Italic | Names, quotes, emphasis |

Proxima Nova is a modern, approachable sans serif with humanist elements -- relevant to Adaptig's people-first approach. Other variations from the Proxima Nova family (condensed, extra-condensed, heavier weights) may be used tastefully in specific situations.

**System fallback stack:** `'Proxima Nova', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif`

### Font Files

Production fonts (full glyph coverage):

| Weight | Path | Format |
|--------|------|--------|
| Regular | `brand-assets/Font/Proxima-Nova/Proxima Nova/proximanova_regular.ttf` | TTF |
| Bold | `brand-assets/Font/Proxima-Nova/Proxima Nova/proximanova_bold.otf` | OTF |
| Bold Italic | `brand-assets/Font/Proxima-Nova/Proxima Nova/proximanova_boldit.otf` | OTF |
| Extra Bold | `brand-assets/Font/Proxima-Nova/Proxima Nova/proximanova_extrabold.otf` | OTF |
| Light | `brand-assets/Font/Proxima-Nova/Proxima Nova/proximanova_light.otf` | OTF |
| Black | `brand-assets/Font/Proxima-Nova/Proxima Nova/proximanova_black.otf` | OTF |

Demo fonts (limited glyph coverage -- see warning below):

Path format: `brand-assets/Font/Proxima-Nova/Demo_Fonts/Fontspring-DEMO-proximanova-<weight>.otf`

Key demo weights: `semibold`, `semiboldit`, `regular`, `regularit`, `medium`, `mediumit`, `thin`, `thinit`. Condensed (`proximanovacond-*`) and extra-condensed (`proximanovaexcn-*`) variants also available.

**Glyph coverage warning:** The Fontspring demo OTFs only include A-Z, a-z, 0-9, and basic punctuation. Hyphens (`-`), ampersands (`&`), and middle dots (`·`) may render as missing-glyph boxes. If a string contains these characters, either (a) use a production font file and adjust the weight, or (b) rewrite the string to avoid the offending characters.

Font specimen and usage reference PDFs are in `brand-assets/Font/Proxima-Nova/References/`.

---

## Shapes

### Lookup Table

Five geometric shapes, each available in all six brand colors (30 PNGs total):

| Shape | Black | Green | Dark Blue | Orange | Beige | Light Blue |
|-------|-------|-------|-----------|--------|-------|------------|
| Half-dome | 01 | 06 | 07 | 08 | 15 | 26 |
| Triangle | 02 | 09 | 10 | 11 | 16 | 27 |
| Asterisk | 03 | 12 | 13 | 14 | 17 | 28 |
| Quatrefoil | 04 | 18 | 20 | 22 | 24 | 29 |
| Leaf | 05 | 19 | 21 | 23 | 25 | 30 |

**Path format:** `brand-assets/Shapes/PNGs/<Color>/Adaptig - Shapes-<NN>.png`

Note: The color folder names `Dark Blue` and `Light Blue` contain a space. In HTML `src` attributes, encode spaces as `%20`.

**Example:** Orange Asterisk = `brand-assets/Shapes/PNGs/Orange/Adaptig - Shapes-14.png`

### Shape Usage Rules

- Shapes can frame photographs, act as background design elements, or serve as decorative accents in presentations and social posts.
- Mainly use shapes on Paper Beige backgrounds.
- Adaptig brand colors may be used interchangeably for each shape.
- On dark backgrounds, use Beige or Light Blue shapes.
- The five main shapes also have split/flipped variations that can substitute for letters in headlines (see below).

### Shapes as Letter Substitution

Shapes and their altered variations (split, flipped) can replace a single letter in a headline to add visual interest:

| Letter | Shape(s) |
|--------|----------|
| A, a | Triangle, Half-dome (half) |
| C, c | Half-dome (half), Half-dome (half, mirrored) |
| D, d | Half-dome (right half) |
| E, e | Asterisk (half) |
| F, f | Half-dome (left half) |
| I, i | Leaf (half) |
| J, j | Leaf, Leaf (with dot) |
| L, l | Half-dome (left quarter) |
| N, n | Half-dome, Half-dome (mirrored) |
| O, o | Asterisk, Quatrefoil |
| R, r | Leaf (half) |
| U, u | Leaf (double), Half-dome (inverted) |
| V, v | Triangle (inverted) |
| W, w | Asterisk (double) |

**Rules:**
- **One shape per word maximum** (unless the word is hyphenated or unusually long).
- Align the top and bottom of the shape with the top and bottom of the letter it replaces.
- **Alternate brand colors** -- never use the same color for a shape and its surrounding text in the same word.
- The word must remain clearly legible. Short words may not work with this treatment.
- Choose a word that is important within the sentence to highlight its significance.

---

## Hand-Drawn Elements

Chalk-textured hand-drawn circles and underlines add a human-centric feel to taglines and key text.

**Rules:**
- Use sparingly to draw attention to key words -- do not overcrowd a sentence or text block.
- Circles and underlines always have a chalk-like texture.
- Always use the same color as the text they highlight.
- Consistent line width across all hand-drawn elements in a composition.
- Never use a different color from the surrounding text; never use plain/non-textured lines.

---

## Illustration Style

### Description

Adaptig's illustration style uses **felt-textured 3D characters** with soft lighting and warm materiality. Characters have a tactile, handcrafted quality with visible felt texture, rounded forms, and gentle shadows.

### Reference Images

Seventeen canonical reference images are in `brand-assets/Illustration Style/`. When generating or commissioning Adaptig brand illustrations, pass ALL of these files as style references so the output matches the house style.

```
brand-assets/Illustration Style/
  Illustration 1.png
  Illustration 2.png
  Illustration 3..png
  Illustration 4..png
  Illustration 5.png
  Gemini Generated Image (9).png
  Gemini Generated Image (10).png
  Gemini Generated Image (11).png
  Gemini Generated Image (12).png
  Gemini Generated Image (13).png
  Gemini_Generated_Image_14owba14owba14ow.png
  Gemini_Generated_Image_cwb558cwb558cwb5.png
  Gemini_Generated_Image_kr8pfjkr8pfjkr8p.png
  Gemini_Generated_Image_prwzbnprwzbnprwz.png
  Gemini_Generated_Image_prwzbnprwzbnprwz (1).png
  62024e4e277c46d3ff2630ea_corporate-illustrations-t.png
  online-marketing-business-illustration-with-modern-designs-in-flat-G0X612.jpg
```

### Image Generation Rule

**Use Nano Banana Pro (`gemini-3-pro-image-preview`) for all brand illustration generation. Never use Imagen 4.** Always pass the reference images from the directory above so the output matches the felt-textured house style.

---

## Photography Direction

- **Prefer illustrations over photography** across all Adaptig branding. The felt-textured 3D style is the primary visual language.
- When photography is included (e.g., "Who we are" sections, team pages), use **well-lit, high-resolution photographs**.
- Photographs may be cut out and framed by brand shapes, with a **dropshadow in one of the brand accent colors** (Orange, Blue, or Green).

---

## Templates and Applied Assets

### Call Backgrounds

| Audience | Path |
|----------|------|
| Trainers | `brand-assets/Call Backgrounds/CallBackground-Trainers.png` |
| Customers | `brand-assets/Call Backgrounds/CallBackground-Customers.png` |
| Marketing | `brand-assets/Call Backgrounds/CallBackground-Marketing.png` |

### LinkedIn Backgrounds

| Variant | Path |
|---------|------|
| Shapes | `brand-assets/LinkedIn Background/LinkedIn shapes .png` |
| Trainer 1 | `brand-assets/LinkedIn Background/LinkedIn Trainer 1.png` |
| Trainer 2 | `brand-assets/LinkedIn Background/Linkedin Trainer 2.png` |
| Trainer 3 | `brand-assets/LinkedIn Background/Linkedin Trainer 3.png` |

### Email Signatures

HTML email signature templates are in `brand-assets/Email Signatures/`:

- Footer preview (no social): `Email Footer - No social media.png`
- Footer preview (with social): `Email Footer - Social media.png`
- Per-person Roam/LinkedIn signatures: `brand-assets/Email Signatures/Linkedin and Roam Lobby Email footers/Signature <Name>.html`

---

## Archive Assets

The `archive/brand-assets/` directory (not in the git repo) contains larger or less frequently needed assets:

- **Design Guide PDF:** `archive/brand-assets/Design Guidelines/Adaptig - Design Guide.pdf` -- the canonical 10-page visual design guide with all rules in visual form.
- **Presentation templates:** 8 PowerPoint/Keynote templates in `archive/brand-assets/Presentation Template/`.
- **Intro videos:** v10 final + v9 in 6 languages (EN, DE, ES, ZH, JA, PT-BR) in `archive/brand-assets/Video/`.
- **Workshop images:** Event and training photos in `archive/brand-assets/Workshop Images/` (HK Events, LA Workshops).
- **Personal assets:** Sam's headshot and portfolio image in `archive/brand-assets/Personal/`.

These files are available on any machine with the full local copy or on the Adaptig shared Google Drive under `Brand Assets/`.

---

## Source Files

Adobe Illustrator source files (excluded from git, available locally):

| Asset | Path |
|-------|------|
| Logo master | `brand-assets/Logo/Live file/Adaptig-logo.ai` |
| Shapes master | `brand-assets/Shapes/Live File/Adaptig - Shapes.ai` |
