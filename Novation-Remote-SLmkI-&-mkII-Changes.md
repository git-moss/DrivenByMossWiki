# 4.00
Requires Bitwig 2.0.
* Fixed: "None" is now display as device name when no device is selected.
* Fixed: Display was empty when a track name contained non-ASCII characters (e.g. ä, ö, ü, ß).

# 3.03
Requires Bitwig 1.3.15+
* Fixed: Modifying discrete parameters like "On/off" did not work.

# 3.02
Requires Bitwig 1.3.15+
* New: Track scrolls into view when selected
* New: Replaced Browser toggling in first row with the option to open/close the VST window.

# 3.01
* New: New option in the script settings to turn on mode selection with drum pads to work around a problem with the Remote Zero MkII.
* New: Added Option: Behaviour on stop
* Fixed: Track bank was not adjusted when track selection was changed in Bitwig.
* Fixed: Bank range in grouped tracks behaves weird (requires Bitwig 1.3.8 RC 2+)

# 3.00
Compatible with Bitwig 1.2.
* Support for new browser
* Fixed track navigation for effect tracks.
* Added preferences option to hide crossfader option from track (gives you 1 additional Send).
* Specific scripts for MkI and MkII.
* Support for Tap Tempo button on MkI (thanks to adamlwatson).

# 2.01
Compatible with Bitwig 1.1.x.

# 2.00
Compatible with Bitwig 1.1.x.
* New mode with Scene / Drum Sequencer
* P1 ("Page" on the Zero) changes now modes of the selected row to better support the Zero model which does not have row selection buttons.
* Improved startup code to prevent the "Ableton is offline" message.
* Added LED feedback for Device Modulation page
* Fixed switching of track modes (normal, fx, master)
* Fixed switching to device mode.
* Fixed display redraw problem when changing track banks (with P2).

# 1.3
Compatible with Bitwig 1.1.x.
* Support for direct parameters (relevant for VSTs).
* Added button state lights for device left/right, device enablement, selected clip lengths and metronome.
* Current device and track bank modes are displayed in Bitwig.
* On track bank change the 1st channel of the bank is selected.
* Bugfix: Added missing Channel Aftertouch.
* Bugfix: Button state of Write was always off.
* Bugfix: Incorrect spacing between cells in Display.

# 1.20
Compatible with Bitwig 1.1.
* Added crossfade parameter to track mode. Removed 1 send channel.
* Option added to the preferences dialog to configure the touchpad.
* Replaced tap tempo with new native function.
* Performance increase.
* Bugfix: Modulation Wheel did not work.

# 1.10
Compatible with Bitwig 1.0.14.
- Press knob row 2 selection button multiple times to toggle between normal tracks, effect tracks and the master track
- Selecting a track does no longer switch to volume mode
- In Track mode only the available Sends are shown
- In Track mode the Sends are displayed with their name
- Master mode indicates 'Master' on the right
- Autodetect for Linux added.
- Bugfix: "New" function did not work.