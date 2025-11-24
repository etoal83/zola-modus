# Modus Theme for Zola

An opinionated Zola theme using the [colour palette of the Modus themes](https://protesilaos.com/emacs/modus-themes-colors).

This is a port of the [hugo-modus](https://github.com/goofansu/hugo-modus) theme to Zola.

<!-- ![Screenshot](screenshot.png) -->

## Features

- **Beautiful Color Schemes**: Modus Operandi (light) and Modus Vivendi (dark) themes
- **Responsive Design**: Built with Tailwind CSS v4
- **Syntax Highlighting**: Support for code blocks with Chroma styles
- **Minimalist Layout**: Clean and readable design
- **Dark Mode**: Automatic dark mode based on system preferences
- **RSS Feed**: Built-in RSS feed generation

## Demo

- [Live Demo](https://etoal83.github.io/zola-modus)

## Installation

There are two ways to use this theme:

### Option 1: As a Git Submodule (Recommended)

Navigate to your Zola site directory and add the theme as a submodule:

```bash
cd my-zola-site
git submodule add https://github.com/etoal83/zola-modus themes/modus
```

Then, set the theme in your `config.toml`:

```toml
theme = "modus"
```

### Option 2: Clone the Theme

Clone this repository into your `themes` directory:

```bash
cd my-zola-site/themes
git clone https://github.com/etoal83/zola-modus modus
```

Then, set the theme in your `config.toml`:

```toml
theme = "modus"
```

### Option 3: Use as a Standalone Site

You can also clone this repository and use it as a complete Zola site:

```bash
git clone https://github.com/etoal83/zola-modus
cd zola-modus
zola serve
```

## Configuration

Add the following to your site's `config.toml`:

```toml
base_url = "https://example.com"
title = "Your Site Title"
description = "Your site description"

compile_sass = true
minify_html = false
build_search_index = false

generate_feeds = true
feed_filenames = ["rss.xml"]

theme = "modus"

[markdown]
highlight_code = true
highlight_theme = "css"

[extra]
# Author information
author = "Your name"

# Custom greeting for the home page
greeting = "Welcome!"

# Copyright text for footer
copyright = "&copy; 2025 Your name"

# Menu items
[[extra.menu]]
name = "Blog"
url = "/blog"

[[extra.menu]]
name = "About"
url = "/about"
```

### Available Configuration Options

#### `[extra]` Section

- `author` (String): Your name or site author
- `greeting` (String): Custom greeting text on the home page (default: "Welcome!")
- `copyright` (String): Copyright text displayed in the footer
- `menu` (Array): Navigation menu items

#### Menu Items

Each menu item should have:
- `name` (String): Display name of the menu item
- `url` (String): URL path for the menu item

## Usage

### Creating Content

Create a new blog post in `content/blog/`:

```bash
cat > content/blog/my-post.md << 'EOF'
+++
title = "My First Post"
date = 2025-01-15
description = "A brief description"

[extra]
toc = true  # Enable table of contents
+++

Your content here...
EOF
```

### Front Matter Options

#### Page Variables

- `title` (String, required): Page title
- `date` (DateTime): Publication date
- `updated` (DateTime): Last update date
- `description` (String): Page description for meta tags

#### `[extra]` Section in Pages

- `toc` (Boolean): Enable table of contents (default: false)

### Building and Serving

```bash
# Serve the site locally with live reload
zola serve

# Build the site for production
zola build
```

## Project Structure

```
.
├── theme.toml           # Theme configuration
├── config.toml          # Site configuration
├── content/
│   ├── _index.md       # Home page content
│   └── blog/
│       ├── _index.md   # Blog section
│       └── *.md        # Blog posts
├── static/
│   └── css/
│       ├── main.css    # Tailwind CSS source
│       └── dist/       # Built CSS and Chroma styles
├── templates/
│   ├── base.html       # Base template
│   ├── index.html      # Home page template
│   ├── page.html       # Single page template
│   ├── section.html    # Section list template
│   ├── 404.html        # 404 error page
│   └── partials/       # Reusable template components
├── LICENSE             # MIT License
└── README.md           # This file
```

## Customization

### Custom CSS

To add custom styles, create a `custom.css` file in your site's `static/css/` directory and reference it in your `config.toml` or templates.

### Override Templates

To customize any template, copy it from `themes/modus/templates/` to your site's `templates/` directory and modify it. Zola will use your version instead of the theme's.

## Syntax Highlighting

The theme includes custom Chroma styles for both light and dark modes:

- `static/css/dist/operandi-chroma-style.css` - Light mode syntax highlighting
- `static/css/dist/vivendi-chroma-style.css` - Dark mode syntax highlighting

These are automatically applied based on the user's system color scheme preference.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## Troubleshooting

### Theme not loading

Make sure:
1. The theme is in `themes/modus/` directory
2. Your `config.toml` has `theme = "modus"`
3. You've run `zola serve` or `zola build`

### CSS not working

Ensure `compile_sass = true` is set in your `config.toml`.

### Menu not showing

Check that you've defined menu items in the `[extra]` section of your `config.toml`.

## Credits

- Original Hugo theme: [hugo-modus](https://github.com/goofansu/hugo-modus) by [Yejun Su](https://yejun.dev)
- Modus themes color palette: [Protesilaos Stavrou](https://protesilaos.com/emacs/modus-themes-colors)
- Tailwind CSS: [https://tailwindcss.com/](https://tailwindcss.com/)

## License

This theme is licensed under the MIT License. See [LICENSE](LICENSE) for details.

- Original hugo-modus theme Copyright (c) 2024 Yejun Su
- Zola port Copyright (c) 2025 EtoAl
