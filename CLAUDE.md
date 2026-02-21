# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a personal website built with Astro, a modern web framework for content-driven websites. The project uses TypeScript and follows a simple, clean architecture focused on static site generation.

## Development Commands

| Command | Description |
|---------|-------------|
| `pnpm install` | Install dependencies |
| `pnpm dev` | Start development server at localhost:4321 |
| `pnpm build` | Build production site (includes type checking) |
| `pnpm preview` | Preview production build locally |
| `pnpm astro check` | Run Astro's type checker |

## Architecture

- **Framework**: Astro v4 with TypeScript
- **Structure**: Standard Astro project layout
  - `src/layouts/`: Reusable page layouts (Layout.astro is the main layout)
  - `src/pages/`: File-based routing (index.astro, about.astro)
  - `public/`: Static assets
- **Styling**: CSS-in-Astro with CSS custom properties for theming
- **TypeScript**: Strict configuration extending astro/tsconfigs/strict

## Key Files

- `src/layouts/Layout.astro`: Main layout component with global styles and meta tags
- `src/pages/index.astro`: Homepage with navigation structure
- `astro.config.mjs`: Minimal Astro configuration
- `package.json`: Contains all development scripts and dependencies

## Development Notes

- The build command includes type checking (`astro check && astro build`)
- Global styles are defined in Layout.astro using CSS custom properties
- The site uses a green accent color theme defined in CSS variables
- Pages use the Layout component for consistent structure and metadata