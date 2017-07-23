# Bitwig Studio | Novation Launchpad Pro & MkII

Support script for Novation's Launchpad Pro controller. You can control track parameters, devices, transport, session view and play the pads.

## Differences MkII and Pro

The MkII misses the left column and the bottom row of buttons from the Launchpad Pro.
Most importantly it misses the **Shift** button. Therefore, the **Mixer** button acts as the **Shift** button.
If you press it also the grid changes. The left row of the grid now represents the missing left column of the Pro.
The second column represents the functions of those buttons in Shift state. 
Also the first row represents the missing buttons of the Pro. Alternatively, you can use the scene buttons to enter those modes (Volume, Pan, etc.).
The colors of the buttons are identical.


## Transport and Editing (Left button column)

Press _Mixer_ button and use the 1st and 2nd column of the grid on the MkII.

* **Shift** - Use in combination with other buttons for additional functionality.
* **Click** - Toggle the metronome 
* **Shift+Click** - Tap Tempo 
* **Undo** - Undo. Press Shift for Redo. 
* **Delete** - Like pressing the delete key. Hold the button for additional functionality in combination with other buttons knobs, see the view explanations below.
* **Quantise** - Quantises the selected clip.
* **Duplicate** - Always duplicates the first selected clip on the current track if pressed with no other button.
    * Launchpad Pro: Keep the Duplicate button pressed and select a clip in session mode to duplicate it
    * Launchpad Pro: Keep the Duplicate button pressed and select a pad from the 1st row when a track mode is on to duplicate the track.
* **Shift+Duplicate** - Toggle repeat 
* **Double** - Creates a new clip on the selected track and slot, starts play and enables overdub.
* **Shift+Double** - Start/Stop playback. Double click to move play cursor to start of song.
* **Record** - Start/Stop recording 
* **Shift+Record** - Toggle launcher overdub
* Press **Shift+Scene buttons** to set the preferred length for new clips.

## Cursors and Mode selection (Upper button row)

* **Arrows** - Navigate in the different modes (see below), holding an arrow button down will scroll through the specific View (e.g. track, scene).
* **Session** - Selects the Session mode to start, stop and record clips. Session can be flipped if Session button is pressed twice.
* **Note** - Selects the Note play mode for playing notes in different scales. If pressed again it activates the Drum mode for playing and sequencing drum instruments.
* **Shift+Note** - Activates the Sequencer mode. If pressed again it activates the Raindrop sequencer.
* **Device** - Selects the Device mode to change the Parameters of the currently selected device. If pressed again it opens the browser for preset selection mode. If no device is selected the browser is opened to insert a device.
* **Shift+Device** - Opens the device browser to add a device after the currently selected one
* **User** - Currently not used.

Note: The preferred play/sequencer mode is remembered for each track.


## Track Control (Lower button row)

These buttons only work in the Session mode. If the Session mode is not yet selected it gets activated.
On the MkII press _Mixer_ and use the 1st row of the grid or the scene buttons.

* **Record Arm** - The 8 buttons of the bottom row of the grid allow to toggle record arm of the currently focused 8 tracks of the track bank.
* **Track Select** - The 8 buttons of the bottom row of the grid allow to select one of the currently focused 8 tracks of the track bank. The currently selected track is indicated on the first row (round) buttons by a brighter white. Furthermore, the front LED is also lit in the color of the current track.
* **Mute** - The 8 buttons of the bottom row of the grid allow to toggle Mute of the currently focused 8 tracks of the track bank.
* **Solo** - The 8 buttons of the bottom row of the grid allow to toggle Solo of the currently focused 8 tracks of the track bank.
* **Volume** - Each column of the grid controls the Volume of the currently focused 8 tracks of the track bank. Hit buttons harder for faster change. The color of a fader is the same as the color of the track. Use the scene buttons for master volume.
* **Pan** - Each column of the grid controls the Panorama of the currently focused 8 tracks of the track bank. Hit buttons harder for faster change. The color of a fader is the same as the color of the track.
* **Sends** - Each column of the grid controls the Send of the currently focused 8 tracks of the track bank. Hit buttons harder for faster change. The color of a fader is the same as the color of the track. Use the Scene buttons to select the Sends 1 to 8.
* **Stop Clip** - The 8 buttons of the bottom row of the grid allow to stop the playing clip of the track of the currently focused 8 tracks of the track bank.
* **Shift+Stop Clip** - Stops all currently playing clips. (Mixer + 8th button of 2nd row on MkII)


## Session Mode

Press _"Session"_ to enter **Session** mode:

* The buttons on the grid start/record the clips. 
* The 8 scene buttons on the right start the scenes. 
* The arrow keys scroll the grid. Hold **Shift** to scroll in blocks of 8.
* Hold **Delete** and press a clip button to delete the clip.
* Launchpad Pro: For "birds eye view" press Shift


## Note Mode (Playing the pads)

Press _"Note"_ to enter **Play** mode:

* The key layout is the same one used with Ableton Push
* Left/Right buttons change the scale (Major, Minor, etc.)
* Up/Down buttons transpose the grid up/down.
* The upper 2 scene buttons change the key layout.
* The white scene button toggles between Chromatic and Scale Only  mode.
* The lower 2 scene buttons change the root note of the scale.
* The played keys are lighting red if global or clip recording (does not work if recording clip is outside of the monitored 8x8 matrix)
  

## Drum Sequencer Mode

Press _"Note"_ twice to enter the Drum Sequencer.

* The drum sequencer works as described in the Ableton Push manual.
* Hold *Delete* + Drumpad to delete the midi notes of the current clip on that 'pad'.
* To make the display of mute/solo/exists states work, the primary device needs to be the drum machine (which is normally the case).
* The Drumpads use the colors set in the drum machine for each pad.
  

## Sequencer Mode

Press _"Shift+Note"_ to enter the **Sequencer** mode:

* The pads display an 8x8 view of the selected clips note grid.
* The rows represent the notes of the selected scale.
* Use the arrow keys to navigate in the grid. 
* Note that you can scroll past the end of the clip (to the right).
* Press pads to enter/delete notes. 
* The velocity of the pressed key is set as well. 
* Use the Scene buttons to change the grids resolution.


## Raindrop sequencer

Press _"Shift+Note"_ twice to change to the Raindrop Sequencer:

* The lowest row displays the playable notes
* The row above a note starts a raindrop
* If the raindrop reaches the note it sounds

  
## Device Mode

Press _"Device"_ to enter the **Device** mode:

* Each column of the grid controls a parameter of the currently selected device. 
* These virtual faders use the same colors as the Bitwig highlight colors.
* Hit buttons harder for faster fader change.
* Cursor up/down to the next / previous device
* Cursor left/right to the next / previous parameter bank


## Browser Mode

Press _"Device"_ twice to enter the browser mode for preset selection. It will only enter the mode if a device is currently selected.
Press _"Shift+Device"_ to open the device browser to add a device after the currently selected one.

* The first 6 columns of the grid relate to the first 6 columns of the preset browser.
* The 8th column (yellow) relates to the result (preset or device) column of the browser.
* The 1st row moves the selection up by 1.
* The 2nd row moves the selection up by 8.
* The 3rd row moves the selection down by 8.
* The 4th row moves the selection down by 1.
* The red button dismisses the new preset or device selection and closes the browser.
* The green button confirms the new preset or device selection and closes the browser.
* The purple buttons are for previewing presets of instrument devices.
* Cursor left/right switches to the next / previous browser tab


## Preferences Dialog

You can set several preferences in the Preferences dialog of the script, which are stored when you exit Bitwig. 
Note that some of them are not available via the Launchpad Pro controller.
