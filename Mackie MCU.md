# Bitwig Studio | Mackie MCU

Support script for the Mackie MCU protocol. While this extension supports the Mackie MCU protocol in general I could only test it with the following devices:
* icon QConPro X
* icon Platform M
* Zoom R16
The settings dialog contains profiles for several devices, which sets the correct hardware settings.

# Navigation

* **<<** (MCU REWIND) - Move the play cursor to the left.
* **>>** (MCU FORWARD) - Move the play cursor to the right.
* **Repeat** (MCU REPEAT) - Toggle repeat
* **Stop** (MCU STOP) - Stop playback. Press again to move play cursor to start of song.
* **Play** (MCU PLAY) - Start/Stop playback. Double click to move play cursor to start of song.
* **Record** (MCU RECORD) - Start/Stop recording
* **Shift+Record** - Toggles the launcher overdub.
* **Shift+Track selection buttons** - Select the length for new clips: 16 bars, 8 bars, 4 bars, 2 bars, 1 bar, 2 beats, 1 beat, 32 bars
* **Jog Wheel** - Move play cursor (press **Shift** for finer adjustment)
* **Scrub** - Toggles between Track and Device editing mode
* **Arrow left, right, up, down** - Like pressing the arrow keys on the computer keyboard
* **Zoom** - If active, the arrow buttons left/right zoom the arranger horizontally. The up/down arrows both toggle the height of the track.

# Buttons

## Display Mode
* **Display Mode** - Toggles the display of the track names in the 1st display.
* **Tempo/Ticks** - Toggle content of segment display. The last 3 digits toggle between ticks or the song tempo.

## Functions
* **Shift** (MCU SHIFT) - Use in combination with other buttons for additional functions.
* **Option** (MCU OPTION) - Use in combination with other buttons for additional functions.
* **Punch in** (MCU F6) - Toggle punch in
* **Punch out** (MCU F7) - Toggle punch in
* **F1-F5** (MCU F1-F5) - Functions for these buttons can be assigned in the settings dialog.

## Assignment
* **Track** (MCU MODE IO) - Select the Track edit mode. Press again to select the Volume edit mode. See the section **Edit Modes** below.
* **Pan** (MCU MODE PAN) - Select the Panorama edit mode. See the section **Edit Modes** below.
* **Send** (MCU MODE SENDS) - Select the Send edit mode. Press multiple times to select the Send channels 1 to 8. See the section **Edit Modes** below. Use in combination with the **Track select** buttons to select the respective Send channel 1-8.
* **Device** (MCU DEVICE) - Select the Device edit mode. See the section **Edit Modes** below.
* **Page Up** (MCU MODE EQ) - Move track bank focus 1 track up. If Device mode is active, the previous device parameter bank is selected.
* **Page Down** (MCU MODE DYN) - Move track bank focus 1 track down. If Device mode is active, the next device parameter bank is selected.

## Automation
* **Read/Off** (MCU READ) - Disables arranger automation recording.
* **Write** (MCU WRITE) - Enables arranger automation recording and sets it to Write mode.
* **Trim** (MCU TRIM) - Since Bitwig has not Trim mode, this button toggles the clip automation recording.
* **Touch** (MCU TOUCH) - Enables arranger automation recording and sets it to Touch mode.
* **Latch** (MCU LATCH) - Enables arranger automation recording and sets it to Latch mode.
* **Undo** (MCU UNDO) - Undos the last action
* **Shift+Undo** - Redos the last undone action

## Utilities

* **Note Editor** - Toggles the display of the note editor pane
* **Automation Editor** - Toggles the display of the automation editor pane
* **Toggle Device** - Toggles the display of the device pane
* **Shift+Toggle Device** - Toggles the display of a plugin window
* **Mixer** - Toggles the display of the mixer pane
* **Browser** (MCU USER) - Starts the browser to browse for presets
* **Shift+Browser** - Starts the browser to insert a new device before the current one
* **Option+Browser** - Starts the browser to insert a new device after the current one
* **Metronome** (MCU CLICK) - Toggle metronome
* **Shift + Metronome** - Enable Metronome Ticks
* **Groove** (MCU SOLO) - Dis-/Enable the Groove
* **OVR** (MCU REPLACE) - Toggle arranger overdub
* **Shift+OVR** - Toggle launcher overdub

