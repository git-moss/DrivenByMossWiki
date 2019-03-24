# Changes

## 6.0 (Unreleased)

* Requires Bitwig 2.4.
* Generic Flexi
  * New: Use native dialog for selecting the configuration file.
* Mackie HUI
  * Support added
* Mackie MCU
  * Fixed: Knob LED was not turned off on non-existing tracks for panorama mode.
* OSC
  * Fixed: Reduced the size of a OSC bundles to stay below 64 Kb, which is the maximum for an UDP packet.

## 5.9

* Requires Bitwig 2.4.
* Beatstep
  * Fixed: Track and Device mode selection did not work.
* Maschine Mikro Mk3
  * Fixed: Pan and Send modes could not be switched.
* MCU
  * Display mode names for Track, Volume and Sends. Send modes also display the name of the send.
  * You can flip backwards through the send modes with Shift+Send.

## 5.8

* Requires Bitwig 2.4.
* Launchpad: Fixed: Switching of Note and Sequencer did not work (only if also Push 1/2 was running)

## 5.7

* Requires Bitwig 2.4.
* Launchpad
  * New: The Bootloader and Firmware version is now logged to the console
  * New: Pro: The user button acts now like the Shift button
* MCU
  * New: Option + one of the Mute buttons: Deactivate all mutes
  * New: Option + one of the Solo buttons: Deactivate all solos
* Push 1/2
  * New: Select + Mute: Deactivate all mutes
  * New: Select + Solo: Deactivate all solos

## 5.6

* Requires Bitwig 2.4.
* MCU
  * Fixed: Removed unescessary clip indication.
* Midi Monitor
  * Fixed: System Exclusive formatting was wrong.
  * Fixed: Check for MMC was wrong.
* OSC
  * Fixed: Track selection did not work when using only "select" and/or did not set 1 as parameter.
  * Fixed: Decimal changes of tempo did not work.
  * Fixed: /device/layer/{1-8}/send/{1-8}/volume and /device/layer/{1-8}/send/{1-8}/volume/touched

## 5.5

* Requires Bitwig 2.4.
* New: There is now only one version number, the number of DrivenByMoss, and one changes file in the Wiki.
* New: Extension Midi Monitor added
* Fixed: Scene navigation with cursors was broken on most devices
* Push 1/2
  * Fixed: Clip indication was broken
