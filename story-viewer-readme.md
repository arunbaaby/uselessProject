# Interactive Story Viewer with Spotlight Effect

A Horror story which you can only read when you move the spotlight which is atached to the cursor.But this only works well in the desktop device

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
- Canvas element for the spotlight
- Responsive layout with centered content

### CSS Features
- Minimal styling
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

1. To read the story just move the cursor over the screen
2. The spotlight will automatically follow the user's cursor
3. The effect works while scrolling through longer content

## Installation

1. Download the index.html file on your desktop device
2. Place your story content in the HTML file
3. Open in a web browser

## Notes

- The spotlight effect is implemented using the Canvas API
- The effect only works on desktop device
- The effect doesnot work well in mobile device
