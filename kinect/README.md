# Kinect

Kinect-based modules for tracking, depth processing, and player workflows.

This category groups reusable Kinect workflows extracted from past interactive art projects. Modules are organized first by **function family**, then by **device version**.

## Supported Systems

- Kinect v1
- Kinect v2
- Azure Kinect

## Structure

Inside the `kinect/` category, modules are organized like this:

```text
kinect/
|-- README.md
|-- skeleton-tracking/
|   |-- README.md
|   |-- v1/
|   |   `-- README.md
|   |-- v2/
|   |   `-- README.md
|   `-- azure/
|       `-- README.md
|-- blob-tracking/
|   |-- README.md
|   |-- v1/
|   |   `-- README.md
|   |-- v2/
|   |   `-- README.md
|   `-- azure/
|       `-- README.md
|-- depth-to-particles/
|   |-- README.md
|   |-- v1/
|   |   `-- README.md
|   |-- v2/
|   |   `-- README.md
|   `-- azure/
|       `-- README.md
`-- player-recorder/
    |-- README.md
    |-- v1/
    |   `-- README.md
    |-- v2/
    |   `-- README.md
    `-- azure/
        `-- README.md
Function Families

Current function families include:

Skeleton tracking

Blob tracking

Depth-to-particles

Player recorder

Each function family may contain separate implementations for:

v1

v2

azure

Requirements

Kinect v1 modules: Kinect SDK v1.8

Kinect v2 modules: Kinect SDK v2.0

Azure Kinect modules: Azure Kinect SDK and drivers

Workflow Notes

Tracking data is typically handled through CHOP

Depth or image-based workflows may use TOP

Different Kinect versions may have different output structures, performance, or setup requirements

Module List

skeleton-tracking/

blob-tracking/

depth-to-particles/

player-recorder/

Notes

This category focuses on Kinect-based workflows.
Version-specific details are documented inside each function family folder.
