# Add a new blog post

## Options

### Option A — Command

```bash
hugo new blog/my-post.md
```

This creates `content/blog/my-post.md` using `archetypes/default.md`.

### Option B — Manual file

Create `content/blog/my-post.md` with at least this front matter:

```toml
+++
title = "My Post"
date = 2025-02-26T12:00:00Z
draft = false
tags = ["Hugo", "Personal"]
+++
```

Then write your Markdown below it.

## Preview locally (includes drafts)

```bash
hugo server -D
# http://localhost:1313/blog/
```

## Notes

- Images: put files in `static/images/` and reference them as `/images/filename.jpg`.
- Future-dated posts are hidden unless you use `hugo server -D -F` or set `buildFuture = true`.
- Tags appear on the single post and are used by the blog list tag filter.
