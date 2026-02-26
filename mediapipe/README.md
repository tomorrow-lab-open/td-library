# MediaPipe

MediaPipe-based tracking and recognition modules.

This category groups reusable MediaPipe workflows extracted from past interactive art projects.  
Modules are organized first by **function family**, then by **input source**.

## Function Families

- Hand tracking
- Face tracking / face mesh
- Pose tracking
- Skeleton tracking
- Object tracking

## Input Sources

Depending on the workflow, modules may be organized by:

- `camera`
- `kinect`

## Requirements

- MediaPipe for TouchDesigner
- Compatible camera or sensor input
- TouchDesigner 2023+

## Workflow Notes

- MediaPipe modules may use different input sources depending on project setup
- Different function families may produce different landmark, tracking, or recognition outputs
- Source-specific details are documented inside each function family folder

## Folder Structure

```text
mediapipe/
|-- README.md
|-- hand-tracking/
|-- face-tracking/
|-- pose-tracking/
|-- skeleton-tracking/
`-- object-tracking/
