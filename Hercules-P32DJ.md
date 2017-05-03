# Bitwig Studio | Hercules P32 DJ

Support script for the Hercules P32 DJ controller.

Get the latest stable release from: http://www.mossgrabers.de/Software/Bitwig/Bitwig.html

**The version in GitHub might always be in an alpha or beta state, you have been warned!**

There is also a tutorial video available: https://www.youtube.com/watch?v=NgEoxJ61OJM

## Features

The following functions are always the same in all modes.

* **Play (Right)** - Start/Stop playback. Double click to move play cursor to start of song.
* **Shift (Right)+Play (Right)** - Toggle repeat
* **Sync (Right)** - Toggle Automation Write
* **Shift (Right)+Sync (Right)** - Toggles the clip launcher automation write enabled state of the transport.
* **Cue (Right)** - Undo
* **Shift (Right)+Cue (Right)** - Redo
* **Browse** - Master Volume (fast)
* **Shift+Browse** - Master Volume (slow)
* **Loop (Left)** - Change tempo
* **Shift (Left)+Loop (Left)** - Change tempo fine
* **Loop Button (Left)** - Tap Tempo
* **Loop (Right)** - Move play cursor (fast)
* **Shift (Right)+Loop (Right)** - Move play cursor (slow)
* **Loop/Tempo Button (Right)** - Toggle metronome
* **Vol-/+** - Turn Headphone Volume Up or Down

To change modes keep the *Right Shift* button pressed and use the lit pads on the left deck.

## Mode 1: DJ Mode

**Important:** This mode requires a specific layout of the tracks and devices in a Bitwig project! Use the template project coming with the script named *DJMode-Template.bwproject*. Open the project and then choose *Save as Template...* from the *File* menu to store it as a template.

Keep the *Right Shift* button pressed and press the *first pad on the left deck* to enter that mode.

* **Crossfader** - Crossfade between A and B
* **Display Left** - Tempo (100 is displayed as a dot, >= 200 as two dots, e.g. 138 BPM = "3.8"; 231 BPM = "3.1.")
* **Display Right** - Displays the tempo fractions (e.g. 138.53 BPM displays "53")

### Deck Left/Right

For the *Shift* functions use the matching left or right Shift button depending if the knob/button whose function you want to trigger is on the left or right.

* **Load** - no function (should open the song browser but currently not possible)
* **3-Band EQ** - Low, Mid, High of EQ DJ (or 1st 3 parameters of any other device)
* **Record** - Turn on/off EQ of left deck
* **Slip** - Turn on/off EQ of right deck
* **Headphone** - Turn On/Off Headphone for Deck Left/Right
* **Volumefader** - Volume of track 1/8
* **Filter** - Cutoff of Filter device (device 1 of track 1/8)
* **Shift+Filter** - Resonance of Filter device (device 1 of track 1/8)
* **Filter Button** - Filter device On/Off (device 1 of track 1/8)
* **4 Knobs** - "Mix"-Parameter of device 2-4 on track 1/8
* **Shift+4 Knobs** - Volume of track 3-6/9-12 (the 4 sub-tracks)
* **4 On/Macro Btns** - Turn device 2-4 On/Off on track 1/8
* **Shift+4 On/Macro** - Mute track 3-6/9-12 (the 4 sub-tracks)
* **Pads (Sampler)** - Start clip
* **Shift (Left)+Pads (Sampler)** - Select scene range
* **Sync (Left)+Pads (Sampler)** - Stop clip playback on that track
* **Pads (Slicer)** - no function (will get functions when Bitwig API gets extensions for loop mangling)
* **Pads (Loop)** - no function (will get functions when Bitwig API gets extensions for loop mangling)
* **Pads (Hot Cue)** - no function (will get functions when Bitwig API gets extensions for loop mangling)
* **Cue (Left)** - no function
* **Play (Left)** - no function

## Mode 2: Mix Mode

Keep the *Right Shift* button pressed and press the *second pad on the left deck* to enter that mode.

