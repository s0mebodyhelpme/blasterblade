---
title: "Using amd_pstate within GRUB"
date: 2024-10-14T14:22:00+08:00
tags: [Linux, Unix, Kernel]
description: ""
---

Simply set the follow inside of _/etc/default/grub_ within the GRUB_CMDLINE_LINUX_DEFAULT= line:

```
amd_pstate=active
```

if you want to set the pstate driver for your AMD CPU to something that is focused on performance. Then, run:

```
sudo grub-mkconfig -o /boot/grub/grub.cfg
```

to regenerate the grub.cfg.
Alternatively, set the amd_pstate driver to passive or guided for less taxing workloads.
