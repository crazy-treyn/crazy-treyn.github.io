# Blogging Guide

Quick reference for creating and managing blog posts.

## Creating a New Post

1. Create a file in `_posts/` with the naming format:
   ```
   YYYY-MM-DD-your-post-title.md
   ```

2. Add front matter at the top:
   ```yaml
   ---
   layout: post
   title: "Your Post Title"
   description: "Brief description for cards and SEO"
   date: 2025-11-29
   tags:
     - tag-one
     - tag-two
   ---
   ```

3. Write your content in Markdown below the front matter.

## Adding a Table of Contents

Add this anywhere in your post (typically after the intro paragraph):

```markdown
* TOC
{:toc}
```

This auto-generates links to all h2 and h3 headings.

## Images

1. Place images in `assets/images/blog/`
2. Reference in your post:
   ```markdown
   ![Alt text](/assets/images/blog/your-image.png)
   ```

Images automatically get max-width, rounded corners, and margins.

## Tags

### Using existing tags
Available tags (in `tags/` directory):
- `data-engineering`
- `microsoft-fabric`
- `power-bi`
- `python`

### Creating a new tag
1. Create `tags/your-tag.md`:
   ```yaml
   ---
   layout: tag
   tag: your-tag
   title: "Posts tagged: Your Tag"
   ---
   ```

2. Use `your-tag` in your post's front matter.

## Mermaid Diagrams

Wrap your diagram in a `<pre class="mermaid">` tag:

```html
<pre class="mermaid">
flowchart LR
    A[Start] --> B[Process]
    B --> C[End]
</pre>
```

Supports flowcharts, sequence diagrams, class diagrams, etc. See [Mermaid docs](https://mermaid.js.org/syntax/flowchart.html).

## Code Blocks

Use fenced code blocks with language identifier:

~~~markdown
```python
def hello():
    print("Hello, world!")
```
~~~

Supported: python, javascript, sql, bash, yaml, json, and more.

## Tables

Standard Markdown tables:

```markdown
| Column 1 | Column 2 |
|----------|----------|
| Value 1  | Value 2  |
```

## Blockquotes

```markdown
> This is a blockquote.
```

## Running Locally

```bash
jekyll serve
# or
bundle exec jekyll serve
```

Visit `http://localhost:4000/blog/`

## File Structure

```
_posts/           # Blog posts
assets/images/blog/  # Blog images
tags/             # Tag archive pages
blog/index.html   # Blog listing page
_layouts/post.html   # Post template
_layouts/tag.html    # Tag page template
```
