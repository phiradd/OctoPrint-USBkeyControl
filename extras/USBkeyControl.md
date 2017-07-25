---
layout: plugin

id: USBkeyControl
title: OctoPrint-USBkeyControl
description: Control your 3D-Printer with a USB keyboard or numberic keypad
author: Richard Moore (forked from OctoRemote by Pascal Krumme)
license: AGPLv3

date: 2017-07-25

homepage: https://github.com/rmoorewrs/OctoPrint-USBkeyControl
source: https://github.com/rmoorewrs/OctoPrint-USBkeyControl
archive: https://github.com/rmoorewrs/OctoPrint-USBkeyControl/archive/master.zip


# library versions not yet published on PyPi. SHOULD ONLY BE USED IF THERE IS NO OTHER OPTION!
follow_dependency_links: false

# TODO
tags:
- printing
- remote
- control
- keypad
- keyboard
- USB
- remotecontrol
- ui

# TODO
screenshots:

compatibility:
  # list of compatible versions, for example 1.2.0. If left empty no specific version requirement will be assumed
  octoprint:
  - 1.2.0

  # list of compatible operating systems, valid values are linux, windows, macos, leaving empty defaults to all
  os:
  - linux
  - windows
  - macos
---

**TODO**: USBkeyControl enables you to perform all usual printer movements with a simple keypress. Current version implements moving the X-, Y- and Z-Axis, homing and controlling up to four extruders.
Movement distance of the extruders can also be controlled via the keypad.
