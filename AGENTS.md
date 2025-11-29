# AGENTS.md

## Build Commands
- `jekyll serve` - Local dev server at http://localhost:4000
- `bundle exec jekyll build` - Production build to `_site/`
- `bundle install` - Install dependencies

## Project Structure
- `_posts/` - Blog posts (format: `YYYY-MM-DD-title.md`)
- `_layouts/` - Page templates (default, post, tag)
- `_includes/` - Reusable partials (header, footer)
- `assets/css/style.css` - All styles (CSS variables at top)
- `assets/images/blog/` - Blog post images
- `tags/` - Tag archive pages

## Code Style
- **CSS**: Use existing CSS variables (`--color-accent`, `--color-bg-secondary`, etc.)
- **Layouts**: Wrap content in `.container` for proper width/padding
- **Posts**: Require front matter with `layout: post`, `title`, `description`, `date`, `tags`
- **Colors**: Orange accent (`#ea580c`), blue secondary (`#3b82f6`), dark bg (`#0d0d0d`)

## Blog Documentation
See `docs/BLOGGING.md` for post creation, images, tags, and Mermaid diagrams.
