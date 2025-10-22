# LLM Pages — Ethics, Art, and Forecasts

A single-page, production-ready web application that publishes a curated set of artifacts: a short story, an ethical AV dilemma, a playful pelican-on-a-bicycle SVG, a Delhi restaurant recommendation, and a macro forecast for the U.S. Fed Funds rate in December 2025. Everything is static and GitHub Pages compatible.

## Features
- Self-contained index.html with professional, responsive UI using Bootstrap 5
- Links to all required artifacts: text, JSON, Markdown, SVG, license, and UID
- Inline validation for:
  - Story word count (300–400 words)
  - About.md contains exactly three words
  - LICENSE contains MIT License text
  - uid.txt matches the provided attachment (data URI)
- SVG rated by a lightweight mock LLM for composition and clarity
- Chart.js visualization of the Fed Funds rate forecast

## Setup / Deployment
- No build step required; simply open `index.html` in your browser.
- This project is designed for GitHub Pages. Once deployed, visit the Pages URL to view the app.

## Usage
- Navigate to the homepage. Use the link list to access each artifact directly.
- The dashboard panels show previews and validations for JSON/Markdown/Text files.
- The pelican SVG is rendered inline and scored by a mock LLM based on SVG structure.

## Technical Overview
- Libraries: Bootstrap 5 (UI), marked.js (Markdown rendering), Chart.js (charting)
- Structure: Single HTML file (`index.html`) with inline CSS and JS. All artifacts reside at the repository root.
- Error Handling: Defensive `fetch()` wrappers, status indicators for PASS/FAIL, and graceful fallbacks when a resource is unavailable.

## Files
- index.html — Main SPA with links and validations
- ashravan.txt — 300–400 word short story about Ashravan after restoration
- dilemma.json — Ethical decision cases for an autonomous vehicle
- about.md — Exactly three words
- pelican.svg — Pelican riding a bicycle (valid SVG)
- restaurant.json — Delhi restaurant recommendation
- prediction.json — Fed Funds rate forecast for Dec 2025
- LICENSE — MIT License
- uid.txt — Attached UID (data URI) uploaded as-is

## License
This project is released under the MIT License. See `LICENSE` for details.
