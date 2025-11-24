+++
title = "Getting Started with Zola"
date = 2025-01-12
description = "A beginner's guide to getting started with Zola, the fast static site generator"
+++

Zola is a fast static site generator written in Rust. It's designed to be easy to use while remaining powerful and flexible.

## Why Zola?

There are several reasons why you might choose Zola for your next project:

- **Speed**: Built in Rust, Zola is incredibly fast
- **Single Binary**: No dependencies to install, just download and run
- **Built-in Features**: Syntax highlighting, Sass compilation, and more
- **Simple**: Easy to learn and use, with great documentation

## Installation

### macOS

```bash
brew install zola
```

### Linux

```bash
# Arch Linux
pacman -S zola

# Ubuntu/Debian (via Snap)
snap install zola --edge
```

### Windows

```powershell
# Using Scoop
scoop install zola

# Using Chocolatey
choco install zola
```

## Creating Your First Site

Once Zola is installed, creating a new site is straightforward:

```bash
# Create a new site
zola init my-site

# Navigate to the directory
cd my-site

# Start the development server
zola serve
```

Your site will be available at `http://127.0.0.1:1111`.

## Basic Project Structure

A Zola project has a simple, intuitive structure:

```
my-site/
├── config.toml      # Site configuration
├── content/         # Your content (markdown files)
├── templates/       # HTML templates
├── static/          # Static files (CSS, images, etc.)
└── sass/           # Sass/SCSS files
```

## Writing Content

Create a new blog post by adding a Markdown file to the `content` directory:

```markdown
+++
title = "My First Post"
date = 2025-01-12
+++

This is my first post with Zola!
```

## Next Steps

- Read the [official documentation](https://www.getzola.org/documentation/)
- Explore available [themes](https://www.getzola.org/themes/)
- Join the [community](https://zola.discourse.group/)

Happy site building! 🚀
