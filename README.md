# Web Programming - Assignment 2

## File Organization
* `index.html`: Contains the core structural markup with 6 box elements (A through F).
* `styleA.css`: Implements Style A layout using CSS Flexbox for vertical alignment, equal spacing, alternating box background colors, and centered content.
* `styleB.css`: Implements Style B layout using inline-block elements, preventing line wraps, hover effects, and fixed positioning for the final element in the bottom-right corner.
* `README.md`: Project documentation and reflections.

## Challenges Faced
1. **Vertical Centering and Equal Spacing in Style A:** Ensuring the boxes were vertically spaced across the viewport height without shrinking or changing their 100x100 dimensions required setting `flex-shrink: 0` and properly configuring `justify-content: space-between` on the body container.
2. **Preventing Wrapping in Style B:** To keep the first five boxes on a single horizontal row even when resizing the window, `white-space: nowrap` was set on the body element alongside `display: inline-block` on the boxes.
3. **Fixed Positioning for Element F:** Keeping the last box locked in the bottom-right corner required switching its position context using `position: fixed` so it stays relative to the browser window regardless of scrolling or resizing.