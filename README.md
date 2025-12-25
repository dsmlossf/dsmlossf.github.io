# GNBG Benchmark Website (Jekyll)

This site is set up as a **blog-style** benchmark website, with **yearly editions**.

## Quick start (GitHub Pages)

1. Create a GitHub repo and add these files.
2. In `_config.yml`:
   - Set `baseurl` to `""` for a user/organization site (`<user>.github.io`),
     or to `"/<repo-name>"` for a project site.
   - Update `benchmark_repo` to your real GitHub repository link.

## Creating an edition post

Create a new markdown file in `_posts/`:

`_posts/YYYY-MM-DD-your-title.md`

Example:

```yaml
---
title: "GNBG 2026: Call for Participation"
edition: 2026
categories: [announcement]
layout: post
---
```

The post will automatically appear under:
- `/editions/2026/` (edition page)
- the homepage (latest posts)
- `/categories/` (if you set `categories`)

## Editions pages

- `/editions/` lists all edition years that currently have posts
- `/editions/2022/`, `/editions/2023/`, ... exist as dedicated landing pages

Tip: keep one pinned “edition overview” post per year (rules + links), and use additional posts for updates/results.
