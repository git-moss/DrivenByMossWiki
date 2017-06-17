# 5.01 (unreleased)
* New: Device and bank names are now shown on the screen when changed.
* Fixed: Could hang in Shift view.
* Fixed: Automatic lookup did not work on Linux.
* Fixed: Notes were duplicated in drum mode.

# 5.00
Requires Bitwig 2.1.
* New: Written now in Java
* New: Length setting for new clips
        
# 4.00
Requires Bitwig 2.0.
* New: Press Shift+Device twice to open the preset browser.
* Performance improvements

# 3.10
Requires Bitwig 1.3.15+
* New: Toggle in-key/chromatic with pad in Shift view (below the scale selection pads).

# 3.09
* New: Cursor left/right in Note and Drum Sequencer now change the page of the clip.
* New: Cursor up/down in Note, Drum and Raindrop Sequencer now change the note range.
* New: The two red buttons in the middle of the Shift view now allow to change the scale.

# 3.08
Requires Bitwig 1.3.15+
* New: Track scrolls into view when selected
* New: Quantize is now working as expected (but only on selected notes). Use the properties window to set the quantize amount.
* Fixed: Scales did not update in sequencers.

# 3.07
* New: Added new 8th centered scale layouts.
* New: Display on screen notification about grid resolution for all sequencers
* Fixed: Scrolling drum range did not scroll it in the Bitwig drum device
* Fixed: The arrow buttons in the Shift mode always move the tracks and scenes. Switched the movement of tracks and scenes to be identical with the grid layout.
* Fixed: Corrected some lighting issues with track and scene button states.

# 3.05
* New: Added Option: Select Clip on Launch
* New: Added Option: Behaviour on stop
* Fixed: Track bank was not adjusted when track selection was changed in Bitwig.

# 3.04
* Double clicking the *Play button* returns play cursor to zero.
* Changed notification text from 'Play' to 'Start/Stop'
* Fixed: Scale layout and chromatic mode could not be changed from properties dialog.
* Fixed: Bank range in grouped tracks behaves weird (requires Bitwig 1.3.8 RC 2+)

# 3.03
* Added options to configure layout in play view with scene buttons.
* Fixed: Important performance improvement (updates of button LEDs are only done when changed) which fixes external hardware sync.

# 3.01
Compatible with Bitwig 1.2/1.3.
* Fixed: Notes did not cover the full range (octave range extended).

# 3.00
Compatible with Bitwig 1.2.
* Shift+7th session button toggles VST window.
* Select next / previous device with the two green buttons on the left of the Shift-page.
* Select next / previous device parameter bank with the two orange buttons on the left of the Shift-page.
* Added notification message when switching between instrument/audio channels and effect channels.
* Fixed track navigation for effect tracks.
* Fixed octave up/down in sequencer mode.

# 2.3
* Streamlined and fixed behaviour of cursor buttons with and without Shift pressed (see updated documentation).
* Bugfix: Fixed display of note range in sequencer mode.

# 2.2
Compatible with Bitwig 1.1.6.
* Removed selection of clip with same index when changing tracks because of some nasty side effects.

# 2.11
Compatible with Bitwig 1.1.X.
* Currently playing measure in Drum- and Notesequencer is now drawn in green. Nonactive measures are now painted orange.
* Bugfix: Clip recording did not start when pad was pressed if Bitwig was not already playing.

# 2.1
Compatible with Bitwig 1.1.
* New sequencer: Raindrops
* Scale settings are now editable in the Preferences dialog.
* Preferences: Fader Ctrl, Soft Keys
* In Note and Drum Sequencer you can now change the loop.
* The selected base key for the scale is now marked green.
* Quantize button is working but only if clip is already focused in editor.
* Replaced tap tempo with new native function.
* Performance increase.
* On track change the clip at the same index as on the previous track is selected.
* Bugfix: Deactivate drum sequencer on audio track
* Bugfix: The scale base key could only be changed in play and sequencer mode.

# 2.0
Compatible with Bitwig 1.0.14.
* Added new Play mode with Scales.
* Added new Drum Sequencer mode.
* Added new Note Sequencer mode.
* Added Transport controls.
* Improved device lookup.
* Bugfix: Right upper pad not recognized.