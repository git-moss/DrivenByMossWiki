# Bitwig Studio | Native Instruments Maschine Mikro Mk3 (unreleased)

Support for Native Instruments Maschine Mikro Mk3.

This extension uses the MIDI mode of the device. Press **Shift + Project** (on the left / top) buttons to enter MIDI mode.

The **Shift** and **Cursor buttons** do not send MIDI values, therefore they cannot be used.

## Transport

* **Play** - Start/Stop playback. Double click to move play cursor to the start of song. You can configure the behavior on stop in the preferences.
* **Rec** - Start/Stop recording.
* **Stop** - Stop playback. If pressed when stopped the play cursor is moved to the start of the song.
* **Restart/Loop** - Toggle transport loop
* **Erase** - Undo
* **Tap** - Toggle metronome
* **Follow** - Quantize the selected clip

## Browser

* **Projects** - Open the browser to add a device on the selected channel
* **Favorites** - Toggle the selection of Favorites in the browser
* **Browser** - Open the browser

In the browser ...
* use the Encoder to scroll through the items.
* Press the Encoder to confirm your selection and close the browser.
* Press the browse button to discard your selection and close the browser.

## Encoder modes

* **Volume** - Enables volume/pan/Sends mode. Press again to toggle between volume, pan and sends mode. The encoder changes the volume/pan/sends of the selected track. Press the encoder to set the parameter to its default value.
* **Swing** - Enables position mode. The encoder changes the position of the play cursor in the arranger. Press the encoder to move the play cursor to the start of the song.
* **Tempo** - Enables tempo mode. Press again to toggle between fine tune and normal change. The encoder changes the tempo of the song. Press the encoder to set the fraction to zero in fine tune mode and to 120 bpm in normal change mode.
* **Plug-In** - Enables device mode. The encoder changes the value of a device parameter. Press the encoder to toggle between the parameters.
* **Sampling** - TODO

## Touchstrip

The Touchstrip behaves based on the following modes.

* **Pitch** - Set the Touchstrip to send pitch bend.
* **Mod** - Set the Touchstrip to send modulation (CC 1).
* **Peform/FX Select** - Set the Touchstrip to replicate the behaviour of the Encoder (e.g. change volume).
* **Notes** - Set the Touchstrip to change the volume of the Master track.

## Automation

* **Group** - Creates a new clip on the selected track and slot, starts play and enables overdub.
* **Auto** - Toggle write clip launcher automation.
* **Lock** - Toggle write arranger automation.
* **Note Repeat** - Toggle Note repeat (when supported by Bitwig).

## Pad Modes

* **Fixed Vel** - If active, velocity of a played pad is always maximum.
* **Scene** - Press a pad to start one of the 16 scenes of the current bank page. Use Chords and Steps buttons to flip through the bank pages.
* **Pattern** - Press a pad to start one of 16 clips of the current bank page on the selected track. Use Chords and Steps buttons to flip through the bank pages.
* **Events** - Press a pad to select one of 16 devices of the current bank page on the selected track. Use Chords and Steps buttons to flip through the bank pages.
* **Variation** - Press a pad to select one of 16 parameter banks of the current bank page of the selected device. Use Chords and Steps buttons to flip through the bank pages.
* **Duplicate** - If active and a pad is pressed, you can duplicate a scene, track or clip depending on the mode (Scene, Select, Pattern)
* **Solo** - Press a pad to toggle Solo of 16 channels of the current bank page. Use Chords and Steps buttons to flip through the bank pages.
* **Select** - Press a pad to select one of 16 channels of the current bank page. Use Chords and Steps buttons to flip through the bank pages.
* **Mute** - Press a pad to toggle Mute of 16 channels of the current bank page. Use Chords and Steps buttons to flip through the bank pages.

* **Pad Mode** - Send notes in drum layout
* **Keyboard** - Send notes chromatic
* **Chords** - Switches notes 1 octave down
* **Step** - Switches notes 1 octave down
