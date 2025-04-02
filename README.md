# 📱 TMO Dataset

Welcome to our dataset! This collection was created using our custom smartphone application running on an **iPhone 13 Pro** with **ARKit 6**. The app captures a variety of rich sensor outputs:

- 🖼️ Synchronized RGB images  
- 🧠 Confidence maps  
- 🌊 Dense depth maps from the LiDAR scanner  
- 📈 IMU sensor data  
- 📸 SfM results from RGBD-SfM
- 📍 Camera pose trajectory (ARKit)



We provide all raw data from ARKit.

You can download the dataset from our [Google Drive](https://drive.google.com/drive/folders/1AHq_IdOLWN2_-hDrKghDJH3RUJpKE_Ic?usp=sharing).


---

## 🗂️ Dataset Types

We offer two types of datasets, tailored for different use cases:

### 1. **ARKit-Video** 🎬
- Captures **long video sequences** similar to RGBD-SLAM datasets
- 📸 Thousands of frames per sequence  
- 🖥️ Resolution: **1280x720**
- 📁 Each scene contains the following folders:
  - `cameraParam/`: Camera parameters and calibration data
  - `confidence/`: Confidence maps
  - `depth/`: Raw depth maps
  - `gravity/`: Gravity
  - `rgb/`: Original RGB images
  - `rgb_keyframe/`: Selected keyframe RGB images
  - `rgbdsfm/sfm_final`: Structure from Motion data
  - `trajectory/`: Camera pose trajectory
  - `filtered_depth/`: Processed depth maps
  - `filtered_keyframe_depth/`: Filtered depth maps for keyframes
  - `preprocessed/`: Preprocessing data for training neural surface reconstruction methods


### 2. **AR-Capture** 🎞️
- A **multi-view object dataset** created using Apple's **Object Capture** API 
- 📷 High-resolution 4K images with depth and gravity data
- 🧮 Usually fewer than 50 images per object  
- 🖼️ Image resolution: **4032x3096**
- 📁 Each scene contains the following folders:
  - `cameraParam/`: Camera parameters and calibration data
  - `confidence/`: Confidence maps
  - `depth/`: Raw depth maps
  - `gravity/`: Gravity
  - `rgb/`: Original RGB images
  - `rgb_keyframe/`: Selected keyframe RGB images
  - `rgbdsfm/sfm_final`: Structure from Motion data
  - `trajectory/`: Camera pose trajectory
  - `filtered_depth/`: Processed depth maps
  - `filtered_keyframe_depth/`: Filtered depth maps for keyframes
  - `preprocessed/`: Preprocessing data for training neural surface reconstruction methods


## 🧸 Object Categories

We currently provide data for the following 11 objects:

- 🤖 Robot Arm 2  
- 🌿 Plant  
- 🌳 Tree  
- 🛋️ Sofa  
- 🚲 Bike  
- 🪑 Recliner Chair  
- ☕ Cafe Stand  
- 🪑 Office Chair  
- 🎥 Camera Stand  
- 👟 Shoe
- 🤖 Delivery Robot
---

We hope this dataset helps you build amazing AR/AI applications! ✨  
Feel free to reach out or contribute if you're using it 💡💬

## 📚 Citation

If you use this dataset in your research, please cite our paper:

```bibtex
@inproceedings{choi2023tmo,
    title = {TMO: Textured Mesh Acquisition of Objects with a Mobile Device by using Differentiable Rendering},
    author = {Jaehoon Choi and Dongki Jung and Taejae Lee and Sangwook Kim and Youngdon Jung and Dinesh Manocha and Donghwan Lee},
    booktitle = {CVPR},
    year = {2023}
}
```

---

