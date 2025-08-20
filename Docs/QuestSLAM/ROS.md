---
title: ROS2 configuration 
layout: page
nav_order: 5
parent: QuestSLAM
permalink: /QuestSLAM/ros
---

# Intro
This covers all of the ros2 topics, services, and actions and their usage.

# Topics

| Topic                         | Topic Type                          | Descriptions                                            |
|:------------------------------|:------------------------------------|:--------------------------------------------------------|
| `QuestSLAM/"id"/battery_level`| std_msgs/Float32                    |battery level as a float 0-100.                          |
| `QuestSLAM/"id"/camera`       | sensor_msgs/Image                   |Image stream from the left camera.                       |
| `QuestSLAM/"id"/odom`         | nav_msgs/msg/Odometry               |Location of the headset as an odometry message.          |
| `QuestSLAM/"id"/is_tracking`  | std_msgs/bool                       |Tracking status.                                         |
| `QuestSLAM/"id"/apriatags`    | ID of the QuestSLAM instance.       |AprialTags as a transform. One transform per tag detected|

# Services

