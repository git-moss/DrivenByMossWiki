# 5.13
Requires Bitwig 2.3.
* Fixed: The "Behaviour on Stop" setting was not respected when using the Stop button (only with the Play button).

# 5.12
Requires Bitwig 2.3.
* New: Shift + Dev. Lock pins now also the cursor track because only pinning the device does not work.

# 5.11
Requires Bitwig 2.2.
* New: Shift + Dev. Lock pins the cursor device.

# 5.10
Requires Bitwig 2.2.
* New: Display the view names when switching between them.

# 5.02
Requires Bitwig 2.1.
* New: In sequencer and drum mode the loop selection buttons represent now one page (not a measure as before). Pressing one of the pads selects the page. To set a "one pad" loop press the pad again.

# 5.00
Requires Bitwig Studio 2.1.
* New: Written now in Java.
* New: Added scale layout setting.
* New: Press Shift and move Volume Fader to move the fader to the current value of the matching track. On the screen you get information if you need to move it up or down.
* New: The scene buttons are now colored in green in Session mode.
* Fixed: MkII: Layer navigation did not work

# 4.00
Requires Bitwig 2.0.
* Fixed: Shift+Track had new clip lengths in wrong order
* New: Shift+Track lights the selected clip length
* New: SendA+Track lights the selected Send
* New: Onscreen display of selected Send
* New: If you press Shift, there are new functions if you press the pads of the first row:
    * Add instrument track
    * Add audio track
    * Add effect track
    * Add device before
    * Add device after
    * Undo
    * Redo
* Performance improvements

# 3.08
Requires Bitwig 1.3.15+
* New: Track scrolls into view when selected
* New: Use different colors for note starts and lengths in note and drum sequencer.
* New: Quantize is now working as expected (but only on selected notes). Use the properties window to set the quantize amount.
* Fixed: Scales did not update in sequencers.

# 3.07
* New: Display on screen notification about grid resolution for all sequencers
* New: Added measures to 1st row of sequencer mode
* Fixed: Scrolling drum range did not scroll it in the Bitwig drum device

# 3.06
* New (MkII): Octave pads in play, sequencer and raindrop view are now colored in the tracks color.
* New: Added Option: Select Clip on Launch
* New: Added Option: Behaviour on stop
* Fixed: Track bank was not adjusted when track selection was changed in Bitwig.

# 3.05
* Shift + Session: Enable automation write in clip launcher
* Fixed: Bank range in grouped tracks behaves weird (requires Bitwig 1.3.8 RC 2+)

# 3.03
* Fixed: Important performance improvement (updates of button LEDs are only done when changed) which fixes external hardware sync.

# 3.02
* You can now select the root note of the scale. Press **Shift** and use the first two row buttons (arranged like a keyboard).
* Fixed lag of script especially in combination with other scripts like Push4Bitwig due to very slow processing of LED button updates. The button states are now cached and only updated when changed.

# 3.01
Compatible with Bitwig 1.2/1.3.
* Shift+Device On/Off toggles editing of device parameters and macros.
* Fixed: Notes did not cover the full range (octave range extended).
* Fixed: Display of the note range was wrong.

# 3.00
Compatible with Bitwig 1.2.
* Support for Browser, press Bank button and then navigate columns with the knobs.
* Switch between Chromatic and In-Key in Play-, Sequencer- and Raindrop-Mode with the middle Session button. Also as a setting in the preferences.
* Shift + Metronome: Enable Metronome Ticks
* Shift + Detail View: Toggle VST window
* Bugfix: Fixed display of note range in sequencer mode.
* Bugfix: Fixed track navigation for effect tracks.

# 2.2
Compatible with Bitwig 1.1.6.
* Drumpads now use the colors set in the drum machine.
* On track bank change the 1st channel of the bank is selected.
* Removed selection of clip with same index when changing tracks because of some nasty side effects.

# 2.11
Compatible with Bitwig 1.1.x.
* On the MkII you can now navigate the device layers. Use Shift+Device Left/Right.
* Bugfix: Currently playing measure in Drumsequencer is now drawn in green.
* Bugfix: Two green colors had the same value on the MkII.

# 2.1
Compatible with Bitwig 1.1.
* Implemented A|B buttons (on first version press Shift+RecArm) and crossfader.
* Toggle monitor and auto monitor: Shift+Mute, Shift+Solo
* Scale settings are now editable in the Preferences dialog.
* In Drum Sequencer you can now change the loop.
* The selected mode is now indicated in green.
* Quantize button is working but only if clip is already focused in editor.
* Replaced tap tempo with new native function.
* Performance increase.
* Replaced tap tempo with new native function.
* New sequencer: Raindrops
* Switching tracks remembers the last selected view (play, drum, sequencer). Also a clip on that track will be selected.
* On track change the clip at the same index as on the previous track is selected.
* Bugfix: Deactivate drum sequencer on audio track

# 2.0
Compatible with Bitwig 1.0.14.
* Added new Play mode with Scales.
* Added new Drum Sequencer mode.
* Added new Note Sequencer mode.
* Improved device lookup.
