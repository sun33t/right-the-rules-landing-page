# Right the Rules Landing Page

A single-page landing site for Right the Rules, a consulting service focused on compliance, change management, and organizational culture.

## Tech Stack

- **Framework**: Astro 5.x (static site generation)
- **Styling**: Tailwind CSS 3.x
- **Typography**: Open Sans via @fontsource
- **Language**: TypeScript (strict mode)
- **Linting**: ESLint + Prettier

## Commands

```bash
npm run dev      # Start dev server (localhost:4321)
npm run build    # Build static site to ./dist/
npm run preview  # Preview production build
npm run prettier # Format all files
```

## Project Structure

```
src/
├── components/     # Reusable Astro components (*.astro)
│   ├── Github.astro
│   └── LinkedIn.astro
├── pages/          # File-based routing
│   └── index.astro # Landing page (root route)
└── env.d.ts        # TypeScript type definitions

public/             # Static assets (copied as-is)
```

## Key Patterns

- **Astro components**: Use `---` frontmatter for imports/logic, template below
- **Tailwind utilities**: Prefer utility classes over custom CSS
- **Fluid typography**: Use `clamp()` for responsive text/icon sizing
- **SVG icons**: Render inline for styling flexibility

## Conventions

- Component files: PascalCase (`Github.astro`)
- Page files: lowercase (`index.astro`)
- Routes are auto-generated from `src/pages/` structure
