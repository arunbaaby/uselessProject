# Interactive Story Viewer with Spotlight Effect

A unique web-based story viewer that creates an immersive reading experience by implementing a flashlight/spotlight effect that follows the user's cursor. The dark overlay with a moving spotlight enhances the atmospheric quality of horror or mystery stories.

## Features

- Dynamic spotlight effect that follows cursor movement
- Smooth spotlight animation with gradient edges
- Responsive design that works across different screen sizes
- Clean, readable typography optimized for storytelling
- Automatic canvas resizing on window resize
- Smooth scrolling support
- Prevention of right-click menu for immersion

## Technical Implementation

### HTML Structure
- Content div containing the story text
- Canvas element for the spotlight overlay
- Responsive layout with centered content

### CSS Features
- Clean, minimal styling
- Mobile-friendly design
- Fixed positioning for the canvas overlay
- Optimized typography for readability
- Pointer events disabled on the canvas to allow text interaction

### JavaScript Functionality
- Canvas-based spotlight effect
- Smooth cursor following using linear interpolation (lerp)
- Radial gradient for soft spotlight edges
- Scroll position tracking
- Window resize handling
- Continuous animation loop using requestAnimationFrame

## Usage

1. Place your story content within the `<div id="content">` element using `<p class="story-text">` paragraphs
2. The spotlight will automatically follow the user's cursor
3. The effect works while scrolling through longer content

## Customization

You can modify these values to adjust the experience:

```javascript
// Spotlight size (in pixels)
ctx.arc(mouseX, mouseY, 60, 0, Math.PI * 2);

// Spotlight smoothness (0-1, lower = smoother)
mouseX = lerp(mouseX, targetX, 0.1);

// Darkness level (0-1, higher = darker)
ctx.fillStyle = 'rgba(0, 0, 0, 0.97)';
```

## CSS Customization

```css
// Adjust text size
.story-text {
    font-size: 1.2rem;
    line-height: 1.8;
}

// Modify content width
#content {
    max-width: 80%;
}
```

## Browser Compatibility

Works in all modern browsers that support:
- HTML5 Canvas
- ES6 JavaScript
- CSS3

## Installation

1. Download all files
2. Place your story content in the HTML file
3. Open in a web browser
4. No additional dependencies required

## License

Feel free to use and modify for your own projects.

## Notes

- The spotlight effect is implemented using the Canvas API
- The effect may impact performance on lower-end devices
- Touch devices will follow touch position instead of cursor
