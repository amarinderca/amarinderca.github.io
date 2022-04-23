---
title: "pfsense firewall hardware upgrade"
date: 2020-08-13T17:25:22-07:00
draft: false
author: "amarinder"
tags:
  - pf
  - pfsense
  - firewall
  - open source
---

### What?

[pfSense](https://www.pfsense.org/) is a free firewall that you can install on any pc. I have been using it for many years.


### Why Upgrade?

I upgraded to gigabit fiber at home. My ISP provides direct sfp handoff without need for a ONT. I can bypass need for ISP provided router and directly connect pfSense to the internet.

I already own motherboard (low powered intel atom cpu embedded board), storage, RAM and DC to DC PSU. I just needed a compatiable SFP+ network card and a new case that has a pci-e slot and proper cooling capabilities.

### Hardware?

* Mobo: [Supermicro Atom A1SRi-2758F](http://www.supermicro.com/products/motherboard/atom/x10/a1sri-2758f.cfm)
* RAM: [4 x 4GB Micron DDR3 ECC SODIMM MT18KSF51272HZ-1G6K2](https://www.micron.com/products/dram-modules/sodimm/part-catalog/mt18ksf51272hz-1g6)
* Stroage: [Supermicro SSD-DM032-SMCMVN1 SATA DOM](https://www.supermicro.com/products/nfo/SATADOM.cfm)
* PSU: [PICOPSU-150-XT](https://www.mini-box.com/picoPSU-150-XT)
* SFP+ Network Card: [Chelsio T420-CR](https://www.chelsio.com/nic/t4-unified-wire-adapters/t420-cr/)
* Case: [Metalfish S2 from Taobao](https://item.taobao.com/item.htm?id=566341915363)

### Chelsio SFP+ Card?

It is very well supported by pfSense. I got it used on eBay for a reasonable price. It does run hot. I zip-tied a small fan to this card to fix this issue. The low profile bracket didn't have any locking mechanism but that was not an issue for me, it fits snugly.

![chelsio sfp+ card](https://i.postimg.cc/brTYNxps/IMG-0677.jpg)

### S2 Case from Taobao?

Cheaper than anything I could find in this form factor. Fits my requirements perfectly.

[![case-spec.png](https://i.postimg.cc/bN7kt8h8/case-spec.png)](https://i.postimg.cc/bN7kt8h8/case-spec.png)

**Pros:** Arrived in 7 business days. Has 3 pin 2x case fans. Includes case fan hub. Includes good magnetic screw driver. Solid body construction. Easy to build in.

**Cons:** Bent side panels but easy aluminum to unbend. Some damage during shipping to where motherboard mounts from stuff bouncing around. No reset button. Kapton Tape helps when dealing with bright power led.

### S2 Pictures?

![case](https://i.postimg.cc/zXgR5MRQ/IMG-0668.jpg)
![case main](https://i.postimg.cc/cCKtvkkr/IMG-0669.jpg)
![case back](https://i.postimg.cc/kMZt09D8/IMG-0670.jpg)
![case back io](https://i.postimg.cc/cCVgw7PT/IMG-0671.jpg)
![case top](https://i.postimg.cc/jSYnjXHS/IMG-0672.jpg)
![case bottom](https://i.postimg.cc/Qdg9KTmk/IMG-0673.jpg)
![mesh panel](https://i.postimg.cc/ZqVWVz1W/IMG-0667.jpg)
![side panels](https://i.postimg.cc/1z9gG3Yx/IMG-0666.jpg)
![extras](https://i.postimg.cc/Hxv7s12q/IMG-0665.jpg)

### Build Pics?

![build](https://i.postimg.cc/LXFmtCsJ/IMG-0679.jpg)


### Does it work?

![temps](https://i.postimg.cc/76zMc6DB/Annotation-2020-08-13-184354.png)
![speed test](https://i.postimg.cc/kgVCk36V/speed-test.png)
