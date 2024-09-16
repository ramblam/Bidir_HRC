# Bidir_HRC
This repository contains codes for a robot system combining speech recognition, TTS, object detection and robot control to enable bidirectional verbal communication in HRC:

  * perception_fusion.py: The main code of the system that combines the robot control, voice commands and object detection.
  * speech_perception.py: The action code that handles the speech recognition and TTS. Creoir Edge VUI SDK is utilized for speech recognition and TTS, see: https://creoir.com/edgevui/
  * grasp_pose_detection_detectron2.py: Handles object detection. Converts the detections from camera frame to robot frame and publishes poses of detected objects to corresponding topic.
  * Opendr_control directory: Contains the lower-level implementations for controlling the robot and gripper, such as pick&place. Largely based on MoveIt (http://moveit.ros.org/) and OpenDR (https://github.com/opendr-eu/opendr).

The demo video:

[![Watch the video](https://img.youtube.com/vi/7vJrGNcnmt4/maxresdefault.jpg)](https://youtu.be/7vJrGNcnmt4)
In case the embedded image link doesn't work, here is a direct link: https://www.youtube.com/watch?v=7vJrGNcnmt4 
