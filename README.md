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

## Turning on comments

Posts have a comment section powered by [giscus](https://giscus.app), which
stores comments in this repository's GitHub Discussions. Readers sign in with
GitHub to comment. It stays hidden until you finish these one-time steps:

1. In the repo's **Settings → General → Features**, tick **Discussions**.
2. Install the [giscus GitHub App](https://github.com/apps/giscus) on this
   repository.
3. In the **Discussions** tab, create a category called `Comments`. Use the
   **Announcement** type, so only giscus and you can start new threads.
4. Go to <https://giscus.app>, enter `bassahin/bassahin.github.io`, pick the
   `Comments` category, and copy the `data-repo-id` and `data-category-id`
   values from the generated snippet.
5. Paste them into `repo_id` and `category_id` under `comments:` in
   `_config.yml`, then push.

To turn comments off for one post, add `comments: false` to its front matter.
To turn them off everywhere, set `enabled: false`.

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
- Optional comment section via giscus (GitHub Discussions)
- No JavaScript or external requests apart from the comment section
