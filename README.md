# Full positional tracking for Oculus Rift

<p align="center">
  <img src="assets/project-preview.jpg" alt="A user wearing an Oculus Rift headset and holding a handheld rig in a lab, with an inset of the stereo headset view" width="460">
</p>

![Platform: Oculus Rift](https://img.shields.io/badge/platform-Oculus%20Rift-lightgrey)
![Source: not recovered](https://img.shields.io/badge/source-not%20recovered-lightgrey)
![Archive: historical student project](https://img.shields.io/badge/archive-historical%20student%20project-informational)

A documentation record of a project investigating positional tracking for an Oculus Rift headset.

Students: [Dor Goldbaum](https://www.linkedin.com/in/dorgold/), [Vlady Ostrovski](https://www.linkedin.com/in/vladislav-ostrovski-b99619121/).

Supervision: Aaron Wetzler.

## Available materials

The historical student project investigated two approaches to adding positional tracking to an Oculus Rift headset. This repository preserves the project description, credits, archived figure and the [original 13-slide Hebrew presentation](original/RiftFusion-Presentation.pptx), supplied by Dor Goldbaum in November 2026.

The presentation describes a head-mounted depth camera using KinectFusion and a Vicon camera system. The presentation divides the design into tracking providers, a position server with a TCP/IP API, and a consumer application. The slides discuss filtering and show API declarations for initialization, filter parameters and position/rotation exchange. These document the historical design; no implementation of that API is included here.

No application source, executable, tracking dataset or build configuration has been recovered. In November 2026, Vlady Ostrovski reported having no surviving project material and Dor could not find the code.

## Use and validation

Open the presentation in PowerPoint, LibreOffice Impress or another PPTX reader to inspect the original design. There is no tracking software to install or run from this repository.

The slides assume a single user in a known room with fixed lighting and a bounded movement area. They report a preference for Vicon over the KinectFusion approach, but provide no numerical accuracy comparison or latency measurements. The Vicon slide lists 120 Hz as a system output rate; this is a historical description, not a benchmark reproduced during recovery.

All 13 slides were rendered with LibreOffice and reviewed during recovery. No source build, headset test, tracking experiment or API execution was performed. No SDK versions are recorded in the recovered materials, and support for current headsets is unverified.

## Links

- [Original RiftFusion presentation (PPTX)](original/RiftFusion-Presentation.pptx)
- [Project entry on Aaron Wetzler's website](https://twerdster.github.io/#full-positional-tracking-for-oculus-rift)
- [Material provenance](PROVENANCE.md)
- [Video linked by the existing project record (not reviewed)](https://www.youtube.com/watch?v=3Y0BYmFOAVQ)

## Attribution and reuse

The student names follow the archived project page. Their profile links were supplied by the respective students in November 2026. The presentation is retained unchanged as original project material. This archive assigns no reuse license to the presentation, figure or other materials. The deck includes third-party illustrations and photographs that this archive does not license. Original authors can open an issue to contribute updates or request corrections or removal of their material.

Figure provenance: `assets/project-preview.jpg` is the original student-project figure from the archived project page on Aaron Wetzler's website, copied without modification.
