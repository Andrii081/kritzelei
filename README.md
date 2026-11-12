# Kritzelei v23 — Doodles / Каракули / Kritzelei

**Free handwriting notebook for iPad** — write with Apple Pencil or a simple stylus. Works offline, no account, no ads, 15 languages.

👉 **Open the app: https://andrii081.github.io/kritzelei/**

## Install on iPad
1. Open the link above in **Safari**.
2. Tap **Share** → **Add to Home Screen** → **Add**.
3. Start Kritzelei once from the new icon while you are online. After that it also works offline.

## New in v15
- Insert short **⅓ A4** notes sections between original PDF pages using the insertion controls or page overview.
- Notes sections grow by ⅓ A4 when writing reaches the penultimate grid/ruled line. Supports Apple Pencil and text; saved automatically.
- Built-in palette has 72 swatches, HSL sliders, HEX entry, and an optional native picker. Works on iPad without relying on Safari opening a hidden input.
- Inserts preserve page order in exports and backups.

## Update v16 — iPad stylus calculator fix
- The calculator now detects Apple Pencil contacts directly, including fast repeated taps on numbers, operators, cursor arrows and history.
- Prevents duplicate inputs from a synthetic click following a Pencil contact. Finger, mouse and keyboard input remain supported.
- Includes all v15 improvements: insert short grid sheets between PDF pages, auto-grow by 1/3 A4 and custom color palette.

## Update v17 — automatic handwriting and technical drawing (optional)
- Select **Pen** → tick **Auto: writing / drawing** to enable geometry recognition on pen lift. Recognizes clearly drawn long straight lines, arcs, circles, rectangles, triangles and certain polylines; small, ambiguous or letter-like strokes remain handwriting.
- Uncheck **Auto** to get exactly the v16 pen behavior (including the existing optional hold-to-straighten control).
- The switch persists on the same device. It is **off by default** to preserve current workflows and existing documents.
- Recognition is geometric, not AI handwriting OCR. Small or ambiguous shapes may need the dedicated Line / Shapes tools; use Undo if a mark is misclassified.
- All existing v15-v16 fixes are retained.

## What's new in v19
- **Single-stroke line correction:** one deliberate long pen stroke can become a straight editable line immediately upon lifting Pencil; no zigzag or holding necessary.
- **Scratch-to-erase:** with Smart Ink enabled, rapidly scrub back and forth over EXISTING handwriting several times in one uninterrupted gesture. The affected ink is erased without changing tools; Undo restores it. Ordinary crosses, triangles and gestures over blank paper are not deleted. The PDF page background is protected.
- **Localized title:** visible brand, browser tab, iPad app-title metadata and install manifests adapt to the chosen one of 15 languages. Note: an already-installed iPad Home Screen icon label is controlled by iPadOS and may need reinstallation to change; don't delete an app without first saving a backup.
- **New app icon:** paper with a lively ink flourish and a pen; same icon for all 15 languages.

## Features
- Notebooks with folders and search; paper: grid, lined, dots, graph paper, isometric, Cornell, blank
- **Endless page** that grows while you write — or classic A4 pages, your choice for every notebook
- **Document scanner**: finds the edges of the sheet automatically, straightens the perspective, removes the background and fits the page to A4 (colour, black & white or original)
- **Exact drawing**: line, arrow, dimension and shape ends stick to the grid lines and their corners (a mark shows it), lengths round to whole millimetres — switch off „Snap“ for any odd size
- **Dimensions as in technical drawing**: tap a line for its length with extension lines, drag from line to line for their true distance, angular dimensions between two lines; type a new value and the second line moves or turns
- **Updates itself**: a new version is fetched as soon as the app comes back to the screen; the version number is shown under „…“
- **Photo and scan buttons also take PDF and GoodNotes files** — their pages go in right after the page you are on
- **QR codes** on photos and scans are recognised automatically: open the link, copy it or insert it as text
- **Calculator** that stays open while you write (sin/cos/tan in degrees, roots, powers, history); tap any number or sign in the line to correct just that one
- **Opens GoodNotes files** (.goodnotes): pages and PDF worksheets are imported in the right order (handwriting from GoodNotes is not transferred yet)
- Fountain pen (pressure-sensitive), ballpoint, highlighter, eraser (whole strokes or parts)
- Ruler line with exact length (cm) and angle; protractor to measure existing angles
- Tap a line to change length, angle and colour; press and drag to move it; horizontal and vertical lines snap to the grid
- Perfect shapes: hold the pen at the end of a stroke to get a straight line, circle, rectangle or arc; shapes and dimension lines
- Lasso: move, scale, recolour, copy and delete
- Text boxes, photos, page overview with bookmarks
- Import PDF and write on it; export the notebook as PDF
- Backup and restore of all notebooks
- Languages: English, Deutsch, Русский, Українська, Polski, Türkçe, Español, Français, Italiano, Português, Nederlands, العربية, 中文, 日本語, 한국어

