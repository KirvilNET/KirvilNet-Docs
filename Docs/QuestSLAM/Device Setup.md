---
title: Device Setup
parent: QuestSLAM
layout: page
nav_order: 2
---

Before we can use the QuestSLAM app we have to configure the headset to optimize it for QuestSLAM
# Developer account
- Follow [this guide](https://medium.com/sidequestvr/how-to-turn-on-developer-mode-for-the-quest-3-509244ccd386) to enable developer mode 
- Download the [Meta Quest Developer Hub (MQDH)](https://developers.meta.com/horizon/develop)
  
# Disable Gaurdian
- Gaurdian must be disabled to prevent app interuptions and relilablity issues.
-  Navigate to **Settings → Advanced → Experimental Settings → Enable Custom Settings**
-  Turn OFF **Physical Space Features, MTP Notification, and Link Auto Connect**
  
# Disable Bluetooth
- Bluetooth can be disabled with `adb shell svc bluetooth disable`

# Ethernet Setup

## Pick a ethernet adapter 
Here is a list of working ethernet adapters that work with the quest 3/3s. All of these provide both power and ethernet conncetions to the headset

- [Cable Matters 5-Port USB-C Hub On-The-Go](https://a.co/d/72hhWqz)
- [onn. 8-in-1 USB-C Adapter, USB 3.0 and 4K HDMI Compatible](https://www.walmart.com/ip/onn-8-in-1-USB-C-Adapter-USB-3-0-and-4K-HDMI-Compatible/590617670)
- [Belkin Connect USB-C to Ethernet + Charge Adapter 100W](https://a.co/d/grTsVxG)

---
## Pluging in
Plugin the adapter and connect the ethernet and power from a relilable poewer source

{: .note }
Wifi must be disabled to prevent conflicts with `adb shell svc wifi disable`

## Power Requirements
The internal quest battery provides around 2.5 hours of use

{: .warning }
Power sources must be able to supply 5v at 3A to charge the headset while in use

This could be done in 2 ways 
> 1. USB Power bank
> 2. 5v regulator connected to the robots battery
> 3. POE to usbc adapter

# Mounting
Mounting the Quest in an optimal location is important for the operation of the QuestSLAM application

## Mounts
There are a variety of mounts made by first robotics teams

- [Mount by 3847 spectrum](https://www.printables.com/model/1115821-spectrum-3847-quest-3s-robot-mount/related)
- [This other one from printables](https://www.printables.com/model/1324702-quest-3-headset-mount-for-robots-and-autonomous-ve?lang=de)

## Mounting position

- Mount the headset at least 12 inches (30cm) above the floor.
- Make sure the headset has a clear view.
- Make sure it will not be blocked by moving parts

# Best Pratices 

- **Cable Type:** CAT5e or CAT6 Ethernet cable
- **Length:** Ideally under 3 feet (1 meter)
- **Shielded:** Recommended in high-EMI environments
- **Strain Relief:** Consider right-angle connectors if space is limited