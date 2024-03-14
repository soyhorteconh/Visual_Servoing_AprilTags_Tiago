# Enhancing TIAGo Robot Capabilities: Introducing Azure Kinect DK for Advanced Grasping of Kitchen Objects
This research project illustrates robotic manipulation through the integration of visual markers, the Azure Kinect DK sensor, and the TIAGo robot. It addresses challenges in marker detection accuracy, robot hand pose estimation, and efficient object manipulation to open and close a drawer. The project showcases real-time algorithm capabilities with improved marker detection and consistent pose predictions. Reducing time execution.

## How to start the environment? ##
1. Build dockerfile (only once)
   ```
   docker build -t dockerfile .
   ```
2. Build image from dockerfile (only once)
   ```
   ./buil.sh
   ```
3. Run container (each time you'll use the container)
   ```
   ./launch_bash.sh
   ```

## How to use the environment? ##
Three main files are available in [apriltags_ws/src/apriltag_ros/apriltag_ros/scripts](https://github.com/soyhorteconh/Visual_Servoing_Tiago/tree/final_version/apriltags_ws/src/apriltag_ros/apriltag_ros/scripts). This files are the ones that allowed to analize the information from the Azure Kinect DK sensor, a visual servoing algorithm, and a simulation.
- apriltag_information_node.cpp : To enhace detection of visual markers.
- apriltag_controller_version2.cpp : A visual servoing that controls hand velocity using the robot hand pose, and the target pose.
- apriltag_visualization_node.cpp : A simulation in real time that tracks the current hand pose, and the estimated hand pose.

## Video Presentation ##
In the following video you can find more information related with the knowledge implemented to develop the algorithm.
[![Watch the video: ](https://img.youtube.com/vi/yUcmC3FrjIs/0.jpg)](https://www.youtube.com/watch?v=yUcmC3FrjIs)
