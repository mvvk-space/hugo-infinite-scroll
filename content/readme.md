---
title: "Theme Documentation"
date: 2023-01-02
layout: "single"
---

Welcome to the **Monoscroll** theme template. This site is designed to be a starting point for a modern, continuous-scroll blog.

## Quick Start

1.  **Clone this repository** (if you haven't already).
2.  **Run the server**: `hugo server`
3.  **Navigate to**: `http://localhost:1313`

## Naming Conventions & Content

### Creating New Posts
To create a new post, run:
```bash
hugo new content posts/my-new-post.md
```
This will create a new file in `content/posts/` with the correct frontmatter.

### Frontmatter
Each post requires the following frontmatter at the top of the file:
```yaml
---
title: "My New Post"
date: 2023-10-27T14:00:00-05:00
draft: true
tags: ["design", "code"]
categories: ["tutorial"]
---
```
*   `draft`: Set to `false` when you are ready to publish.
*   `tags` and `categories`: Use these to organize your content. The theme handles them automatically.

## Customization

### Headers & Menus
To add new items to the top navigation, edit `hugo.toml`:

```toml
[[menu.main]]
  identifier = "new-link"
  name = "New Link"
  url = "/new-link/"
  weight = 10
```

### Spinning Up New Categories
Simply add a `categories` list to your post frontmatter. Hugo will automatically generate the list pages for them.
For example, adding `categories: ["Photography"]` will create a page at `/categories/photography/` that lists all posts in that category using the continuous scroll layout.

### About & Static Pages
To create a standard page (like this one or "About"), create a markdown file in the root of `content/`:
```bash
hugo new content about.md
```
Ensure you set the layout if you want specific styling, though the default `single` layout works for most text-based pages.

## Theme Architecture
*   **`themes/monoscroll`**: logical root of the theme.
*   **`layouts/index.html`**: Controls the homepage continuous scroll.
*   **`static/css/style.css`**: All styling is here. Edit this to change colors, fonts, or glassmorphism effects.
