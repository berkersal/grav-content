---
title: Wayland
---

## How to Enable Wayland on My Setup


Comment
```
blacklist ttm
blacklist drm_kms_helper
blacklist drm
```
in [/etc/modprobe.d/mhwd-gpu.conf](file:///etc/modprobe.d/mhwd-gpu.conf)

<hr>

Add
```
nvidia-drm.modeset=1
```
to
`/etc/default/grub`

<hr>

Put the SDDM Wayland conf to

> `/etc/sddm.conf.d`

<hr>

Install `sddm-git`

<hr>

Disable auto-login