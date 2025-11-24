+++
title = "Welcome to the Modus Theme for Zola"
date = 2025-01-15
updated = 2025-01-16
description = "Introducing the Modus theme - a beautiful, accessible Zola theme"

[extra]
toc = true
+++

Welcome to the Modus theme for Zola! This theme brings the acclaimed Modus color schemes to the Zola static site generator, offering a beautiful and highly accessible design for your content.

## Introduction

This is the inaugural post showcasing the **Modus theme** for Zola, ported from the Hugo theme by [goofansu](https://github.com/goofansu/hugo-modus). The theme embodies the principles of accessibility, readability, and elegant simplicity.

## What Makes Modus Special?

The Modus themes stand out for several reasons:

### 1. Accessibility

The color schemes conform to the **WCAG AAA** standard, the highest level of color contrast accessibility. This means:

- Comfortable reading in any lighting condition
- Suitable for users with various visual needs
- Professional appearance that works everywhere

### 2. Dual Themes

The theme includes both color schemes:

- **Modus Operandi**: A light theme perfect for daytime reading
- **Modus Vivendi**: A dark theme that's easy on the eyes at night

The theme automatically switches based on your system preferences!

### 3. Modern Technology

Built with modern web technologies:

- Zola for blazingly fast static site generation
- Tailwind CSS v4 for efficient styling
- Responsive design that works on all devices
- Minimal JavaScript for maximum performance

## Features

The theme includes everything you need for a modern blog or website:

- Beautiful typography optimized for reading
- Syntax highlighting for code blocks
- Table of contents support (like this page!)
- Responsive navigation menu
- RSS feed generation
- Clean and semantic HTML

## Code Example

Here's a quick example showing the syntax highlighting:

```rust
fn main() {
    println!("Hello, Modus theme!");

    let colors = vec!["Operandi", "Vivendi"];
    for color in colors {
        println!("Modus {}", color);
    }
}
```

## Getting Started

To use this theme in your Zola project:

1. Add the theme as a git submodule:
   ```bash
   git submodule add https://github.com/etoal83/zola-modus themes/modus
   ```

2. Update your `config.toml`:
   ```toml
   theme = "modus"
   ```

3. Start the development server:
   ```bash
   zola serve
   ```

## Explore More

Check out the other posts on this demo site to see more of what the theme can do:

- **Typography Showcase**: See all markdown elements in action
- **Color Schemes**: Learn about the Modus color philosophy
- **Getting Started with Zola**: A beginner's guide

## Conclusion

Whether you're building a personal blog, documentation site, or portfolio, the Modus theme provides a solid, accessible, and beautiful foundation for your content.

We hope you enjoy using this theme as much as we enjoyed creating it!

---

**Note**: This post was updated on January 16, 2025 to add more details. Notice how the theme displays both the original publication date and the update date.
