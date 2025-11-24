+++
title = "Typography Showcase"
date = 2025-01-10
description = "A comprehensive showcase of typography and markdown elements in the Modus theme"

[extra]
toc = true
+++

This post demonstrates all the typography and markdown elements available in the Modus theme. It's designed to showcase the beautiful Modus color palette in action.

## Headings

### Third Level Heading

This is a paragraph under a third-level heading. The Modus theme uses distinct colors for different heading levels, making your content hierarchy clear and visually appealing.

#### Fourth Level Heading

Fourth-level headings use yet another color from the Modus palette, ensuring that your document structure is always clear.

## Text Formatting

You can use **bold text** for emphasis, *italic text* for subtle emphasis, or ***bold and italic*** for maximum impact. You can also use `inline code` to highlight technical terms or code snippets.

## Lists

### Unordered Lists

- First item in the list
- Second item with some **bold text**
- Third item with `inline code`
  - Nested item one
  - Nested item two
    - Deeply nested item
- Fourth item back at the top level

### Ordered Lists

1. First step in the process
2. Second step with some explanation
3. Third step with more details
   1. Sub-step one
   2. Sub-step two
4. Final step

### Mixed Lists

1. You can mix list types
   - Unordered sub-item
   - Another unordered sub-item
2. Back to ordered list
   - More unordered items

## Code Blocks

### Rust

```rust
fn main() {
    let message = "Hello from Rust!";
    println!("{}", message);

    let numbers: Vec<i32> = (1..=5).collect();
    for num in numbers {
        println!("Number: {}", num);
    }
}
```

### JavaScript

```javascript
function greet(name) {
    return `Hello, ${name}!`;
}

const users = ['Alice', 'Bob', 'Charlie'];
users.forEach(user => {
    console.log(greet(user));
});
```

### Python

```python
def fibonacci(n):
    """Generate Fibonacci sequence up to n terms."""
    a, b = 0, 1
    for _ in range(n):
        print(a, end=' ')
        a, b = b, a + b

fibonacci(10)
```

### HTML

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Modus Theme</title>
</head>
<body>
    <h1>Welcome to Modus</h1>
    <p>A beautiful Zola theme.</p>
</body>
</html>
```

## Blockquotes

> This is a blockquote. The Modus theme styles blockquotes with a beautiful colored border and subtle background that works perfectly in both light and dark modes.

> You can have multiple paragraphs in a blockquote.
>
> Like this second paragraph here. Notice how the styling remains consistent and readable.

## Tables

| Feature | Light Mode | Dark Mode | Status |
|---------|-----------|-----------|--------|
| Typography | Excellent | Excellent | ✓ |
| Code Highlighting | Yes | Yes | ✓ |
| Responsive Design | Yes | Yes | ✓ |
| Table Styling | Beautiful | Beautiful | ✓ |

### Complex Table

| Language | Difficulty | Use Case | Popularity |
|----------|-----------|----------|------------|
| Rust | Intermediate | Systems Programming | Rising |
| Python | Beginner | Data Science, Web | Very High |
| JavaScript | Beginner | Web Development | Very High |
| Go | Beginner | Backend Services | High |

## Links

You can include [internal links](/blog) or [external links](https://www.getzola.org) in your content. External links are automatically marked with an arrow (↗) indicator.

Visit the [Zola documentation](https://www.getzola.org/documentation/) to learn more about static site generation.

## Horizontal Rule

---

## Inline Elements

Here's a paragraph with various inline elements: **bold**, *italic*, `code`, and a [link](https://example.com). You can combine these: **bold with *italic* inside** and `code with **bold**` (though the bold won't show in code).

## Edge Cases

### Long Code Lines

```rust
fn very_long_function_name_that_demonstrates_horizontal_scrolling_in_code_blocks(parameter1: String, parameter2: i32, parameter3: bool) -> Result<String, Error> {
    // This line is intentionally long to show how the theme handles horizontal scrolling
    let result = format!("Processing {} with value {} and flag {}", parameter1, parameter2, parameter3);
    Ok(result)
}
```

### Nested Lists with Code

1. First item with code example:
   ```bash
   zola serve
   ```
2. Second item with more explanation
   - Nested unordered item
   - Another nested item with `inline code`
3. Final item

## Summary

The Modus theme provides excellent typography for all standard Markdown elements, with beautiful syntax highlighting and a color palette that works perfectly in both light and dark modes.
