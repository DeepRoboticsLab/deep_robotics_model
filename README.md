# Robot Models Repository

This repository contains 3D models for three Deep Robotics robots: **Lite3**, **M20**, and **X30**. Each model is provided in MJCF, URDF, and USD formats.

**Note**: We are using Large File System (LFS) to store large meshes. If you are trying to download the files, please use the following command. (Don't download the repo as a .zip file. The .usd and .dae files are stored using LFS and they cannot be downloaded in a .zip file.)

```bash
sudo apt update
sudo apt install git-lfs
git clone https://github.com/DeepRoboticsLab/URDF_model.git
git lfs install
git lfs pull
```
## Model Overview
**Note**: High resolution models are good for new simulators like isaaclab/isaacsim but old simulators like pybullet cannot open files this big.
| Robot Model | High Resolution Image | Low Resolution Image |
|:-----------:|:---------------------:|:--------------------:|
| **Lite3**   | <img src="./images/lite3_high_res.png" width="200" /><br>Lite3/Lite3_urdf/urdf/Lite3_high_res.urdf | <img src="./images/lite3.png" width="200" /><br>Lite3/Lite3_urdf/urdf/Lite3.urdf |
| **X30**     | <img src="./images/x30_high_res.png" width="200" /><br>X30/X30_urdf/urdf/X30_high_res.urdf | <img src="./images/x30.png" width="200" /><br>X30/X30_urdf/urdf/X30.urdf |
| **M20**     | <img src="./images/m20_high_res.png" width="200" /><br>M20/M20_urdf/urdf/M20_high_res.urdf | <img src="./images/m20.png" width="200" /><br>M20/M20_urdf/urdf/M20.urdf |

## Contributors
See the [Contributors](Contributors.md) page for a list of contributors.

