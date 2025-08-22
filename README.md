# Three.js Textures Demo

A comprehensive Three.js demonstration showcasing Physically Based Rendering (PBR) materials with interactive controls. This project features multiple texture sets with full PBR material maps that can be adjusted in real-time.

## Features

- **Three Complete Texture Sets**:
  - Wispy Grass Meadow
  - Badlands Boulders  
  - Space Cruiser Panels

- **Full PBR Material Support**:
  - Albedo/Diffuse maps
  - Ambient Occlusion (AO) maps
  - Height/Displacement maps
  - Metallic maps
  - Normal maps
  - Roughness maps

- **Interactive Controls**:
  - Real-time material parameter adjustments using Tweakpane
  - OrbitControls for camera navigation
  - Responsive design

- **Modern Development**:
  - Built with Vite for fast development
  - ES6 modules
  - Clean, maintainable code structure

## Setup and Installation

1. **Clone or download the project**
   ```bash
   git clone <repository-url>
   cd texturess
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the development server**
   ```bash
   npm run dev
   ```

4. **Open your browser**
   Navigate to `http://localhost:5173` (or the port shown in your terminal)

## Usage

### Controls

- **Mouse Controls**:
  - Left-click + drag: Rotate camera
  - Right-click + drag: Pan camera  
  - Scroll wheel: Zoom in/out

- **Tweakpane Interface**:
  - Three collapsible panels for each material type
  - Adjustable parameters:
    - Metalness (0.0 - 1.0)
    - Roughness (0.0 - 1.0)
    - Displacement Scale (0.0 - 1.0)
    - AO Map Intensity (0.0 - 1.0)

### Texture Sets

#### 1. Wispy Grass Meadow
- Natural terrain texture with organic patterns
- Ideal for ground surfaces and natural environments

#### 2. Badlands Boulders  
- Rocky terrain with detailed surface variations
- Perfect for rocky landscapes and geological features

#### 3. Space Cruiser Panels
- Sci-fi industrial texture with metallic surfaces
- Great for futuristic and mechanical objects

## Project Structure

```
texturess/
├── public/
│   └── rawtextures/          # Texture assets
│       ├── wispy-grass-meadow_*.png
│       ├── badlands-boulders_*.png
│       ├── space-cruiser-panels2_*.png
│       └── uvMappingTest.jpg
├── src/
│   ├── main.js              # Main Three.js application
│   └── style.css            # Minimal styling
├── index.html               # Main HTML file
├── package.json             # Project dependencies
└── README.md               # This file
```

## Technologies Used

- **Three.js** (v0.178.0) - 3D graphics library
- **Vite** - Build tool and development server
- **Tweakpane** (v4.0.5) - GUI controls for parameter adjustment
- **OrbitControls** - Camera navigation controls

## Building for Production

To create a production build:

```bash
npm run build
```

To preview the production build:

```bash
npm run preview
```

## Customization

### Adding New Textures

1. Place texture files in `public/rawtextures/` following the naming convention:
   - `{name}_albedo.png`
   - `{name}_ao.png`
   - `{name}_height.png`
   - `{name}_metallic.png`
   - `{name}_normal-ogl.png`
   - `{name}_roughness.png`

2. Update `src/main.js` to load and configure the new textures

### Modifying Materials

The material parameters can be easily adjusted in the Tweakpane interface. For more advanced modifications, edit the material properties in `src/main.js`.

## Browser Support

This project requires a modern browser with WebGL support:
- Chrome 80+
- Firefox 78+
- Safari 13+
- Edge 80+



## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## Acknowledgments

- Texture assets provided for educational demonstration purposes
- Three.js community for excellent documentation and examples
- Vite team for the excellent development experience
