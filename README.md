# Bidir_HRC
This repository contains codes for a robot system combining speech recognition, TTS, object detection and robot control:

  * perception_fusion.py: The main code of the system that combines the robot control, voice commands and object detection.
  * speech_perception.py: The action code that handles the speech recognition and TTS. Creoir Edge VUI SDK is utilized for speech recognition and TTS, see: https://creoir.com/edgevui/
  * grasp_pose_detection_detectron2.py: Handles object detection. Converts the detections from camera frame to robot frame and publishes poses of detected objects to corresponding topic.
  * Opendr_control directory: Contains the lower-level implementations for controlling the robot and gripper, such as pick&place. Largely based on MoveIt (http://moveit.ros.org/) and OpenDR (https://github.com/opendr-eu/opendr).

The demo video:
(add link or whole video here!)
