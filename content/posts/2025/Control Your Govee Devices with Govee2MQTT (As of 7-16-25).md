---
title: "Control Your Govee Devices with Govee2MQTT (As of 7-16-25)"
date: 2025-07-16
tags: ["smart home", "mqtt", "govee", "automation"]
categories: ["tech"]
draft: false
---

Govee2MQTT is currently the best way to control your Govee devices. You’ll need an MQTT server for it to work. In this blog, I’ll be focusing on integration with Home Assistant. One awesome feature is that Govee2MQTT even controls my smart kettle, so I can have my coffee ready to go—how cool is that?

### Steps to Set It Up

Step 1: Install MQTT (if it’s not already installed).

Step 2: Install mactomqtt.

Step 3: Go to Settings in Home Assistant and enable Advanced Mode (you'll find this under your user profile).

Step 4: Visit the Govee2MQTT GitHub page and copy the repository URL.

Step 5: In Home Assistant, go to Settings > Add-ons > Add-on Store, click the three-dot menu in the top right, and select Repositories. Paste in the Govee2MQTT URL.

Step 6: After adding the repository, install the Govee2MQTT add-on. You’ll need to enter your email, password, and API key.

💡 To get your API key: Open the Govee app, go to Account > Settings, then look for something like “API Key.” Tap it, give a reason (e.g., "Home Assistant"), and you’ll get your key.

Step 7: Press Start on the add-on. Wait a few minutes—it might take some time if you have a lot of Govee devices.

  

I know Matter is out, and if your device supports it you can add it to Home Assistant, but Matter is not out and mass and you might not be able to control the effects of your device. Matter might take me few more years to replace something like Home Assistant so here is your guide on how to install govee2mqtt.

**
