# CSS - Transitions

## Table of Contents

1. [Introduction](#introduction)
2. [Basic Example](#basic-example)
3. [Transition Properties](#transition-properties)
4. [Multiple Transitions](#multiple-transitions)
5. [Conclusion](#conclusion)

## Introduction

CSS transitions allow you to change property values smoothly (over a given duration).

## Basic Example

```html
<!DOCTYPE html>
<html>
  <head>
    <style>
      div {
        width: 100px;
        height: 100px;
        background: red;
        transition: width 2s;
      }

      div:hover {
        width: 300px;
      }
    </style>
  </head>
  <body>
    <div></div>
  </body>
</html>
```

## Transition Properties

- `transition-property`: Specifies the name of the CSS property the transition effect is for.
- `transition-duration`: Specifies how many seconds or milliseconds the transition effect takes to complete.
- `transition-timing-function`: Specifies the speed curve of the transition effect.
- `transition-delay`: Specifies when the transition effect will start.

## Multiple Transitions

To specify multiple transition properties, separate them with commas:

```css
div {
  transition: width 2s, height 2s, transform 2s;
}
```

## Conclusion

CSS transitions provide a way to control animation speed when changing CSS properties, making it easier to create smooth and visually appealing transitions.
