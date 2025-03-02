# SPA Loading Indicator 🌱

A lightweight, configurable loading screen for Single Page Applications that shows real-time progress while resources load. Perfect for Angular, React, Vue, or any SPA framework.

### Pro tip: Simply copy-paste the sample code into your app root html tag. Update the H1 tag content.

![image](https://github.com/user-attachments/assets/b6bd693a-5169-4e99-a091-d76e021a9367)

## Features ✨

- Real-time progress calculation based on resource sizes
- Supports both scripts and stylesheets
- Smooth progress bar animations
- Fallback timeout system
- Ultra-lightweight (no dependencies)
- Easy to customize and integrate

## Installation & Usage 🚀

1. Add the loading screen HTML to your root component:
```html
<app-root>
  <!-- Paste the loading screen code here -->
  <div id="loading-screen" class="loading-screen">
    [...]
  </div>
</app-root>
```
2: Ensure it's placed before your app's main content



## Configuration ⚙️
Customize in the CONFIG object:

```javascript
const CONFIG = {
  resourceTypes: ['script', 'link[rel="stylesheet"]'], // Elements to track
  transitionDuration: 300, // Progress bar animation duration (ms)
  minimumDisplayTime: 500, // Minimum display time (ms)
  fallbackTimeout: 10000 // Fallback timeout (ms)
};
```

## Customization 🎨
Modify the CSS to match your brand:

```css
.loading-screen {
  background-color: #ffffff; /* Background color */
}

.progress-bar-container {
  background-color: #e0e0e0; /* Track color */
  height: 20px; /* Progress bar height */
  border-radius: 10px; /* Rounded corners */
}

.progress-bar {
  background-color: #4caf50; /* Progress color */
}

.progress-percentage {
  color: #333333; /* Text color */
  font-size: 24px; /* Text size */
}
```

## How It Works 🔧
- Detects all resources in the document
- Calculates total resource sizes using HEAD requests
- Tracks loading progress of each resource
- Updates progress bar and percentage in real-time
- Automatically handles completion and errors

## Contributing 🤝
Contributions are welcome! Please follow the contribution guidelines.

## License 📄
MIT © 
