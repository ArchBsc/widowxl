# Interbotix WidowXL - ROS 2 Humble 

## Ρύθμιση Περιβάλλοντος

```bash
# Fix για δεκαδικά (Ελλάδα)
export LC_NUMERIC="en_US.UTF-8"

# Fix για NVIDIA/Qt (Αποφυγή GUI crashes)
export QT_QPA_PLATFORM=xcb
```

## Εγκατάσταση MoveIt 2

```bash
sudo apt update
sudo apt install ros-humble-moveit ros-humble-moveit-setup-assistant -y
```
## Build & Run

```bash
cd ~/ros2_ws

colcon build --symlink-install --packages-select my_widowxl_description
source install/setup.bash
```
## Εκκίνηση MoveIt Setup Assistant

```bash
ros2 launch moveit_setup_assistant setup_assistant.launch.py
```
