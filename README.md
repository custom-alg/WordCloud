# AI Camp Word Cloud

A single-file dashboard that turns AI Camp feedback into a word cloud. Each word is sized by how often it was mentioned and has its own color. Built for Škoda Auto × 42Prague.

## Features

- **Word cloud and stats**: total mentions, unique keywords, top keyword, median mentions. A table view is available too.
- **Easy data import**: paste rows from Google Sheets or Google Forms responses, or upload a CSV/TSV. Pick the word and count columns, then replace or add to the existing data.
- **Fully editable**: change words, counts and per-word colors. Edit the title and description in Settings.
- **Print export**: *Download for print* opens a preview of the exact image that will be saved.
  - PNG, 3000 × 2000 px, cloud only (no title or stats)
  - Light (default) or Dark. In Dark, colors are lightened to stay readable.
- **Save & sync**: "Save & sync for everyone" republishes the page with the current data, so every viewer sees the same version.
- **Light/dark UI** that follows the system setting.

## Usage

1. Open **Edit dashboard**.
2. **Import** tab: paste or upload your Sheet/Form data → map columns → *Replace all words*.
3. **Words** tab: fine-tune words, counts and colors.
4. **Save & sync for everyone**.
5. **Download for print**: check the preview, choose Light or Dark, then *Download PNG*.

## Notes

- Data lives inside the HTML file itself (no backend, no database).
- There is no live Google Sheets connection yet. Import is copy/paste or CSV.
- Fonts: Sora (cloud), Manrope (headings), IBM Plex Sans (UI), loaded from Google Fonts.
- Sample data is included and can be restored with *Reset to sample data* in Settings.

## Stack

Plain HTML, CSS and JavaScript, with no dependencies. The cloud layout is a spiral placement with collision detection, and the export is drawn on a `<canvas>`.