---
title: "Why I’m Stepping Away from NixOS (For Now)"
date: 2025-07-16
tags: ["nixos", "linux", "reflection"]
categories: ["tech"]
draft: false
---

I love NixOS. It’s one of the most unique and powerful Linux distributions out there. The idea of a fully declarative system—where everything is managed in a single configuration file—is amazing. It gives me confidence and clarity. I always know what’s on my machine, where things are configured, and how to recreate it exactly on another system.

But ironically, the same thing I love about NixOS is also why I’m stepping away from it—for now.

## The Struggle: Programming with NixOS

When I sit down to write or run a script, I often hit a wall: missing dependencies.

Since NixOS doesn’t rely on a global package manager in the traditional sense, I need to explicitly declare everything I need in a nix-shell, a flake, or in the system configuration. This becomes a friction point, especially when I’m trying to experiment, learn, or prototype.

I’m not a professional developer at the time of this writing. I’m still learning and growing in my coding journey. But I find myself spending more time configuring the environment than actually writing code. I forget which packages I need, I have to dig through documentation, and sometimes even rebuild the whole system just to get a program running.

It’s not NixOS’s fault. That’s the tradeoff you make for a reproducible, clean system. But for someone like me, it’s frustrating when I just want to get in and code.

## What I'm Switching To

For my next Linux desktop, I’m probably going with something more traditional—most likely Debian or Arch. Both offer simpler, more familiar workflows for development. If I need a library or tool, I can install it instantly with apt or pacman. No rebuilding the whole system, no worrying about nix expressions or shell environments.

Right now, I want something that gets out of my way so I can focus on learning and building. I’ll likely come back to NixOS down the road, but for now, I need to reduce friction.

## Where NixOS Still Wins: Servers and Family Systems

That said, I still love NixOS for servers. It’s perfect for creating repeatable environments, which makes it ideal for infrastructure. I plan to continue using it for my home servers—especially when combined with tools like Ansible, SNMP, webhooks, and auto-deploy scripts. Once I have my configs dialed in, I can push the same setup across multiple machines and know they’ll behave exactly the same.

I also plan to use NixOS for computers I manage for family members. As the designated “IT person” in my immediate family, I want their systems to be stable and predictable. NixOS lets me lock down everything, easily redeploy configurations, and keep things running smoothly with minimal support needs.

## Final Thoughts

NixOS is a brilliant system. It’s ideal for:

- Sysadmins  
      
    
- Infrastructure engineers  
      
    
- People who love full control over their systems  
      
    
- Developers who want reproducible, sandboxed environments  
      
    

But for new or intermediate programmers—especially those who just want to open a terminal and start building—it can feel like a wall. The need to manage environments explicitly and the learning curve around the Nix language can get in the way of momentum.

I’m not saying goodbye forever. NixOS is still part of my long-term toolset. But for right now, I need a desktop experience that supports my creative flow rather than interrupts it.

And when I’m ready to come back, NixOS will be right there waiting—reproducible as ever.

**
