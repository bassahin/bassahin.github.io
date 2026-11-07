---
title: "Hello, world"
description: "The first post on the new blog, and a quick tour of how it works."
tags: [meta, jekyll]
---

Welcome to the blog! This first post doubles as a cheat sheet for writing new
ones — delete it whenever you like.

## Writing a post

Every post is a Markdown file in the `_posts/` folder, named like this:

```
_posts/YYYY-MM-DD-your-post-title.md
```

At the top of each file goes a small block of *front matter*:

```yaml
---
title: "Your post title"
description: "One sentence shown on the home page and in link previews."
tags: [ideas, code]
---
```

Push the file to `main` and GitHub Pages rebuilds the site in a minute or so.

## Formatting

You get everything Markdown offers: **bold**, *italics*, `inline code`,
[links](https://github.com/bassahin), lists, and more.

> Block quotes look like this — handy for pulling out a key idea.

Code blocks are syntax-highlighted:

```python
def greet(name: str) -> str:
    return f"Hello, {name}!"

print(greet("world"))
```

| Feature        | Included |
| -------------- | :------: |
| RSS feed       | ✅       |
| Tags & archive | ✅       |
| Dark mode      | ✅       |
| SEO tags       | ✅       |

That's it. Happy writing!
