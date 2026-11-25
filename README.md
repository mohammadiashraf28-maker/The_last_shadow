A 30-second vertical 3D anime-horror short built with **Three.js** for the scene and **Remotion** for timeline, captions, audio, and rendering.

## Requirements
- Node.js 18.17+ (20 LTS recommended)
- npm

## Run
```bash
npm install
npm run dev
```
Open the Remotion Studio URL shown in the terminal and select `TheLastShadow`.

## Render MP4
```bash
npm run render
```
Output: `out/the-last-shadow.mp4`

## Render a poster frame
```bash
npm run still
```

## Project structure
- `src/three-scene.tsx`: procedural Three.js alley, anime-inspired girl silhouette, shadow creature, rain, fog, red moon, animated lights and camera.
- `src/the-last-shadow.tsx`: 30-second Remotion composition, English captions, audio, fade transitions.
- `public/horror-ambience.wav`: original generated ambient sound bed.

## Notes
- The 3D characters are procedural placeholder geometry, not rigged production character models. Replace them with GLB/GLTF models for detailed anime characters and skeletal animation.
- The scene is intentionally asset-light and needs no external model downloads.
- The scene uses a fixed 1080x1920 composition at 30 fps (900 frames).
- Three.js is rendered in the browser through WebGL. For headless rendering, use a machine/browser setup with WebGL enabled. If Chromium reports a WebGL context error, enable GPU/WebGL support for Remotion's Chromium environment.
- Captions are currently English. Edit the `captions` array in `src/the-last-shadow.tsx` to change the wording or timing.
