# Succulence Rover Setup and Launch Guide

Follow the setup instructions from the official repository to start either the simulation Docker environment or the physical robot Docker environment:

https://github.com/CollaborativeRoboticsLab/algorithmic-robots-world

After the environment is running:

1. Connect to the TurtleBot.
2. Open the VS Code workspace.
3. Edit `params_physical.yaml` as needed.
4. Navigate to the workspace:

```bash
cd succulence_ws
```

5. Build the workspace and source the setup file:

```bash
colcon build
source install/setup.bash
```

6. In the first terminal, launch the mission:

```bash
ros2 launch succulence_rover_ros mission_physical.launch.py
```

7. In a second terminal, start RViz:

```bash
rviz2
```

8. Open the RViz configuration file:

```text
succulence_slam_physical.rviz
```
