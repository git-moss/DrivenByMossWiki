# Changes

## 8.00 (unreleased)

* Requires Bitwig API 9.
* Launchpad
  * New: Delete + Scene button in Session view deletes the scene
* OSC
  * New: The port of the OSC server ("receive on") can be configured again.
* Push 1/2
  * New: Added note repeat, long press Repeat button for configuration settings
  * New: Delete + Track button: Delete the track
  * New: Delete + Scene button (in Play, Piano, Drum 64, Session view): Delete the scene
  * New: Delete + pad in scene play mode: Delete the scene
  * New: Added "Clear Mute/Solo" to drum channel details
  * New: Long press the record button to configure record quantization
  * New: More parameters for note editing

## 7.11 (unreleased)

* Requires Bitwig 2.4+.


## 7.10

* Requires Bitwig 2.4+.
* Generic Flexi:
  * New: Commands to edit fx tracks. See commands in new category FX Track
  * New: Commands to edit 64 user parameters. See commands in new category User
  * Fixed: *Track: Toggle trackbank* had no effect
* Komplete Kontrol A-Series / M32
  * Fixed: Track name was not displayed
* Push 1/2
  * New: Added User mode. Allows to map 64 parameters. Press USER button to enter. Setup on Push 1 is now Shift+USER.
  * New: Push 1: Show longer track/layer names in Details mode
  * New: Push 1: Indicate volume with one bar when VU is active
  * New: Push 2: Improved layout of transport mode
  * New: Push 2: Only redraw display image if something has changed
  * Fixed: Layer details page did not close automatically when Select-button was released.
  * Fixed: Do not close transport mode when accidently tempo or position knob is touched.
  * Fixed: Push 1: Layout of panorama on max right
  * Fixed: Push 1: Send modes could not be accessed
  * Fixed: Push 1: NullPointerException if Track mode was active and an effect track was selected in Bitwig

## 7.05

* Requires Bitwig 2.4+.
* Generic Flexi:
  * New: Commands to set Solo, Mute, Rec Arm, Monitor and Auto Monitor (in addition to toggle).
* Komplete Kontrol MkII
  * New: Added control indication depending on selected mode (volume, pan, send, device parameters)
* Launchpad MkII
  * Fixed: Blinking of playing clips did not work
* MCU
  * Fixed: Volume indication was broken
* Push 1
  * Fixed: Do not send color palette request, which is only working for Push 2

## 7.04

* Requires Bitwig 2.4+.
* Ableton Push 2
  * Fixed: Improved stability writing the color palette
* Komplete Kontrol MkII
  * New: Added Send mode (CLEAR button to toggle). Edit all sends of the selected channel.
  * New: Add track number to mixer view channels
  * New: Added Recording Option: Toggle Rec Arm State of selected track
  * New: Now, first checks if the selected device on the selected channel is a Komplete 
    Kontrol devcice, if not the first instrument device is checked. This way you can edit 
    multiple Komplete Kontrol instances on a channel.

## 7.03

* Requires Bitwig 2.4+.
* All devices
  * New: Moved scale settings to document
* Ableton Push 2
  * New: Set a new color palette for the pad LEDs to be closer to the Bitwig colors.
  * Fixed: The default note view is set to Play again, was Drum View.
* APC40
  * Fixed: All views except Play View were drawn wrong.
* Komplete Kontrol MkII
  * New: Added a parameter/device mode (CLEAR button to toggle)!
* Maschine Mikro MkIII
  * Fixed: Display warning when no device is selected in parameter mode
  * Fixed: Indicate non-existing parameters as "None" in parameter mode
* MCU
  * Fixed: Jogwheel jumped back one step after movement ended
* Novation Remote SL Mk III
  * Fixed: Drawing of track and device modes were wrong when no track was selected (2nd try)
* OSC
  * Fixed: Open Stage Control template produced a crash if the master volume was changed.

## 7.02

* Requires Bitwig 2.4+.
* Novation Remote SL Mk II
  * Fixed: Drum pads did not work
  * Fixed: Crash displaying send and master track
