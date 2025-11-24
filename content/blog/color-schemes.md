+++
title = "Understanding the Modus Color Schemes"
date = 2025-01-14
description = "Learn about the beautiful Modus Operandi and Modus Vivendi color schemes"
+++

The Modus theme uses the acclaimed Modus color palette designed by Protesilaos Stavrou. This post explores what makes these color schemes special.

## What are Modus Themes?

The Modus themes are a pair of highly accessible color schemes originally designed for Emacs:

- **Modus Operandi**: A light theme with excellent readability
- **Modus Vivendi**: A dark theme that's easy on the eyes

Both themes prioritize **accessibility** and **readability** while maintaining aesthetic appeal.

## Design Principles

### 1. Accessibility First

The Modus themes conform to the highest standard for color contrast (WCAG AAA), ensuring:

- Excellent readability in all lighting conditions
- Comfortable long reading sessions
- Accessibility for users with visual impairments

### 2. Semantic Color Usage

Colors are used meaningfully throughout the theme:

- Headings use distinct colors to establish hierarchy
- Links are clearly distinguishable with the blue-warmer shade
- Code syntax highlighting uses carefully selected colors
- UI elements maintain consistency

### 3. Automatic Dark Mode

The theme automatically switches between light and dark modes based on your system preferences. Try changing your system theme to see it in action!

## Color Examples

### Text Hierarchy

The theme uses different colors for different heading levels:

## Level 2 Heading (Yellow-faint)

### Level 3 Heading (Blue-faint)

#### Level 4 Heading (Magenta)

### Code Highlighting

The theme includes custom syntax highlighting for both light and dark modes:

```python
# Python example showing syntax highlighting
def greet(name: str) -> str:
    """Return a greeting message."""
    return f"Hello, {name}!"

# Function call
message = greet("World")
print(message)
```

### Interactive Elements

Links are styled with `blue-warmer` color and have a subtle hover effect:

- [Internal link example](/blog)
- [External link example](https://protesilaos.com/emacs/modus-themes)

## Try It Yourself

Change your system's color scheme preference to see how the theme adapts:

- On **macOS**: System Preferences → General → Appearance
- On **Windows**: Settings → Personalization → Colors
- On **Linux**: Depends on your desktop environment

The transition is instant and all colors remain harmonious and readable in both modes.

## Learn More

To learn more about the philosophy behind the Modus themes, visit:

- [Modus Themes Official Documentation](https://protesilaos.com/emacs/modus-themes)
- [Modus Themes Colors](https://protesilaos.com/emacs/modus-themes-colors)