## Your data
Your notebooks are stored **only on your device** (in the browser storage of Safari). Nothing is uploaded anywhere.
Use **Save backup** from time to time, so you keep a copy if the device or browser data is lost.

## Price
Kritzelei is **free at least until the end of 2028**. Later versions may offer additional paid features.
Saving backups and exporting your notes as PDF will always stay free.

## License
Kritzelei is licensed under the **[PolyForm Noncommercial License 1.0.0](LICENSE.md)**:
free for personal and other non-commercial use. Commercial use needs written permission from the author — please contact me via GitHub.

Required Notice: Copyright 2026 Andrii Manoilo (https://github.com/Andrii081)

Included libraries (PDF.js, jsPDF) keep their own open-source licenses, see [THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md).

## Author
Idea, concept and development: **Andrii Manoilo**, built with the help of AI.


## v19: Experimental multilingual calligraphy

- The Pen toolbar has an optional **Beautiful handwriting / Calligraphy** checkbox (off by default). It is independent of Auto line/shape mode.
- After a pause of 1.45 seconds, a *multi-stroke* group is locally recognized with Tesseract.js (selected language determines the model). Only high-confidence readings (80%+) are automatically replaced by a handwritten-style text object. Undo immediately restores ink.
- To handle a single letter, Chinese character, Arabic glyph, or an uncertain reading, use **Lasso → Beautify selected handwriting** and review/edit the proposed text before replacing.
- The first use of a given language requires internet to download the Tesseract.js engine and that language model; later uses may work from the browser cache. Recognition occurs on the iPad; images of handwriting are not sent to an OCR server. The OCR libraries are requested from jsDelivr; language models come from the Tesseract language-data CDN.
- Supported recognition language codes: en, de, uk, ru, pl, tr, es, fr, it, pt, nl, ar, zh (Simplified), ja, ko. Recognition quality varies greatly by language/handwriting and is **not guaranteed**: Tesseract is primarily OCR for printed text, not professional Pencil handwriting recognition.
- Calligraphic display uses Caveat for Latin/Cyrillic, Aref Ruqaa Ink for Arabic, Ma Shan Zheng for Chinese, Yuji Syuku for Japanese, and Nanum Pen Script for Korean. Fonts are requested from Google Fonts on demand; fallback fonts apply if offline.
- The notebook and its PDF/export structure remain identical to v18. No changes are made to existing notes until the new feature is enabled.


## v20 — safer handwriting and individual letters

- Fixed the disappearing-letter problem: **scratch erase now has its own switch, OFF by default**, independent of geometry recognition. Scribble erasing requires at least seven deliberate quick alternating passes over existing ink; it cannot run when calligraphy mode is enabled. Note that if both features are enabled, handwriting protection takes priority.
- In Calligraphy mode the pen stays in handwriting mode, even if Auto geometry was enabled, to avoid silently converting parts of letters into technical shapes. A small, bounded smoothing filter removes jitter without changing stroke topology or deleting strokes.
- OCR now analyzes **spatially separate letter/character groups** using Tesseract single-character mode (PSM 10), not entire words. Each securely recognized character is positioned independently where it was written. Only very confident readings (93%+) change automatically. Uncertain characters remain as gently smoothed hand ink.
- Lasso → Beautify selected handwriting opens a per-character review. Characters are separated by spaces; use `□` to keep an individual handwritten glyph. Corrections are applied only to validated single characters. Undo restores every replaced stroke.
- **Limitations:** joined cursive letters or multiple connected characters cannot be segmented reliably without a specialized handwriting AI. For those, the app keeps original handwriting and merely smooths strokes. Tesseract.js is primarily printed-text OCR, so actual iPad handwriting recognition remains experimental and may rarely convert letters. The first OCR model download requires internet.
- Previous PDFs, colored ink, calculators, icon and language-specific names remain unchanged.

## Update v21 — restored automatic drawing + smooth handwriting
- Pencil geometry recognition and calligraphy can now be enabled together. Every deliberate straight stroke is recognized without a hold gesture; near-horizontal and near-vertical strokes are snapped onto the sheet's grid lines. Two or three common-origin long axes are labeled X/Y/Z and placed on the grid.
- Reworked deliberate scratch erase: multiple fast back-and-forth passes over pre-existing ink delete the touched strokes, with Undo, and can coexist with handwriting recognition. The separate scratch-erase switch remains available.
- Each newly written glyph is modestly smoothed immediately. Individual high-confidence OCR letters use the true handwritten Google Fonts **Bad Script** face (Latin/Cyrillic) rather than a generic print font. Other writing remains ink. Font and OCR language models download from the web when needed.
- External font use: Bad Script is distributed by Google Fonts under the SIL Open Font License 1.1, see https://github.com/google/fonts/tree/main/ofl/badscript ; no font binary is redistributed inside this package.
- Actual iPad/Apple Pencil recognition still needs device testing.

## v22 — numbers, pen weight, genuine crosses and cursive face

- The optional handwriting OCR accepts **single digits 0–9** as well as characters; low-confidence symbols get a restricted numeric pass. A standalone closed oval is inherently ambiguous among 0/O/О; it stays as ink instead of being incorrectly replaced by D. In an existing numeric sequence, an oval is treated as 0. The manual lasso review can correct ambiguous readings.
- Recognized calligraphy uses a connected handwriting typeface **Pacifico** for Latin and Cyrillic, and stores the original **inkW** to draw a colored outline preserving the chosen pen thickness. Other scripts use the existing writing fonts. The first font load needs an internet connection.
- The X/Y system now recognizes **two intersecting pen lines**, not only shared endpoints. It snaps the cross's origin to the actual grid and preserves negative and positive halves. Additional Z support remains available.
- Geometry metadata now survives closing and reopening the notebook.
- OCR is still Tesseract, which is **not a reliable handwriting-recognition engine**; ambiguous or low-confidence readings are deliberately left untouched. Never expect universal or perfect conversion.


## v23 — long arrowheaded axes, erasable calligraphy, improved numerals

- **Normal eraser now removes recognized calligraphy** (`t: "x"`) as a complete editable character, with both "Whole" and "Partial" eraser modes. The undo button restores erased characters. Imported image/PDF backgrounds remain protected.
- **Large, hand-drawn X/Y coordinate crosses** are found from the two dominant intersecting stroke shafts, including rough Pencil traces with small arrowheads at the ends. A minimum long-stroke length and a real crossing help avoid converting ordinary handwriting into axes. The result is redrawn with tidy arrowheads, X/Y labels and exact graph-paper alignment. Arrow-tool strokes can also be recognized. A subsequent diagonal from the common origin can become Z.
- **Digits 0–9** receive an additional digit-restricted OCR vote even when general OCR proposes a letter. Accepted digits use the handwritten **Caveat** display font rather than a regular printed numeral. Visible ink weight and selected pen color are retained. To avoid replacing O/О/D incorrectly, ambiguous standalone ovals remain handwriting unless numeric context exists.
- **Irregular ink** receives stronger bounded smoothing, keeping sharp corners, original strokes, color and pressure. Uncertain recognition never deletes the original glyph. For an ambiguous character, select it with Lasso → Beautify selected handwriting and correct the result before replacing.
- Supports the previous features for multi-page PDF notes, ⅓ A4 inserts, stylus calculator, color palette, natural handwriting and local backups.

**Important:** Tesseract OCR remains a printed-text OCR engine, not a high-accuracy handwriting model. It is unable to guarantee reading badly formed letters/digits. The recognizer and bundled tests verify processing rules but not every user's handwriting. Test on the actual iPad/Apple Pencil and keep backup copies. Initial use of the OCR engine and font resources requires internet.

## Update v24 — numbered X/Y coordinates and deliberate scratch erasing

- X/Y axes now show **numbered ticks for every grid cell**, initially 1, 2, 3, etc., with negative values on the other halves.
- **Hold a number for about half a second** to enter a positive step (e.g. 50); labels become 50, 100, 150... while every grid cell stays one tick. Both axes of the same cross update; the step persists in backups and PDF exports. Existing v23 coordinate crosses are upgraded on opening.
- All **automatic handwriting OCR / character substitution has been disabled and its controls removed**. Original handwriting is left as ink. Previously transformed calligraphy objects remain visible and erasable.
- The optional scribble-to-erase gesture requires a **single continuous stroke completed in at most one second** that intersects pre-existing ink at **four distinct points**. Only strokes with actual geometric intersections are erased, not nearby strokes within a broad area. One undo restores the erased objects. Independent drawing strokes cannot combine into an erasing gesture.
- Grid axes and handwritten strokes remain editable using the existing tools.
