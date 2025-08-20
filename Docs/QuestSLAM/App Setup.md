---
title: App Setup
parent: QuestSLAM
layout: page
nav_order: 4
---
# QuestSLAM install

## Requirements
- ADB (Android Debug Bridge)
- MQDH (Meta Quest Developer Hub)


## Instalation
1. To begin plugin the headset to your computer and run `adb tcpip 5555`
2. Install the QuestSLAM application through MQDH

{: .note}
**On the first launch you will have to have the headset on to allow permissions**

3. Launch the app with `adb shell am start -n "com.kirvilnet.QuestSLAM/com.unity3d.player.UnityPlayerGameActivity`

## Command Arguements
These need to be placed after a `-e` tag

| Arguement    | Description                             |Default.            | Example           | Required |
|:-------------|:----------------------------------------|:-------------------|:------------------|:-|
| `"ip"`       | ip of rosbridge                         |`"0.0.0.0"`         | "10.7.1.10"       |✅|
| `"port"`     | port of rosbridge                       |`"9090"`            |"9090"             |✅|
| `"id"`       | ID of the QuestSLAM instance.           |`"0"`               |"567"              |✅|

