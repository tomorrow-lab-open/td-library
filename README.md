# TD Library

Reusable TouchDesigner components extracted from 60+ interactive art projects.

Built by [tomorrow.lab](https://github.com/tomorrow-lab-open), Wave Pongruengkiat and Dom (Yihuan Zhou)

## What's Inside

| Category     | Modules                                                                                     | Description                                                                               |
| ------------ | ------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| `kinect/`    | Skeleton tracking, depth-to-particles, blob tracking, player recorder                       | Kinect-based modules for tracking, depth processing, and player workflows                 |
| `mediapipe/` | Hand tracking, Face tracking / face mesh, Pose tracking, Skeleton tracking, Object tracking | MediaPipe-based tracking and recognition modules                                          |
| `vfx/`       | Particles, feedback loops, instancing, point cloud, projection mapping                      | Reusable visual effect modules driven by Kinect, camera, or other data sources            |
| `sensors/`   | Arduino, thermal, Leap Motion, MQTT bridge                                                  | Hardware input and device bridge modules                                                  |
| `audio/`     | Audio analysis, beat detection                                           | Audio analysis and CHOP-based reactive control modules                                    |
| `utils/`     | Multi-screen, camera switching, device select, data recording                               | Common utility modules for screen setup, device selection, and recording interactive data |

## Usage

Each module is a self-contained `.tox` file. Drag it into your TouchDesigner project.

1. Download or clone this repo
2. Open your `.toe` project in TouchDesigner
3. Drag any `.tox` file into your network
4. Connect inputs and outputs as documented

## Module Structure

Every module follows this structure:

```text
category/module-name/
|-- module-name.tox    # Main reusable component
|-- demo.toe           # Working example
`-- README.md          # What it does, inputs, outputs, and dependencies
```



## Category READMEs

Each category folder includes its own `README.md` to explain the scope, dependencies, version differences, and internal structure of that category.

For example:

* `kinect/README.md` can describe Kinect v1, Kinect v2, and Azure Kinect workflows
* `mediapipe/README.md` can describe supported tracking types and plugin requirements
* `vfx/README.md` can describe reusable effect families and common input sources

This keeps the root README concise while allowing each category to document its own setup and module details.

## Naming Convention

All module files follow a consistent naming pattern:

```text
kinect-[function].tox   # kinect-skeleton-in.tox
mp-[function].tox       # mp-hand-tracker.tox
vfx-[function].tox      # vfx-particles.tox
sensor-[function].tox   # sensor-mqtt-in.tox
audio-[function].tox    # audio-analyzer.tox
util-[function].tox     # util-multi-screen.tox
```


## Definition of Done

A module is ready when it:

* [ ] Works standalone, drag into any project
* [ ] Has labeled inputs and outputs, with clear parameter names
* [ ] Has a README explaining what it does, how to use it, and dependencies
* [ ] Has a demo `.toe` file
* [ ] Follows the naming convention

## Status

**Phase 1: Audit** (current), reviewing 60+ past projects and identifying reusable components.

| Phase    | Timeline  | What                                          |
| -------- | --------- | --------------------------------------------- |
| Audit    | Weeks 1-2 | Open every project and map what is reusable   |
| Extract  | Weeks 3-6 | Pull components into clean `.tox` modules     |
| Document | Weeks 5-7 | Create README and demo for each module        |
| Publish  | Weeks 7-8 | Clean the repo, prepare examples, and release |

## Source Projects

These interactive art projects are the source material:

| Project          | Category  | Key Components                                  |
| ---------------- | --------- | ----------------------------------------------- |
| PADUNG KK        | Kinect    | Skeleton tracking for dance                     |
| ALaLa            | Kinect    | Depth-to-particle visuals                       |
| Kong Interactive | Kinect    | Blob tracking, 179 iterations                   |
| Khwan Dance      | Kinect    | Skeleton recording and 4 principles analysis    |
| Kwan 6060        | MediaPipe | Hand tracking                                   |
| WitinBKK         | MediaPipe | Face tracking / face mesh overlay               |
| IF               | MediaPipe | Pose tracking                                   |
| ZER0NE           | MediaPipe | Image segmentation                              |
| CEING            | MediaPipe | Full body and hand tracking, generative visuals |

## Requirements

* TouchDesigner 2023+ (free or commercial)
* Kinect v1 modules: Kinect SDK v1.8
* Kinect v2 modules: Kinect SDK v2.0
* Azure Kinect modules: Azure Kinect SDK and drivers
* MediaPipe modules: [mediapipe-touchdesigner plugin](https://github.com/torinmb/mediapipe-touchdesigner)

## Contributing

This library is built by extracting components from real projects. If you want to contribute:

1. Fork this repo
2. Add your `.tox` module following the structure above
3. Include a demo `.toe` and `README.md`
4. Submit a PR

## License

MIT

*tomorrow.lab, Chiang Mai, Thailand*