* Novation Remote SL Mk III
  * New: The browser result name is now shown in two columns
  * Fixed: Drawing of track modes were wrong when no track was selected
  * Fixed: Track could not be added when no track was selected
  * Fixed: Browser mode could crash if a non-existing filter column was selected
  * Fixed: Button long press events caused unnecessary warnings in the log
* OSC
  * New: Added layer tab to Open Stage Control template.
  * New: Added sending of /device/layer/selected/{attributes}
  * Fixed: Some types used "selected" and some "select". Both can be used now.
  * Fixed: Fixed location of master track in Open Stage Control template for 0.47.1.

## 7.01

* Requires Bitwig 2.4+.
* Arturia Beatstep
  * Fixed: Caught exception when pads are transposed. Now an error is printed to the console.
* Generic Flexi
  * Fixed: MMC commands with device IDs > 15 did not work.
* Novation SL Mk III
  * New: Route all 16 MIDI channels to Bitwig (not only channel 1)

## 7.0

* Requires Bitwig 2.4+.
* New: Added support for Novation SL Mk III
* Fixed: scrolling of parameter pages by page bank did not work (e.g. Shift + cursor left/right on Push)
* Ableton Push 2
  * New: Deactivated channels and layers are drawn in dark colors
* Komplete Kontrol Mk II / A-series / M32
  * New: Light record button as well on clip recording and clip overdub

## 6.4

* Requires Bitwig 2.4+.
* Generic Flexi
  * New: The speed (fast and slow) for relative knob changes can be configured
  * New: A command can be assigned to be the Shift button (Global: Shift Button), which gives extra functionality if combined with another control (e.g. Play, Rewind, Forward and Knob Speeds).
* Komplete Kontrol
  * New: Mapping of first Komplete Kontrol parameter is no longer necessary
  * New: Improved automatic lookup

## 6.3

* Requires Bitwig 2.4+.
* Generic Flexi
  * New: Added setting to store the last selected mode
  * New: MIDI CC is now available as a function destination
* Komplete Kontrol
  * New: Added setting to flip the track/clip navigation of the encoder knob
  * New: Added setting to flip the clip and scene navigation of the encoder knob
  * New: Added setting to set the length of new clips
  * New: Added setting to set the behaviour on transport stop
  * New: Added M32 to the extension name

## 6.2

* Requires Bitwig 2.4+.
* APC40
  * New: Shift mode stays active until you release the Shift key.
  * Fixed: Clip indicator was not displayed.
* Launchpad Pro
  * Improved 2 colors.
* Komplete Kontrol
  * Fixed: Record option "Record clip" did not start recording when transport was stopped.
  * New: Adapted to protocol version 1.9
* Midi Monitor
  * New: Log system realtime events
  * New: Setting to filter system realtime events
* Push 1/2
  * New: You can now tweak the speed of the knobs in the settings (Workflow -> Knob Speed Normal / Knob Speed Slow)

## 6.1

* Requires Bitwig 2.4.
* Generic Flexi
  * Fixed: Exception when Send volume was mapped/changed and a FX or the Master track was selected.
* Komplete Kontrol
  * New: Added information about mute state due to soloed track(s)
  * New: Added more selected track information to confirm to updated protocol
  * New: Added scene navigation and play
  * New: Slowed down knob change rate on MkII
* OSC
  * New: You can now configure the value range. So far, this was 128. Now you can increase the range to 1024 or 16384. Note that you also need to configure the widgets in your OSC client accordingly.

## 6.0

* Requires Bitwig 2.4+.
* Generic Flexi
  * New: Use native dialog for selecting the configuration file.
  * Fixed: Fixed a typo (CC40 was named CC30).
* Komplete Kontrol
  * Switched to new MIDI protocol
  * Support for A-series and M32
* Mackie HUI
  * Support added
* Mackie MCU
  * Fixed: Knob LED was not turned off on non-existing tracks for panorama mode.
* OSC
  * Fixed: Reduced the size of a OSC bundles to stay below 64 Kb, which is the maximum for an UDP packet.
* Push
  * Automation could not be activated if an effect track or the master track was selected.

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
