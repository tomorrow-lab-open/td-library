# TD Library

Reusable TouchDesigner components extracted from 60+ interactive art projects.

Built by [tomorrow.lab](https://github.com/tomorrow-lab-open) — Wave Pongruengkiat + Dom (Yihuan Zhou)

## What's Inside

| Category | Modules | Description |
|----------|---------|-------------|
| `kinect/` | Skeleton tracking, depth-to-particles, blob tracking, player recorder | Body tracking via Kinect sensor |
| `mediapipe/` | Hand tracking, face mesh, pose estimation | Lightweight pose/hand/face tracking |
| `vfx/` | Particles, feedback loops, instancing, projection mapping | Visual effects components |
| `sensors/` | Arduino, thermal, Leap Motion, MQTT bridge | Hardware input abstraction |
| `audio/` | Audio analysis, beat detection, CHOP-driven visuals | Audio reactive components |
| `utils/` | Multi-screen, file recording, camera switching | Common infrastructure tools |

## Usage

Each module is a self-contained `.tox` file. Drag it into your TouchDesigner project.

```
1. Download or clone this repo
2. Open your .toe project in TouchDesigner
3. Drag any .tox file into your network
4. Connect inputs/outputs as documented
```

## Module Structure

Every module follows this structure:

```
category/module-name/
├── module-name.tox    # The component (drag into any project)
├── demo.toe           # Working example
└── README.md          # What it does, inputs, outputs, dependencies
```

## Naming Convention

```
kinect-[function].tox      # kinect-skeleton-in.tox
mp-[function].tox          # mp-hand-tracker.tox
vfx-[function].tox         # vfx-particles.tox
sensor-[function].tox      # sensor-mqtt-in.tox
audio-[function].tox       # audio-analyzer.tox
util-[function].tox        # util-multi-screen.tox
```

## Definition of Done

A module is ready when it:

- [ ] Works standalone (drag into any project)
- [ ] Has labeled inputs/outputs (clear parameter names)
- [ ] Has a README (what it does, how to use, dependencies)
- [ ] Has a demo .toe file
- [ ] Follows the naming convention

## Status

**Phase 1: Audit** (current) — reviewing 60+ past projects, identifying reusable components

| Phase | Timeline | What |
|-------|----------|------|
| Audit | Weeks 1-2 | Open every project, map what's reusable |
| Extract | Weeks 3-6 | Pull components into clean .tox modules |
| Document | Weeks 5-7 | README + demo for each module |
| Publish | Weeks 7-8 | Clean repo, examples, release |

## Source Projects

These interactive art projects are the source material:

| Project | Category | Key Components |
|---------|----------|---------------|
| PADUNG KK | Kinect | Skeleton tracking for dance |
| ALaLa | Kinect | Depth-to-particle visuals |
| Kong Interactive | Kinect | Blob tracking, 179 iterations |
| Khwan Dance | Kinect | Skeleton recording + 4 principles analysis |
| Kwan 6060 | MediaPipe | Hand tracking |
| WitinBKK | MediaPipe | Face mesh overlay |
| IF | MediaPipe | Pose estimation |
| ZER0NE | MediaPipe | Image segmentation |
| CEING | MediaPipe | Full body + hand tracking, generative visuals |

## Requirements

- TouchDesigner 2024+ (free/commercial)
- Kinect modules: Kinect v2 or Azure Kinect + drivers
- MediaPipe modules: [mediapipe-touchdesigner plugin](https://github.com/torinmb/mediapipe-touchdesigner)

## Contributing

This library is built by extracting components from real projects. If you want to contribute:

1. Fork this repo
2. Add your .tox module following the structure above
3. Include a demo .toe and README
4. Submit a PR

## License

MIT

---

*tomorrow.lab — Chiang Mai, Thailand*
