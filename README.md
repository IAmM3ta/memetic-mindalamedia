# MEMETiC • MiNDALA MEDiA

**Interactive Audio-Visual Synesthesia Instrument & Portfolio**

Created by Metta Thomas under MiNDALA MEDiA.

A single-file experience where touch and device orientation control a rich sinusoidal synthesizer, while custom WebGL shaders and advanced particle physics make the geometry *breathe* with the sound.

## Features

- **Playable 3D Instrument**: The glowing icosahedron is both visual centerpiece and interface
- **Touch Synthesis**: Horizontal movement controls pitch, vertical movement controls filter cutoff and amplitude
- **Gyroscopic Modulation**: Tilt your device to dynamically shape the sound and particle behavior
- **Custom WebGL Shaders**: Real-time vertex displacement and fresnel rim lighting driven by live audio analysis
- **Advanced Particle System**: 420 particles powered by curl noise + vorticity confinement for organic, fluid-like motion
- **True Synesthesia**: Sound energy directly influences scale, emissive intensity, and turbulence of the 3D scene

## How to Play

### Mobile (Best Experience)

1. Open the site on your phone
2. Scroll to the large 3D hero section
3. **Touch and hold** anywhere on the glowing icosahedron
4. **Drag your finger**:
   - Left/Right → Pitch (frequency)
   - Up/Down → Brightness & Filter (timbre)
5. **Tilt your phone** → The low-pass filter and particle field respond to orientation
6. Release your finger to gracefully fade the voices out

### Desktop

Click and drag on the 3D area. Mouse position maps similarly to touch. Gyro is not available on desktop.

## Technical Breakdown

| Layer              | Technology                          | Purpose                              |
|--------------------|-------------------------------------|--------------------------------------|
| 3D Rendering       | Three.js r134                       | Icosahedron + particle field         |
| Custom Shaders     | GLSL (Vertex + Fragment)            | Audio-reactive displacement & glow   |
| Audio Synthesis    | Web Audio API                       | 5 detuned sine oscillators + filter + delay |
| Animations         | GSAP + native requestAnimationFrame | Smooth interactions & reactivity     |
| Styling            | Tailwind CSS                        | Modern, responsive design            |
| Physics            | Custom JS (Curl Noise + Vorticity)  | Emergent swirling particle behavior  |

## Browser Compatibility

- **Recommended**: Chrome (desktop or Android)
- **iOS Safari**: Fully supported with the latest fixes (explicit `AudioContext.resume()` + short `setTargetAtTime` ramps)
- Always perform a hard refresh (`Cmd/Ctrl + Shift + R`) after updates

## Running Locally

```bash
git clone https://github.com/IAmM3ta/memetic-mindalamedia.git
cd memetic-mindalamedia
open index.html   # or double-click the file
```

No installation, build step, or dependencies required.

## Deployment

This project is ideal for GitHub Pages:

1. Go to your repository **Settings → Pages**
2. Under "Build and deployment", set Source to `main` branch and folder to `/ (root)`
3. Your live site will be available at:
   `https://iamM3ta.github.io/memetic-mindalamedia`

## Philosophy

MEMETiC treats interface as instrument and geometry as gesture. The icosahedron is not merely displayed — it is played. Sound and vision are not separate layers; they are coupled in a closed synesthetic loop.

---

**Metta Thomas** / MiNDALA MEDiA

[View Live Demo](https://iamM3ta.github.io/memetic-mindalamedia)