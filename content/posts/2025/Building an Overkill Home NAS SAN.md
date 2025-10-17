---
title: Building an Overkill Home NAS SAN
draft: false
tags:
  - tag1
  - tag2
athur: Casey Robinson
---
<div style="position:relative; padding-bottom:56.25%; height:0; overflow:hidden;">
  <iframe src="https://www.youtube.com/embed/VIDEO_ID"
      style="position:absolute; top:0; left:0; width:100%; height:100%; border:0;"
      allowfullscreen>
  </iframe>
</div>
****
I needed a network storage solution to store my data and support virtual machines. Since I change operating systems often—sometimes once a month—I wanted a reliable way to manage storage without depending on internal drives or USB sticks, which are not reliable for long-term use.  

Buying large storage for each machine is expensive and less secure. A centralized storage solution made much more sense.

---

## NAS vs. SAN: The Basics

When you think of network storage, you’re probably thinking of a NAS, since that’s what most YouTubers show off. But there are actually two different types of network storage:

### NAS (Network Attached Storage)
- File-based storage.  
- Uses protocols like **SMB** or **NFS**.  
- Most people and companies rely on **SMB** because it works across Windows, macOS, and Linux.  

### SAN (Storage Area Network)
- Block-level storage for direct connections over the local network.  
- Typically uses **iSCSI** over Ethernet or Fiber.  
- Not designed for multi-machine file sharing the way SMB is.  

---

## My Requirements
I wanted my system to be:  
- **Fast**  
- **Energy-efficient**  

Because of this, I decided to use **SSDs**. While they aren’t ideal for bulk storage, they work well as supplemental storage for my Proxmox server, which hosts my media library. I also set up an iSCSI connection for VM storage.  

---

## My Hardware Setup
- **CPU:** Ryzen 5 3600 (stock cooler)  
- **RAM:** 36GB Silicon Power Value Gaming  
- **Storage:** 4 × 2TB TEAMGROUP SSDs  
- **Boot Disk:** Crucial P3 Plus 500GB SSD  
- **Motherboard:** ASRock B450M PRO4  
- **Storage Enclosure:** ICY DOCK 6-Bay 2.5” SATA HDD/SSD  
- **Case:** RackChoice 2U Micro ATX Compact Rackmount (2 × 5.25” bays)  

The system runs **ZFS**, a powerful, scalable file system with built-in redundancy.  

---

## RAID Setup
ZFS uses RAID to stripe or mirror data across drives. A few RAID levels worth noting:  

- **RAID 0:** Stripes data for maximum speed, but lose one drive and you lose everything.  
- **RAID 1:** Mirrors data on two drives for redundancy.  
- **RAID 5:** Uses one drive for parity; can survive one drive failure.  
- **RAID 6:** Similar to RAID 5, but can survive two drive failures.  

I actually bought five SSDs, but one is a **cold spare**—ready to replace a failed drive immediately.  

⚠️ Important reminder: **RAID is not a backup**. It’s only redundancy until you can swap in a new drive and rebuild.  

---

## Movie Myth Busting
In movies, the bad guys often grab hard drives and throw them in a bag. In reality:  
1. Hard drive platters can be scratched easily, destroying the data.  
2. If the drives are part of a RAID, they need to stay in the same group (and often the same order) to work.  

---

## Future Plans
For the future, I plan to:  
- Add a **dual-port 10GbE NIC** for faster speeds.  
- Install another SSD bay.  
- Expand with **4 × 8TB HDDs** for bulk storage.  
- Enable **network booting** for my PC.  
- Eventually move to **LTO tape** for long-term archival storage.  

---

## Final Thoughts
This NAS/SAN setup is my personal overkill solution for storage, virtualization, and media. It’s been a huge step toward making my lab more reliable and flexible.  

If you’ve built your own NAS or SAN, I’d love to hear how you set yours up!  
