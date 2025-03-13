# CSS Style Inline / Internal / External

## Table of Contents

1. [Inline CSS](#inline-css)
2. [Internal CSS](#internal-css)
3. [External CSS](#external-css)

## Inline CSS

Inline CSS is used to apply a unique style to a single HTML element. It uses the `style` attribute of the HTML element.

Example:

```html
<p style="color: blue;">This is a blue paragraph.</p>
```

## Internal CSS

Internal CSS is used to define styles for a single HTML page. It is defined in the `<head>` section of an HTML file, inside a `<style>` tag.

Example:

```html
<!DOCTYPE html>
<html>
  <head>
    <style>
      p {
        color: red;
      }
    </style>
  </head>
  <body>
    <p>This is a red paragraph.</p>
  </body>
</html>
```

## External CSS

External CSS is used to define styles for multiple HTML pages. It is defined in an external `.css` file and linked to the HTML files.

Example:

```html
<!DOCTYPE html>
<html>
  <head>
    <link rel="stylesheet" type="text/css" href="styles.css" />
  </head>
  <body>
    <p>This is a paragraph styled with external CSS.</p>
  </body>
</html>
```

`styles.css`:

```css
p {
  color: green;
}
```
