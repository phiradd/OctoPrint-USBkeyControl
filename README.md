# OctoPrint-USBkeyControl
forked from pkElectronics/OctoPrint-Octoremote

No substantial changes from Octoremote have been made yet!

## Work in Progress! Use with care ##

Octoremote is a system to control serveral functions of your printer with a simple press of a button. Control the axis movement, manual extrusion and homing without the need of navigating through the printer menu or opening the Octopi GUI in your browser. 

OctoRemote consists of two components, the Octoprint plugin and an arduino based hardware controller. The controller and the plugin communicate through a serial connection using a simple byte-based protocol. As OctoRemote is based on Octoprint it is totally printer independent and works easily with any Octorprint compatible printer. At the moment following printer actions are implemented:

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

    https://github.com/pkElectronics/OctoPrint-Octoremote/archive/master.zip

The plugin repository also contains the source code of the Arduino program which is necessary for the hardware controller. Installation if described in detail in the Hardware section.

## Configuration

Use the OctoRemote Plugin page from the Octoprint settings to adjust the parameters to your needs. 



The default settings were developed and tested using an Anet A8 printer.

## Usage

It´s pretty easy, wait for Octoprint to start and start hitting the buttons, movement distance starts at Stage 1 and goes up until Stage 4 with each keypress. From Stage 4 it jumps back to 1. Same holds true for the extruder selection except that it wraps around when the number of configured extruders is reached. Keep in mind that extruding and retracting material only works if the hotend has the right temperature.

## Hardware

The original plugin uses an arduino with a custom keypad. This fork will use a standard USB keyboard or USB numberic keypad as a local keyboard controller