## Fader Controls

* **Lock** - Locks the faders
* **Flip** (MCU_FLIP) - Toggles between Instrument/Audio/Hybrid tracks and the Effect tracks.
* **Cancel** (MCU CANCEL) - Cancels browsing when the Browser is active, otherwise like pressing the Escape key on the computer keyboard.
* **Enter** (MCU ENTER) - Confirms browsing when the Browser is active, otherwise like pressing the Enter key on the computer keyboard.
* **|<** (MCU BANK LEFT) - Move track bank focus 1 track up. If Device mode is active, the previous device parameter bank is selected.
* **>|** (MCU BANK RIGHT) - Move track bank focus 1 track down. If Device mode is active, the next device parameter bank is selected.
* **<< 8** (MCU TRACK LEFT) - Move track bank focus 8 tracks up. If Device mode is active, the previous device is selected.
* **8 >>** (MCU TRACK RIGHT) - Move track bank focus 8 tracks down. If Device mode is active, the next device is selected.


# Edit Modes

## Common functions in all modes

* **Record-arm buttons** (MCU ARM1-8) - Press to arm the specific track for recording.
* **Mute buttons** (MCU MUTE1-8) - Un-/mute the specific track
* **Solo buttons** (MCU SOLO1-8) - Un-/solo the specific track
* **Track selection buttons** (MCU SELECT1-8) - Select the specific track. Use in combination with the **Send** button to select the send channel 1-8. Use in combination with the **Shift** button to set the length of a new clip.
* **Shift+Solo** - Toggle auto monitor
* **Shift+Mute** - Toggle monitor
* **8 faders** (MCU FADER_TOUCH1-8) - Change volume of selected 8 tracks. Touching a fader automatically selects the track.
* **Master fader** (MCU FADER MASTER) - Change volume of master fader. Touching the fader selects the master track.
* **Press knob** (MCU VSELECT1-8) - Resets the current parameter to its default value.

## Track edit mode
* **8 knobs** - Change the volume, panorama, crossfader and Send 1-5 of the selected track. Hold **Shift** for fine adjustments.
* You can configure in the preferences that the crossfader option is hidden and you get 6 sends instead.

## Volume edit mode
* **8 knobs** - Change the volume of that channel. Hold **Shift** for fine adjustments.

## Panorama edit mode
* **8 knobs** - Change the panorama of that channel. Hold **Shift** for fine adjustments.

## Send 1 - 8 edit mode
* **8 knobs** - Change the volume of send of that channel. Hold **Shift** for fine adjustments.

## Devices edit mode

* **Device Knobs 1-8** - Change the currently selected 8 device parameters
* **|<** (MCU BANK LEFT) - If Device mode is active, the previous device parameter bank is selected.
* **>|** (MCU BANK RIGHT) - If Device mode is active, the next device parameter bank is selected.
* **<< 8** (MCU TRACK LEFT) - If Device mode is active, the previous device is selected.
* **8 >>** (MCU TRACK RIGHT) - If Device mode is active, the next device is selected.
* **Page Up** (MCU MODE EQ) - If Device mode is active, the previous device parameter bank is selected.
* **Page Down** (MCU MODE DYN) - If Device mode is active, the next device parameter bank is selected.

## Browser

* Press the _Browser_ button to start
* Navigate columns with the _Track Control knobs_.
* Click the knobs to enter a filter or the results. Click again to confirm.
* To confirm a patch or device selection and close the Browser press the _Enter_ button.
* To discard the patch selection press the _Cancel_ button.

# Foot switches

* **Footswitch 1** (MCU USER A) - Function be assigned in the settings dialog.
* **Footswitch 2** (MCU USER A) - Function be assigned in the settings dialog.

# Preferences dialog

* Set preferences for Device capabilities, etc.
