# Robot Models Repository

This repository contains 3D models for eight Deep Robotics robots: **Lite3**, **M20**, **M20S**, **X30**, **M20_Piper**, **DR02 Pro**, **DR02 Standard**, and **S10**. Models are provided in MJCF, URDF, and, where available, USD formats. To visualize a model and take measurements, we recommend using this [viewer tool](https://viewer.robotsfan.com/) — just drag the model folder onto the web page.

High-resolution models are available on [Google Drive](https://drive.google.com/drive/folders/1EOELXUYSBPEJeD0rUIkJxnlLMDr6IHBV?usp=sharing) and are intended for use with modern simulators such as Isaac Lab and Isaac Sim. The low-resolution models bundled in this repository are provided for broad compatibility with older simulators.

## Lite3 model update (2026-08-21)

The Lite3 URDF, MJCF, and USD files use the supplied 2026-08-21 OEM release. The URDF adds fixed D435i, MID360, and IMU mounting frames. The MJCF includes the corresponding sites, a fixed depth camera, a single-ray lidar rangefinder, and named IMU sensors. The USD release updates leg collisions to cylinders and revises thigh centers of mass and joint drive parameters. Meshes and the existing `Lite3/{urdf,mjcf,usd}` paths are retained.

These files retain the OEM format-specific data: thigh centers of mass differ between URDF and MJCF/USD, and the USD sensor layer contains no sensor definitions. Check these differences when transferring configurations between simulators. Four dangling USD references to empty foot visual prims were removed; the foot collision spheres and all existing visual geometry are preserved.

## Model Overview

| Robot Model | High-Resolution Render | Low-Resolution Render |
|:-----------:|:----------------------:|:---------------------:|
| **Lite3** | <img src="./images/rendered/high_res/LITE3-H.png" width="320" alt="High-resolution Lite3 render" /> | <img src="./images/rendered/low_res/LITE3.png" width="320" alt="Low-resolution Lite3 render" /> |
| **M20** | <img src="./images/rendered/high_res/M20-H.png" width="320" alt="High-resolution M20 render" /> | <img src="./images/rendered/low_res/M20.png" width="320" alt="Low-resolution M20 render" /> |
| **M20S** | — | <img src="./images/rendered/low_res/M20S.png" width="320" alt="Low-resolution M20S render" /> |
| **M20_Piper** | — | <img src="./images/rendered/low_res/M20P.png" width="320" alt="Low-resolution M20 Piper render" /> |
| **X30** | <img src="./images/rendered/high_res/X30-H.png" width="320" alt="High-resolution X30 render" /> | <img src="./images/rendered/low_res/X30.png" width="320" alt="Low-resolution X30 render" /> |
| **DR02 Pro** | <img src="./images/rendered/high_res/DR02P-H.png" width="320" alt="High-resolution DR02 Pro render" /> | <img src="./images/rendered/low_res/DR02P.png" width="320" alt="Low-resolution DR02 Pro render" /> |
| **DR02 Standard** | <img src="./images/rendered/high_res/DR02D-H.png" width="320" alt="High-resolution DR02 Standard render" /> | <img src="./images/rendered/low_res/DR02D.png" width="320" alt="Low-resolution DR02 Standard render" /> |
| **S10** | — | <img src="./images/rendered/low_res/S10.png" width="320" alt="Low-resolution S10 render" /> |


## Contributors

See the [Contributors](Contributors.md) page for a list of contributors.
