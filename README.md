# My Father's Life

A collection of stories and memories from my life, written for Lydia, Steven, Molly, Owen, and Liam.

Built with [Hugo](https://gohugo.io/) using the [Stack](https://github.com/CaiJimmy/hugo-theme-stack) theme.

## Prerequisites

- [Git](https://git-scm.com/downloads)
- [Hugo Extended](https://gohugo.io/installation/) (v0.158.0 or later)

## Getting Started

Clone the repository and pull the theme submodule:

```bash
git clone https://github.com/wingej0/jeffwinget.com.git
cd jeffwinget.com
git submodule update --init
```

Start the local dev server:

```bash
hugo server -D
```

Then open http://localhost:1313/ in your browser. The `-D` flag includes draft posts.

## Creating a New Post

```bash
hugo new content post/my-post-title.md
```

This creates a new Markdown file in `content/post/`. Open it and write your content below the front matter (the section between `---` markers). New posts default to `draft: true` — change it to `false` when ready to publish.

Posts support categories and tags in the front matter:

```markdown
---
title: "My Post Title"
date: 2026-03-20
draft: false
categories:
  - Growing Up
tags:
  - childhood
  - family
---

Your story here.
```

## Adding Images to a Post

To include images in a post, convert it to a page bundle:

1. Create a directory: `content/post/my-post-title/`
2. Move the Markdown file into it as `index.md`
3. Place images in the same directory
4. Reference them in Markdown: `![description](image.png)`

## Building for Production

```bash
hugo
```

This generates the site in the `public/` directory.