* **Browse Button** - Open preset browser
* **Load** - A: Add instrument track, B: Insert device after the currently selected one
* **Shift+Load** - A: Add instrument track, B: Insert device before the currently selected one
* **3-Band EQ** - Send 3-8 (Low A = Send 3 ... High B = Send 8)
* **Record** - Start/Stop recording
* **Slip** - Toggle launcher overdub
* **Vol-/+** - No function
* **Headphone** - A: Solo selected track, B: Mute selected track
* **Volumefader** - A: Change Volume of selected track, B: Change Panorama of selected track
* **Filter** - Change Send 1/2 volume (fast)
* **Shift+Filter** - Change Send 1/2 volume (slow)
* **Filter Button** - Reset Send 1/2 volume
* **4 Knobs** - Change the Volume of track 1-4/5-8
* **Shift+4 Knobs** - Change the Panorama of track 1-4/5-8
* **4 On/Macro Btns** - De-/Activate track 1-4/5-8
* **Shift+4 On/Macro** - Toggle track monitor
* **Play (Left)** - Creates a new clip on the selected track and slot, starts play and enables overdub. Keep the button pressed and use the left SIZE/ADJUST knob to adjust the clip length.
* **Shift (Left)+Play (Left)** - Quantize active clip

### Sub Mode 1: Mix

Press left Sampler button to enter.

* **Pads**
    * 1st (top) row: Select track 1-4/5-8
    * 2nd row: Solo track 1-4/5-8
    * 3rd row: Mute track 1-4/5-8
    * 4th row: Rec Arm track 1-4/5-8
* **Shift (Left)+Pads** - Select track bank
* **Sync (Left)** - Open/close the window of the currently selected VST device (if any)
* **Cue (Left)** - Execute Duplicate

### Sub Mode 2: Drum Sequencer

Press left Slicer button to enter.

* **Pads** - Select and play the drum pad
* **Shift (Left)+Pads** - Turn on/off the steps of the selected pad/drum in the currently selected clip
* **Sync (Left)+Pads** - Only select the drum pad
* **Cue (Left)+Pads** - Left pad rows select the grid resolution. Right pads act as cursor keys: Octave up/down, clip left/right

### Sub Mode 3: Play

Press left Loop button to enter.

* **Pads** - Play the note depending on the current scale, base key and octave.
* **Shift (Left)+Pads**
    * 1st (top) row: Toggle In-Key/Chromatic
    * 2nd row: Scale down/up
    * 3rd row: Base key down/up
    * 4th row: Octave down/up
* **Sync (Left)** - Open/close the window of the currently selected VST device (if any)
* **Cue (Left)** - Execute Duplicate

### Sub Mode 4: Program Change

Press left Hotcue button to enter.

* **Pads** - Sends a program change.
* **Shift (Left)+Pads**
    * 1st (top) row (left): Select program range: 1-32, 33-64, 65-96, 97-128
    * Pads on the right: Send bank change 1-16
* **Sync (Left)** - Open/close the window of the currently selected VST device (if any)
* **Cue (Left)** - Execute Duplicate

### Sub Mode 5: Session

Press right Sampler button to enter.

* **Pads** - Start a clip.
* **Shift (Left)+Pads** - Move the 4x8 session rectangle.
* **Sync (Left)+Pads** - Stop clip playback on that track
* **Cue (Left)** - Execute Duplicate


## Mode 3: Device Mode

Keep the *Right Shift* button pressed and press the *third pad on the left deck* to enter that mode.

* **Browse Button** - Open preset browser
* **Load** - A: Add instrument track, B: Add audio track
* **3-Band EQ** - Send 3-8 (Low A = Send 3 ... High B = Send 8)
* **Record** - Start/Stop recording
* **Slip** - Toggle launcher overdub
* **Vol-/+** - No function
* **Headphone** - A: Solo selected track, B: Mute selected track
* **Volumefader** - A: Change Volume of selected track, B: Change Panorama of selected track
* **Filter** - Change Send 1/2 volume (fast)
* **Shift+Filter** - Change Send 1/2 volume (slow)
* **Filter Button** - Reset Send 1/2 volume
* **4 Knobs** - Change the value of parameter 1-4/5-8 of the current device
* **Shift+4 Knobs** - No function
* **4 On/Macro Btns** - Turn on/off devices 1-8
* **Shift+4 On/Macro** - No function
* **Play (Left)** - New: Creates a new clip on the selected track and slot, starts play and enables overdub.

### Sub Mode 1, 2, 3, 4 and 5

Same as in Mix mode.


## Mode 4: Browse Mode

Press the *browse button* in *Device Mode* to activate the *Browse Mode*. All functions are the same as in *Device Mode* except the following:

* **Browse Knob** - Select a new preset
* **Browse Button** - Accept new preset selection
* **Shift+Browse Button** - Discard new preset selection
* **Filter** - Left: Change selected Category, Right: Change selected Tag
