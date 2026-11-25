# Robot Models Repository

This repository contains 3D models for nine Deep Robotics robots: **Lite3**, **M20**, **M20S**, **X30**, **M20_Piper**, **DR02 Pro**, **DR02 Standard**, **S10**, and **S10_Piper**. Models are provided in MJCF, URDF, and, where available, USD formats. To visualize a model and take measurements, we recommend using this [Deep Robotics viewer](https://developer.deeprobotics.cn/viewer/) — just drag the model folder onto the web page.

High-resolution models are available on [Google Drive](https://drive.google.com/drive/folders/1EOELXUYSBPEJeD0rUIkJxnlLMDr6IHBV?usp=sharing) and are intended for use with modern simulators such as Isaac Lab and Isaac Sim. The low-resolution models bundled in this repository are provided for broad compatibility with older simulators.

The M20S MJCF and USD use the URDF’s link masses and inertia tensors, collision shapes, joint position and effort limits, and camera and lidar mounting frames. The MJCF stores each URDF velocity rating in joint `user[0]` (rad/s) for controllers. Its torque motors do not enforce a speed cap. The low-resolution model uses STL visuals and the high-resolution model uses DAE visuals.

Lite3 sensor frames were corrected on 2026-10-27: the D435i and MID360 mounting frames tilt downward by 20° and 15°, respectively. The URDF and USD define mounting frames; the USD also supplies optical frame transforms without active camera or lidar prims. The MJCF aligns its camera and single-ray rangefinder axes with these mounts.

Each high-resolution URDF matches its low-resolution counterpart in all model fields except the visual mesh references and mesh directory. DR02 Pro uses one box per hand for collision in URDF, MJCF, and USD. Each box encloses both visual mesh resolutions.

## Model Overview

| Robot Model | High-Resolution Render | Low-Resolution Render |
|:-----------:|:----------------------:|:---------------------:|
| **Lite3** | <img src="./images/rendered/gridless/high_res/LITE3-H-stance.png" width="320" alt="High-resolution Lite3 render" /> | <img src="./images/rendered/gridless/low_res/LITE3-stance.png" width="320" alt="Low-resolution Lite3 render" /> |
| **M20** | <img src="./images/rendered/gridless/high_res/M20-H-stance.png" width="320" alt="High-resolution M20 render" /> | <img src="./images/rendered/gridless/low_res/M20-stance.png" width="320" alt="Low-resolution M20 render" /> |
| **M20S** | <img src="./images/rendered/gridless/high_res/M20S-H-stance.png" width="320" alt="High-resolution M20S render" /> | <img src="./images/rendered/gridless/low_res/M20S-stance.png" width="320" alt="Low-resolution M20S render" /> |
| **M20_Piper** | — | <img src="./images/rendered/gridless/low_res/M20P-stance.png" width="320" alt="Low-resolution M20 Piper render" /> |
| **X30** | <img src="./images/rendered/gridless/high_res/X30-H-stance.png" width="320" alt="High-resolution X30 render" /> | <img src="./images/rendered/gridless/low_res/X30-stance.png" width="320" alt="Low-resolution X30 render" /> |
| **DR02 Pro** | <img src="./images/rendered/gridless/high_res/DR02P-H.png" width="320" alt="High-resolution DR02 Pro render" /> | <img src="./images/rendered/gridless/low_res/DR02P.png" width="320" alt="Low-resolution DR02 Pro render" /> |
| **DR02 Standard** | <img src="./images/rendered/gridless/high_res/DR02D-H.png" width="320" alt="High-resolution DR02 Standard render" /> | <img src="./images/rendered/gridless/low_res/DR02D.png" width="320" alt="Low-resolution DR02 Standard render" /> |
| **S10** | <img src="./images/rendered/gridless/high_res/S10-H-stance.png" width="320" alt="High-resolution S10 render" /> | <img src="./images/rendered/gridless/low_res/S10-stance.png" width="320" alt="Low-resolution S10 render" /> |
| **[S10_Piper](./S10_Piper)** | — | <img src="./images/rendered/gridless/low_res/S10P-stance.png" width="320" alt="Low-resolution S10 Piper render" /> |


## Contributors

See the [Contributors](Contributors.md) page for a list of contributors.
