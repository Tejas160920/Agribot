# AgriBot: Precision Farming Robot 🌱 

## Overview
AgriBot is an autonomous precision farming robot that leverages computer vision and deep learning to perform intelligent agricultural tasks. The software stack focuses on weed detection, depth estimation, and autonomous navigation to enable precise and environmentally conscious farming practices.

## 🔍 Key Features
- Real-time weed detection and classification using YOLOv4
- Depth estimation using monocular vision
- Autonomous navigation using ROS2 and LIDAR
- GUI for robot control and monitoring
- Environmentally conscious precision farming through optimized pesticide usage

## 🛠️ Technical Architecture

### Weed Detection System
- Implements YOLOv4 (You Only Look Once) architecture
- Uses Darknet-53 as the backbone for feature extraction
- Custom-trained on approximately 1,400 images of weeds and crops
- Real-time bounding box generation for crop-weed differentiation

### Depth Estimation
- Single-camera monocular depth estimation
- Utilizes YOLO-generated boundary boxes
- Reference-based distance calculation using known width constants
- Real-time distance measurement in inches

### Implementation Details
- Darknet framework implementation in C and CUDA
- OpenCV's `cv2.dnn_DetectionModel()` for detection pipeline
- ROS2 integration for autonomous navigation
- LIDAR-based obstacle detection and avoidance

## 🔧 Tech Stack
- YOLOv4
- Darknet
- OpenCV
- ROS2
- Python
- C/CUDA

## 📦 Installation

```bash
# Clone the repository
git clone https://github.com/Tejas160920/agribot.git

# Navigate to project directory
cd agribot

# Install dependencies
pip install -r requirements.txt

# Additional ROS2 dependencies
# Follow ROS2 installation guide for your system
```

## 🚀 Usage

1. Start the ROS2 core:
```bash
ros2 launch agribot_navigation navigation.launch.py
```

2. Run the weed detection system:
```bash
python weed_detection.py
```

3. Launch the GUI:
```bash
python gui.py
```

## 🤝 Contributing
Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

## 📄 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.


## 📞 Contact
- Tejas Gaikwad
- Email: tejasgaikwad16092002@gmail.com
- GitHub: [Tejas160920@](https://github.com/Tejas160920)
