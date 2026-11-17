# oculus-positional-tracking: maintenance context

Read this file, then SKILL.md, README.md and linked recovery/provenance records. Current update: 17 November 2026.

RiftFusion investigated adding headset position tracking through KinectFusion or Vicon, with tracking providers, a position server and a consumer application.

## Original material

The original image, 13-slide presentation and historical video link are preserved. No source, tracking dataset, executable or build configuration has been recovered. Original source, submodule pins, images, reports, slides, notices and author-response records are unchanged. [Historical implementation and recovery notes](docs/RECOVERY.md) retain the earlier setup and failed-build evidence; existing PROVENANCE.md or source/PROVENANCE.json remains authoritative where present.

## Updated demo

Play a generated head trajectory and vary noise, sample delay and exponential smoothing; export the synthetic samples. This is new independent JavaScript/Canvas code in docs/, not a restored or ported historical application. No KinectFusion/Vicon recordings or original API run here. Noise and frame-delay controls are illustrative parameters, not measured sensor performance.

Run https://twerdster.github.io/oculus-positional-tracking/ or `python3 -m http.server 8000 --directory docs` from the repository root. No build, account, SDK or external service is required. Serve docs/ as the GitHub Pages source.

## Checks and review

updated/VALIDATION.json records 11 passing Chromium browser assertions for the new demo, including responsive layout checks; these are scoped interaction checks on synthetic/local examples. No original native build, sensor accuracy or physical-mobile/Safari/Firefox coverage was added. Two Claude CLI editorial passes reviewed the concise README and new-demo guide; useful wording and scope qualifications were checked against code and recovery records. Detailed review records are private.

Preserve attribution, original bytes and licensing boundaries. New demo code has a scoped MIT license in docs/DEMO-LICENSE.txt; it does not cover historical materials or third-party dependencies. Correspondence, personal contact data and machine-specific setup details stay private. Before every commit review and synchronize this file and SKILL.md.
