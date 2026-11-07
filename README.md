# bassahin.github.io

My personal blog, built with [Jekyll](https://jekyllrb.com/) and hosted on
GitHub Pages at <https://bassahin.github.io>.

## Writing a new post

1. Add a Markdown file to `_posts/` named `YYYY-MM-DD-title.md`.
2. Start it with front matter:

   ```yaml
   ---
   title: "Post title"
   description: "One-line summary for the home page and link previews."
   tags: [tag-one, tag-two]
   ---
   ```

3. Commit and push to `main`. GitHub Pages rebuilds the site automatically.

## Customizing

| What                         | Where                             |
| ---------------------------- | --------------------------------- |
| Title, tagline, social links | `_config.yml`                     |
| Header navigation            | `nav:` in `_config.yml`           |
| Colors and fonts             | `:root` in `assets/css/main.css`  |
| About page                   | `about.md`                        |
| Page structure               | `_layouts/`, `_includes/`         |

## Running locally (optional)

```bash
bundle install
bundle exec jekyll serve
```

Then open <http://localhost:4000>.

## Features

- Home page with excerpts, yearly archive and tag index
- Dark mode that follows the system setting
- Syntax highlighting, reading-time estimate, older/newer post links
- RSS feed (`/feed.xml`) and SEO/social preview tags
- No JavaScript and no external requests
