# AGENTS.md

## Build Commands
- `bundle install` - Install dependencies
- `bundle exec jekyll serve` - Local dev server at http://localhost:4000
- `bundle exec jekyll build` - Production build to `_site/`

## Project Structure
- `_posts/` - Blog posts (format: `YYYY-MM-DD-title.md`)
- `_layouts/` - Page templates (default, post, tag)
- `_includes/` - Reusable partials (header, footer)
- `assets/css/style.css` - All styles (CSS variables defined at top)
- `tags/` - Tag archive pages (create new file for each tag)

## Code Style
- **CSS**: Use existing variables (`--color-accent`, `--color-secondary`, `--spacing-*`)
- **Layouts**: Wrap content in `.container`; use Liquid templating (`{% %}`, `{{ }}`)
- **Posts**: Require front matter: `layout: post`, `title`, `description`, `date`, `tags`
- **HTML**: 2-space indent; use semantic elements; no inline styles
- **Colors**: Orange accent `#ea580c`, blue secondary `#3b82f6`, dark bg `#0d0d0d`
- **New tags**: Create `tags/<tag-name>.md` with `layout: tag` front matter

## Blog Guide
See `docs/BLOGGING.md` for posts, images, tags, TOC, and Mermaid diagrams.
