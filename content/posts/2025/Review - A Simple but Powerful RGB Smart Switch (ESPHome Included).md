---
title: Review - A Simple but Powerful RGB Smart Switch (ESPHome Included)
date: 2025-11-17
draft: false
tags:
  - tech
  - smart-home
athur: Casey Robinson
---
Today I want to talk about a simple smart switch—but with a twist. This isn’t just a basic on/off switch. It’s an **RGB smart switch**, meaning the entire interface lights up in RGB and can be fully controlled through **Home Assistant**.

The switch has **two separate lighting zones**:  
1. **The main light**  
2. **A secondary smart light**

Both can be controlled independently, giving you a lot of options for feedback lighting, color coding, scenes, or just fun effects.

Since it’s a **single-gang switch**, it works great for both simple bulbs and smart bulbs. You can tell the switch’s relay to **turn on**, **turn off**, or **toggle**, and you can choose whether button presses actually toggle the relay or are used strictly for automations.

Another great feature is the wide range of **button actions** it supports. The switch can detect:  
- **Single press**  
- **Double press**  
- **Hold**  
- **Toggle**

It recognizes these for both the “on” and “off” states, which gives you a ton of flexibility for custom controls and Home Assistant automations.

And the best part:  
**It’s 100% local.**  
The switch ships with **ESPHome pre-installed**, so there’s no cloud dependency, no required accounts, and no forced manufacturer updates.

---

## ❗ The One Downside

The only real downside is that you can’t configure it to toggle the relay when it loses connection to Home Assistant.  
You *can* add this manually through ESPHome, but it would be nice to have this behavior available from the factory as a fallback.

---

## 🔗 Product Link  
(Non-affiliated)  
https://www.amazon.com/KAUF-ESPHome-Compatible-Tasmota-Assistant/dp/B0B1CKWV7K/
---
## Notes / Links / Sources
- [Casey j Robinson YT](https://www.youtube.com/@caseystudio)
- [Tech_Addiction](https://www.youtube.com/@tech-addiction404)
- [Github](https://github.com/nt76022)