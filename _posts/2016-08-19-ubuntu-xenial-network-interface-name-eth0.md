---
layout: post
title: "Change Network Interface to old 'eth0' Naming Scheme on Ubuntu 16.04 LTS Xenial Xerus"
tags: [ubuntu, network]
---

1. Edit */etc/default/grub*:
  ```
  GRUB_CMDLINE_LINUX="net.ifnames=0 biosdevname=0"
  ```
2. `update-grub`
3. Edit */etc/network/interfaces*, rename interface to `eth0`.
4. Reboot

---
1. [http://www.itzgeek.com/how-tos/mini-howtos/change-default-network-name-ens33-to-old-eth0-on-ubuntu-16-04.html](http://www.itzgeek.com/how-tos/mini-howtos/change-default-network-name-ens33-to-old-eth0-on-ubuntu-16-04.html)
