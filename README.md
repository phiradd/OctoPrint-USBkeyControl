# OctoPrint-USBkeyControl
forked from pkElectronics/OctoPrint-Octoremote

No substantial changes from Octoremote have been made yet!

## Work in Progress! Use with care ##

USBkeyControl is a system to control serveral functions of your printer with a simple press of a button. Control the axis movement, manual extrusion and homing without the need of navigating through the printer menu or opening the Octopi GUI in your browser. 

USBkeyControl uses a USB keyboard or numeric keypad plugged into the Octoprint controller (Raspberry Pi, etc).

At the moment following printer actions are implemented:

* Homing X&Y and Z
* Moving of all axis
* Extrude/Retract material
* Stop Print
* Pause Print
* Start/Resume Print
* Select Extruder
* Select movement distance (4 options)

## Setup

Install via the bundled [Plugin Manager](https://github.com/foosel/OctoPrint/wiki/Plugin:-Plugin-Manager)
or manually using this URL:

    https://github.com/rmoorewrs/OctoPrint-USBkeyControl/archive/master.zip

## Configuration

Use the OctoRemote Plugin page from the Octoprint settings to adjust the parameters to your needs. Not sure if key re-mapping will be supported or not.


## Usage

Wait for Octoprint to start and start hitting the buttons, movement distance starts at Stage 1 and goes up until Stage 4 with each keypress. From Stage 4 it jumps back to 1. Same holds true for the extruder selection except that it wraps around when the number of configured extruders is reached. Keep in mind that extruding and retracting material only works if the hotend has the right temperature.

## Hardware

The original plugin uses an arduino with a custom keypad. This fork will use a standard USB keyboard or USB numberic keypad as a local keyboard controller
