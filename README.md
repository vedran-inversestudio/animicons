# Animicons

Animicons is a project for bringing static SVG icons to life with smooth, interactive animations. On hover, icons morph by moving their SVG points, making your UI more engaging and dynamic.

## Features
- Animate SVG icons on hover using path morphing
- Powered by [anime.js](https://animejs.com/)
- Easily extendable to any SVG icon
- Simple HTML/JS setup (no build tools required)

## Getting Started

1. **Clone or download this repository.**
2. Open `demo.html` in your browser.
3. Hover over the filter icon to see the animation in action.

## How It Works
- The demo uses inline SVGs and the anime.js library to morph the icon's path data on hover.
- The animation is defined by two SVG path strings: the original and the morphed version.
- A reusable JavaScript function (`addMorphAnimation`) lets you easily add animations to any icon.

## Adding Your Own Animated Icons
1. **Inline your SVG icon** in `demo.html` (or your own HTML file). Give the `<path>` a unique `id`.
2. **Create a morphed path** for your icon. You can use an online SVG path editor like [SVG Path Editor](https://yqnn.github.io/svg-path-editor/) to tweak the shape.
3. **Call the animation function:**

```js
addMorphAnimation({
  iconId: 'yourIconContainerId',
  pathId: 'yourPathId',
  original: 'original path string',
  morphed: 'morphed path string'
});
```

4. **Repeat** for as many icons as you like!

## Dependencies
- [anime.js](https://cdnjs.cloudflare.com/ajax/libs/animejs/3.2.1/anime.min.js) (included via CDN in the demo)

## Example
See `demo.html` for a working example with the Filter icon.

## License
MIT
