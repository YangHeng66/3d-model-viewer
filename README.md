# 3D Model Viewer

Interactive 3D product showcase built with Three.js featuring real-time model switching and mouse-driven parallax effects.

## Features

- **Multiple 3D Models**: Switch between 5 different glTF models (Helmet, Buggy, Engine, Camera, Sci-Fi Helmet)
- **Interactive Controls**: Mouse/touch-driven rotation and parallax background
- **HDR Environment**: Realistic lighting with RGBE environment mapping
- **Responsive Design**: Adapts to all screen sizes with optimized rendering
- **Performance Optimized**: Reduced motion support, efficient shadow mapping, adaptive pixel ratio

## Tech Stack

- Three.js 0.160.0
- GLTFLoader for 3D model loading
- RGBELoader for HDR environment maps
- Vanilla JavaScript (ES6 modules)

## Quick Start

1. Clone the repository
2. Open `index.html` in a modern browser
3. Click model buttons to switch between different 3D objects

No build process or dependencies required - runs directly in the browser.

## Project Structure

```
three/
├── index.html          # Main application file
├── Shopify.png         # Background image
└── 3Dmodel/           # Local 3D model storage (optional)
```

## Configuration

Key settings in `index.html`:

```javascript
const CONFIG = {
    currentModel: 'helmet',
    envUrl: 'royal_esplanade_1k.hdr',
    mouseSensitivity: 1.0,
    lerpFactor: 0.05
};
```

## Models

All models sourced from [Khronos glTF Sample Models](https://github.com/KhronosGroup/glTF-Sample-Models):

- Damaged Helmet
- Buggy Car
- 2 Cylinder Engine
- Antique Camera
- Sci-Fi Helmet

## Browser Support

Requires WebGL 2.0 support:
- Chrome 56+
- Firefox 51+
- Safari 15+
- Edge 79+

## License

MIT
