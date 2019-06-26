# Orchestration of Dedicated Desktops: The ODD Office
by John Michael Eubank

This work is licensed under the Creative Commons Attribution-NonCommercial 4.0 International License. To view a copy of this license, visit http://creativecommons.org/licenses/by-nc/4.0/ or send a letter to Creative Commons, PO Box 1866, Mountain View, CA 94042, USA.

Want to roll out the ODD Office in your organization? Keep an eye on this space for links to ODD Office approved solutions. Want some help developing a commercial ODD Office solution? Drop me a line here on Github!


## Layers of the solution

* Hardware
  * Scale-out components - the desktop catalog
* Per-box software
  * BIOS, firmware
  * OS, drivers
  * Apps
* Orchestration software

## Lifecycle of the solution

* Developing the hardware catalog
* Installing software
* Deployment and testing
* Scaling out
* Migrating users
* Responding to failures
* Upgrading hardware
* Upgrading software
    * OS upgrade orchestration
    * App upgrade orchestration

## App installs as image layers

## Dual system image architecture

Inspired by the TR-069 architecture, a dual system image setup allows a given desktop to have an active system image that it's running at a given time, and an alternate image. This is also inspired by blue-green deployment methodologies. A boot pointer decides which system image to boot from, and the alternate image can be updated in the background while the active image is running.
