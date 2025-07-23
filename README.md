# Pixar Lamp Robot Animation

A 3D HTML canvas application that renders a Pixar-style lamp robot with animation capabilities.

## Features

- **3D Rendering**: Uses Three.js for high-quality 3D graphics
- **Lamp Robot Model**: Realistic 3D model with base, arm, joint, head, and light bulb
- **Animation System**: Supports keyframe-based animations with bezier curve interpolation
- **Interactive Controls**: Manual control over robot properties
- **JSON Animation**: Loads animation data from JSON files

## Robot Properties

1. **Brightness**: Controls the light bulb intensity (0-100%)
2. **Rotation**: Rotates the head horizontally (0-359°, 180° = forward)
3. **Tilt**: Tilts the head vertically (-30° to 90°, 0° = horizontal)

## Animation Features

- **Frame Rate Control**: Configurable playback speed (1-120 FPS)
- **Keyframe Animation**: Smooth interpolation between keyframes
- **Bezier Curves**: Custom easing functions for natural motion
- **Looping**: Optional animation looping
- **Frame Scrubbing**: Manual frame-by-frame control

## Files

- `index.html` - Main application file
- `robot_animation_schema.json` - Animation configuration schema
- `robt_animation_example.json` - Example animation data
- `requirement.txt` - Project requirements

## Usage

1. Open `index.html` in a modern web browser
2. Use the control panel to:
   - Play/Pause/Reset animation
   - Manually adjust brightness, rotation, and tilt
   - Scrub through animation frames
3. The robot will animate according to the JSON configuration

## Animation JSON Format

The animation system uses a JSON format with:
- Frame rate and timing settings
- Keyframe arrays for each property
- Bezier curve control points for smooth interpolation
- Support for brightness, rotation, and tilt animations

## Technical Details

- **3D Engine**: Three.js r128
- **Rendering**: WebGL with antialiasing and shadows
- **Animation**: Custom keyframe interpolation with bezier curves
- **UI**: Modern CSS with backdrop blur effects
- **Responsive**: Adapts to window resizing

## Browser Compatibility

Requires a modern browser with WebGL support:
- Chrome 51+
- Firefox 51+
- Safari 10+
- Edge 79+