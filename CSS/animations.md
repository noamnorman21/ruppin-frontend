# CSS - Animations

CSS animations make it possible to animate transitions from one CSS style configuration to another. Animations consist of two components: a style describing the CSS animation and a set of keyframes that indicate the start and end states of the animation's style, as well as possible intermediate waypoints.

## Example

Here is a simple example of a CSS animation:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>CSS Animation Example</title>
    <style>
      .example {
        width: 100px;
        height: 100px;
        background-color: red;
        position: relative;
        animation-name: example-animation;
        animation-duration: 4s;
      }

      @keyframes example-animation {
        from {
          left: 0px;
        }
        to {
          left: 200px;
        }
      }
    </style>
  </head>
  <body>
    <div class="example"></div>
  </body>
</html>
```

In this example, the `.example` div will move from left to right over a duration of 4 seconds.

## Key Properties

- `animation-name`: Specifies the name of the `@keyframes` at-rule describing the animation's keyframes.
- `animation-duration`: Specifies the length of time that an animation should take to complete one cycle.

## Additional Resources

- [MDN Web Docs on CSS Animations](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Animations)
- [CSS Tricks on Animations](https://css-tricks.com/almanac/properties/a/animation/)
