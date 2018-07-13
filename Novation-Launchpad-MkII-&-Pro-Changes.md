# Novation Launchpad Pro & MkII - Changes

## 3.41

Requires Bitwig 2.4.

* New: Scenes in Session view are now colored.

## 3.4

Requires Bitwig 2.3.

* New: Added Piano play view (press Note twice).
* New: Scene 1 button toggles device window in device mode.
* New: Switched function of Double and Shift+Double.
* Fixed: The duplicate button did always toggle repeat (should only when Shift is pressed).
* Fixed: Could only randomly switch to Sequencer modes.
* Fixed: Pro: Rarely happening lock up of device when switching modes (finally found it!)

## 3.3

Requires Bitwig 2.1.

* New: Press the Shift button in combination with one of the three green buttons in the right upper corner to insert an instrument, audio or effect track.
* Fixed: The new Shift+Scene clip length selection introduced in 3.2 broke the switching of drum modes. Drum modes are now toggled with the (User 1) Note button as well.

## 3.2

Requires Bitwig 2.1.

* New: In sequencer and drum mode the loop selection buttons represent now one page (not a measure as before). Pressing one of the pads selects the page. To set a "one pad" loop press the pad again.
* New: Press Shift+Scene buttons to set the preferred length for new clips.
* Fixed: Extension could crash if aftertouch was used.

## 3.1

Requires Bitwig 2.1.

* Launchpad Pro: New: Keep the Duplicate button pressed and select a clip in session mode to duplicate it
* Launchpad Pro: New: Keep the Duplicate button pressed and select a pad from the 1st row when a track mode is on to duplicate the track.
* New: Opens browser for inserting a device if none is present on a track
* New: Cursor up/down in device note moves to the next / previous device
* New: The Duplicate button (with no other button pressed) now always duplicates the first selected clip on the current track.
* Fixed: Could hang in Shift view.
* Fixed: Aftertouch was not working in Play mode.
* Fixed: Switching back from Drum 64 mode did not work and the Extension needed to be restarted

## 3.0

Requires Bitwig 2.1.

* New: Written now in Java
* New: Setting to flip the recording button behaviour
* New: Setting to auto select the drum channel
* New: Setting to turn off unused drum pads
* New: Setting to set the length for new clips
* New: Session can be flipped if Session button is pressed twice
* Launchpad Pro: New: Session "birds eye view", press Shift
* Launchpad Pro: New: Click and Record buttons are shown in different colors when active

## 2.0

Requires Bitwig 2.0.

* New: Press Shift+Device to add a device after the currently selected one
* Performance improvements

## 1.12

Requires Bitwig 1.3.15+

* New: Track scrolls into view when selected
* New: Use scene buttons in Volume mode for master volume.
* New: Use different colors for note starts and lengths in note and drum sequencer.
* New: Delete+Pad in drum sequencer now deletes all notes on that note not only 32 bars.
* New: Quantize is now working as expected (but only on selected notes). Use the properties window to set the quantize amount.
* Fixed: Scales did not update in sequencers.

## 1.11

* Launchpad Pro:
  * New: 2 new drum modes. Press Shift in drum mode and use upper 3 scene buttons to change modes. 2nd mode displays 4 drum sound, 3rd mode 8. Use the lower 4 scene buttons in 2nd mode to toggle between the drum sounds 1-4, 5-8, 9-12, 13-16. Use the lower 2 scene buttons in 3rd mode to toggle the drum sounds 1-8, 9-16.
* New: Added new 8th centered scale layouts.
* Fixed: Poly aftertouch error when note was out of range.

## 1.10

* New: Added Option: Select Clip on Launch
* New: Added Option: Behaviour on stop
* New: Octave pads in play, sequencer and raindrop view are now colored in the tracks color.
* New (only Pro): Overview navigation for session. Keep Shift button pressed in Session mode.
* New (only Pro): Implemented temporary modes for Volume, Pan and Sends button. All temporary modes on other now also turn off when no other button was pressed.
* Fixed: Track bank was not adjusted when track selection was changed in Bitwig.
* Fixed: Bank range in grouped tracks behaves weird (requires Bitwig 1.3.8 RC 2+)

## 1.02

* Fixed Polyaftertouch

## 1.01

* Fixed: Notes did not cover the full range (octave range extended).

## 1.00

* Initial Release.
