# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with this repository.

## Project Overview

This is a personal portfolio website for Tomas Barrera (akires47.com). It's a single-page site showcasing professional background, skills, and contact information.

## Tech Stack

- **Framework**: Astro 5.x
- **Styling**: Tailwind CSS 3.x
- **Language**: TypeScript
- **Package Manager**: pnpm

## Project Structure

```
src/
├── components/
│   ├── Hero.astro      # Hero section with name, title, avatar, companies
│   ├── About.astro     # About section with bio and experience
│   ├── Skills.astro    # Skills grid display
│   ├── Contact.astro   # Contact section with email and social links
│   └── Footer.astro    # Site footer
├── layouts/
│   └── Layout.astro    # Base HTML layout with meta tags
└── pages/
    └── index.astro     # Main page composing all components
public/
└── favicon.svg         # Site favicon
```

## Common Commands

```bash
# Install dependencies
pnpm install

# Start development server
pnpm dev

# Build for production
pnpm build

# Preview production build
pnpm preview
```

## Architecture Notes

- **Component Props**: All components use TypeScript interfaces for props
- **Data Flow**: Skills, companies, and social links are defined in `index.astro` and passed to components
- **Styling**: Uses Tailwind utility classes with a dark theme (zinc color palette)
- **Typography**: Uses Inter font loaded from Google Fonts
- **Responsive**: Mobile-first design with md: breakpoint adjustments

## Design System

- **Primary Gradient**: violet-400 to cyan-400
- **Background**: zinc-950 (main), zinc-900 (cards)
- **Border**: zinc-800 (default), violet-500/50 (hover)
- **Accent Colors**: violet-400 (Vulktech), cyan-400 (Kazend)
