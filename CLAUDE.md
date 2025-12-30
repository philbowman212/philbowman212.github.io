# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Personal data portfolio website for Philip Bowman, hosted on GitHub Pages. Built on the HTML5 UP "Dimension" template - a single-page application using modal-style article switching.

## Development Workflow

**No build tools** - This is a static site with no npm, Makefile, or compilation steps.

**Deployment**: Push to `master` branch → GitHub Pages auto-deploys to `philbowman212.github.io`

**Testing**: Open `index.html` directly in a browser for local preview.

## Technology Stack

- HTML5, SCSS/CSS, JavaScript (jQuery)
- Font Awesome for icons
- Google Fonts (Source Sans Pro)

## Architecture

**Single-page modal pattern**: Navigation links toggle visibility of article sections (intro, projects, about, contact) rather than loading new pages. The JavaScript in `assets/js/main.js` handles article switching, responsive breakpoints, and animations.

**SCSS organization** (`assets/sass/`):
- `base/` - Reset, typography, page fundamentals
- `layout/` - Header, footer, wrapper, background, main content
- `components/` - Reusable UI: buttons, forms, tables, icons, lists
- `libs/` - Variables, mixins, functions, breakpoints

The SCSS is pre-compiled to `assets/css/main.css`. For styling changes, either:
1. Edit the SCSS and compile (requires sass CLI), or
2. Edit `main.css` directly for quick fixes

## Content Editing

All content is in `index.html`. Portfolio sections are `<article>` elements with IDs: `intro`, `projects`, `about`, `contact`. Project links point to external GitHub repositories.
