# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static HTML portfolio website ("CV Cómic") for Carlos Santos, a Full Stack Developer. The project uses a single HTML file with embedded CSS and JavaScript to create a comic book-themed resume/CV.

## Architecture

- **Single-file application**: `hv.html` contains all HTML, CSS (inline `<style>`), and JavaScript (inline `<script>`)
- **No build process**: Open the HTML file directly in a browser to view
- **Video assets**: The `videos/` directory contains MP4 files that can be embedded in the portfolio
- **No dependencies**: Pure HTML/CSS/JavaScript with no external libraries or frameworks

## Key Features

1. **Comic-style design**: Custom CSS creates a comic book aesthetic with speech bubbles, panels, and retro styling
2. **Video loading system**: JavaScript function `loadVideo()` allows users to dynamically load videos from YouTube, Vimeo, or direct MP4 URLs
3. **Responsive grid layouts**: Uses CSS Grid for skills badges and video cards
4. **Print-friendly**: Includes `@media print` styles for PDF generation

## Development

**To view the site:**
```bash
# Open directly in browser (Windows)
start hv.html

# Or use a simple HTTP server if needed
python -m http.server 8000
```

**To modify:**
- Edit `hv.html` directly - all code is in one file
- CSS starts at line 7 (inside `<style>` tag)
- HTML structure starts at line 387
- JavaScript starts at line 522 (inside `<script>` tag)

## Code Organization in hv.html

- Lines 7-385: CSS styling (comic theme, animations, responsive design)
- Lines 387-520: HTML content (header, panels, timeline, projects, contact)
- Lines 522-574: JavaScript (video loading functionality)

## Notes

- Contact information in the HTML (lines 514-518) uses placeholder values
- Video cards (lines 474-501) are designed to load external videos dynamically
- The design is optimized for modern browsers with CSS Grid and Flexbox support
