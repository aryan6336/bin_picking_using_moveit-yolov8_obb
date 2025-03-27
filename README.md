# Task
# ROS 2 Project Setup and Commands

## Execute these commands to start

```bash
cd ~/moveit2_obb
colcon build --symlink-install
source install/setup.bash
sudo apt install ros-humble-ros-gz-sim
sudo apt install ros-humble-ros-ign-gazebo
sudo apt install ros-humble-ros-gz-bridge
sudo apt install ros-humble-moveit-ros-visualization
ros2 launch panda_moveit_config moveit_gazebo_obb.py
```

---

## On new Terminal

```bash
cd ~/moveit2_obb
colcon build --symlink-install
source install/setup.bash
sudo apt install numpy==1.21.0
ros2 launch yolvo8_obb yolvo8_obb.launch.py
```

---
## On new Terminal

```bash
source moveit2_obb/install/setup.bash
rm -rf ~/.local/lib/python3.10/site-packages/cv2/qt/plugins
pip uninstall numpy -y
pip install "numpy<2" --force-reinstall
pip uninstall opencv-python -y
pip install opencv-python
cd moveit2_obb/UI
python3 bolt_selector.py

---
