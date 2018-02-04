# 10.0 (unreleased)
Requires Bitwig 2.??.
* New: Drawing of Push 2 display is now fully integrated. No external application is needed anymore.
* New: Devices display an icon
* New: Clip mode has the option to display a piano roll.
* New: The new session mode can display the names of scenes and clips.
* New: The last selected mix mode (track, volume, pan , ...) is remembered.

#9.40 (unreleased)
* New: Support for pinning tracks and devices
* New: Harmonized track navigation with master track. Pressing the button below the master track will move into the master tracks' devices. Going up from devices selects the master track.
* New: Slowed down scrolling of crossfader assignment and scale knob.
* New: When no device or layer is selected the button to go up to the tracks is still displayed.
* Fixed: Grid notes were not updated when switched to effect or master track.

#9.31
* Fixed: Add Device button did not work (regression in 9.30).
* Fixed: Modifying values of the 2nd page of a drum pad layers did modify the values of the 1st page.
* Fixed: Drumpads did not produce sound after a button combination with delete, mute, solo or select was used.
* Fixed: Loop length in clip mode was also offset by 1 but should not.

#9.30
* New: Slowed down scrolling of browser columns and presets.
* New: The values of the last touched browser column can now be changed with the tempo knob for finer adjustments.
* New: Improved visibility of selected browser column filters.
* New: If the browser is closed in Bitwig, the last active mode is set on the Push.
* Fixed: Resetting a browser column did crash the extension.

#9.25
* Fixed: The time values displayed in clip mode were 0 based instead of 1 as displayed in Bitwig.
* New: The change speed of play start, end, loop start, length in Clip Mode are slowed down.

#9.24
* Fixed: Drawing of scene birds eye view was not correct if scene/track numbers were not a multiple of 8.
* Fixed: Push 1: Non-ASCII characters in track names did not work

#9.23
Requires Bitwig 2.1.
* New: Setting for a preferred note view to use for new tracks.
* New: Prevent flickering when accidently touching the tempo or position knob while tweaking one of the other 8 knobs.

# 9.22
Requires Bitwig 2.1.
* New: The devices and track views use the 8th button above the display (2nd row on Push 1) for navigating up in the hierarchy.
* New: Devices view contains a new "Banks" toggle button to toggle between banks and devices. This is especially useful for instruments which contain layers (incl. Multiout VSTs).
* New: Changed Whole-half and added Half-whole scale.

# 9.21
Requires Bitwig 2.1.
* New: Scenes can be started from Play and Piano view.
* New: Push 2: The last selected mix mode is remembered when switching back from other modes.
* New: Push 2: Long pressing the Stop Clip button does indicate if a track has a playing clip by coloring the track buttons red.
* Fixed: When in note mode hold the session button to engage the momentary function didn't work anymore.
* Fixed: Push2Display did not store several color settings
* Fixed: Info knob in setup mode was switched with 2nd button row.
* Fixed: Locrian scale contained a wrong note.
* Fixed: Switched variants of Hirojoshi, Pelog scale.
* Fixed: Display of some scales in chromatic mode were wrong (e.g. Diminished, Whole-Half, Whole Tone)
* Fixed: Push 1: Send mode did not work
* Fixed: Push1: Length of value display was too long

# 9.20
Requires Bitwig 2.1.
* New: In sequencer and drum mode the loop selection buttons represent now one page (not a measure as before). Pressing one of the pads selects the page. To set a "one pad" loop press the pad again.

# 9.10
Requires Bitwig 2.1.
* New: When in Session view and press Session again a menu turns up (like in note view) where you can select different views. The normal Sesson view, the flipped version and a new Scene view. This view displays the first 64 scenes ready for jamming. The color of a scene uses the color of the first clip found in the scene (only checks in the first 8 tracks). Use the Layout button on Push 2 to quickly step through these views.
* New: Changed the layout of the Drum 64 view to match the normal Drum view.
* New: The Fixed Length menu contains a new row with options which allows to create a new clip without storing the length.
* New: Added more function options to the Footswitch 2.
* New: You can use the Delete button in combination with a pad in Play mode. But note that this can be dangerous since the notes you see might not come from the currently selected clip!
* New: If Browse is pressed and no device is currently selected, add device is called.
* New: The Duplicate button (with no other button pressed) now always duplicates the first selected clip on the current track.
* Fixed: When using the "use parent color" color the pads were not colored at all in session mode.
* Fixed: Aftertouch was not working in Piano mode.
* Fixed: Mastermode was not activated when Master volume knob was touched
* Fixed: Holding Record and selecting a track could only arm 1 track. After that the record button had to be released and pressed again.
* Fixed: 64 Drum mode: Sounds did not play when octave was transposed.

# 9.00
Requires Bitwig 2.1.
* New: Written now in Java
* New: **Black** keys in Piano mode are now using the track color.
* New: Setting to turn off to display clips of record enabled tracks in red
* New: Setting to lock the session orientation
* New: Setting to choose an action for pressing rec armed empty clip in Session mode
* New: Layout button steps through the play or sequencer modes (depending on which type is active). Shift+Layout button toggles between play and sequencer modes
* New: All drum modes are now accessible from the track input selection menu (when Note button is pressed)
* New: To rec arm a track, keep the record button pressed and select the channel (first button row).
* New: To navigate groups, layers and devices press now the respective first row button. Long press any of the first row buttons to move up the hierarchy again.
* New: To navigate in a clip use now the Page left/right (device in/out on Push 1) buttons.
* New: New clip length is now stored in a setting
* New: Scene lights are now off if the scene does not exist
* New: Flipping the session view does no longer swap the scene and the 2nd row buttons, since this does not make much sense on the Push 2.
* New: The cursor keys now consistently always change the track (device, layers) and scene bank, except in browser they change the browser tabs.
* New: Removed direct parameters because they cause more problems than they help. Use Remote control parameters instead.
* Fixed: Implemented a workaround for the always empty Groove parameter names.
* Fixed: Changing the Metronome volume was not working, change now with Select+Knob 9.
* Fixed: Long pressing Automation did not bring up the automation selection when arranger/clip record was toggled.

# 8.10
* New: Session mode: Press "Stop Clip" + any pad on a track to stop the currently playing clip on that track.
* New: Stop Clip + Track is now also working when not in Session mode. Furthermore, you can use the 1st or 2nd-row buttons.
* New: Option in Settings to turn off empty drum sequencer pads (otherwise orange).
* New: Groove display can be left by pressing the Quantize button again.
* New: Flipping arrange and clip record now also flips automation.
* New: Performance improvements
* Fixed: Select+Pad and Delete+Pad was not working in 64 drum mode.

# 8.00
Requires Bitwig 2.0.
* New: New track details mode with option to set track color (keep Select pressed)
* New: New layer details mode with option to set layer/drum pad color (keep Select pressed)
* New: Clip mode
    * Keep Delete pressed and touch 8th knob to reset the accent.
    * You can set the clip color
* New: Basic version of 64 pad drum view (enter drum mode, keep Shift pressed and then press 4th scene button).
* New: Press "Add Device" to add a device after the currently selected one
* New: Press Shift+"Add Device" to add a device before the currently selected one
* New: Browser
    * Press Shift+Browse to cancel browsing
    * Rearrangement of browser layout
    * New: The browser filter columns can be hidden in the settings
    * New: Press Delete + touch knob to reset filter
    * New: Change the tabs of the browser with the left/right cursor buttons (especially useful with the Sampler)
    * New: Hold *Browse* and select a pad in Session mode to browse for clips
* New: Push 2: Modulation of parameter values is now displayed (Push2Display updated to support this)
* New: Preference to reverse the behaviour of the record and overdub functions
* Fixed: Scrolling with cursor keys could lead to endless scrolling
* Fixed: On Screen parameter notification for empty parameter (displayed ":")

# 7.42
Requires Bitwig 1.3.15+
* New: Added button to master mode to turn on/off audio engine.
* New: Adding a track now selects it.
* New: Shift+Duplicate to create a new scene from the currently playing clips
* New: Shift+New: Like New button but without activating launcher overdub.
* Fixed: Changing the Send on Push 1 did show the notification string in the display.
* Fixed: Octave up/down in raindrop sequencer did switch track but should change octave.
* Fixed: Switching between Mute and Solo mode did not work on Push 1 in Drum sequencer.

# 7.41
* New: Smoother value updates
* Fixed: Added missing knob labels in Master mode (Push 2)
* Fixed: Changing discrete direct parameters works again

# 7.40
Requires Bitwig 1.3.15+
* New: Duplicate+Track-Select duplicates track
* New: Duplicate+Clip duplicates the clip
* New: Double/Double Loop: Duplicate the content of the currently selected clip
* New: Track scrolls into view when selected
* New: Support for record arm on master track
* New: Switch to the next/previous opened project (operate from the Master mode)
* New: Added transpose feature for Sequencer, Raindrops and Session view (use Shift+Octave Up/Down). Select+Octave transposes in 12 steps.
* New: Use different colors for note starts and lengths in note and drum sequencer.
* New: Delete+Pad in drum sequencer now deletes all notes on that note not only 32 bars.
* New: Quantize is now working as expected. Use Shift+Quantize to set the quantize amount. This menu can now also be opened by long pressing the Quantize button.
* New: Coloured record button when Shift is pressed (for launcher overdub).
* Fixed: Scale not updated in sequencers when changed.
* Fixed: Accent mode not working in raindrop sequencer.

# 7.34
* New: 2 new drum modes. Press Shift in drum mode and use upper 3 scene buttons to change modes. 2nd mode displays 4 drum sound, 3rd mode 8. Use the lower 4 scene buttons in 2nd mode to toggle between the drum sounds 1-4, 5-8, 9-12, 13-16. Use the lower 2 scene buttons in 3rd mode to toggle the drum sounds 1-8, 9-16.
* New: Added new scale layout "8th centered". Moved the layout orientation into a separate button.
* New: Display on screen notification about grid resolution for all sequencers.
* New: Slight change of the ribbon configuration layout.
* Fixed: Mute/Solo+Pad in Drum sequencer did also mute/solo the whole track.
* Fixed: 16 pads (the ones from the drum mode) sent notes in Session mode.
* Fixed: Change of FX track group was not reflected on controller.
* Fixed: Octave up/down button turns now off when the end of notes is reached.
* Fixed: Poly aftertouch error when note was out of range.
* Fixed: Fixed drum notes not sounding when pads are muted or soloed.
* Push 2:
    * Fixed: Ribbon LEDs for crossfader in session mode were not displayed correctly.
    * Fixed: Notifications were not shown on the display (e.g. note ranges)

# 7.33
* Fixed: Keeping Session button pressed did not return to previous play view.

# 7.32
* New: Octave pads in play, sequencer and raindrop view are now colored in the tracks color.
* New: Added Option: Select Clip on Launch
* New: Added Option: Stop Automation on knob release
* Fixed: Touchstrip LEDs were not set correctly
* Push 2:
    * Push2Display: Restore window position at startup.
    * Push2Display: Show warning message if configuration file could not be stored.

# 7.31
* New: Overview navigation for session. Keep Shift button pressed in Session mode.
* New: Added new option to Play button behaviour: **Pause** behaves like the Space bar.
* Fixed poly aftertouch not working with Push 2.
* Fixed ribbon LEDs on Push 2 when in CC or Fader mode.
* Fixed: Bank range in grouped tracks behaves weird (requires Bitwig 1.3.8 RC 2+)

# 7.30
* Push 1/2:
    * New Workflowsetting: Auto-Select drum channel (Off, Channel)
    * Changed Automation Override button combination from Select + Automation to Delete + Automation.
    * Improved workaround for quantize function.
    * Fixed: Important performance improvement (updates of button LEDs are only done when changed) which fixes external hardware sync.
    * Fixed: Pressing Delete+Pad did also start play or record
    * Fixed: 8th button of first row was not turned off on shutdown
    * Fixed: New clip creation for 1 and 2 Beat length.
    * Fixed lighting of some buttons
* Push 2:
    * New: Press Convert button to bring up the Slice to Drum Machine dialog.
    * New: Press Shift+Convert button to bring up the Slice to Multisample dialog.
    * Activate Poly Aftertouch on startup.
    * Added version number to Push2Display.
* Push 1:
    * Fixed: Displayed was not cleared on shutdown

# 7.22
* Improved device navigation:
    * If no device is selected (e.g. no device on the track) and *Device Out* is pressed the view is switched to the current track.
    * If *Device In* is pressed in a track/mix mode and it is not a group the view is switched to device mode.
    * If *Device Out* is pressed on a top level device the view is switched to track mode.
    * If *Device In* is pressed on a multi-output VST plugin but no output layers were created the parameters are shown instead of an error that there are no layers.
* NOTE: There is currently a bug in Bitwig which crashes Bitwig Studio if you switch from layers to devices under certain circumstances!

# 7.21
* Fixed: Script did crash on Linux when a song was closed. Workaround for a Bitwig bug.

# 7.20
* Push 1
    * New: Added Firmware version information to configuration mode (long press User button)
* Push 2
    * New: Added Setup mode. Allows to set the display brightness, LED brightness and the response of the pads. Press Setup button
    * New: Added Info mode. Displays the Firmware version, build revision and serial number of the device.
    * Fixed: Device layers could not be displayed if no send existed

# 7.11
* Push 2:
    * Improved: USB lookup of device
    * Fixed: Menu display for devices: On-State was not set, Window menu was missing for VSTs.

# 7.10
* Push 1/2:
    * New: Implemented Volume, Pan and Sends modes for the layers view. 
        * Push 1: Use **Select+Volume/Pan/Track** buttons to activate. For Sendmodes press **Pan** multiple times.
        * Push 2: Use the menu buttons above the display to activate.
    * Improved: If no device is selected the primary device of the current channel (if any) is used. This prevents that you have to manually select a device with the mouse.
    * Improved: Deactivated **Add Effect** button since the function is currently not working and just confused users (requires API fix)
* Push 2:
    * Improved: Deactivated LED on unused buttons Convert and Setup
    * Fixed: Script did crash when non-ASCII characters were used in names
    * Fixed: In Track view soloing the selected track also soloed the mastertrack
    * Fixed: Sends were not displayed in Track View for the last channel when tracks were less than 8
    * Fixed: Menu for long press Mute/Solo was not displayed in Sendviews
    
# 7.00
* Push 1 & 2
    * New: Added Mute, Solo and Auto Monitor buttons to Master track (use 2nd row buttons like with normal tracks).
    * New: The flip mode of the session view is now be stored as a setting
    * New: In device mode the buttons next to ON/OFF device are now device, fixed, direct and expand,macro,parameters like when pressing the device button twice.
    * Improved: Drum Pads no longer sound when used in combination with Delete, Mute or Solo buttons.
    * Improved: Button redrawing on track change (removed flickering)
    * Improved: Better readability in Browser mode
    * Improved: Display of Groove mode
    * Fixed: Unused knobs in Groove mode were not deactivated and produced errors
    * Fixed: Select indication of Device, Volume, Track, Pan and Clip did not work all the time
    * Fixed: Marker enablement in Panel selection view.
    * Fixed: Midi CC 127 could not be selected for ribbon.
    * Fixed: Error when CC for ribbon was selected and the ribbon was not yet used
    * Fixed: CC area of ribbon was not working in PB/CC mode
* Push 2
    * New: Implemented graphical support for the display
    * New: Lock Solo/Mute (behaviour like Push 1): Shift+Solo/Mute
    * Improved: Push2Display: Correct default path for Bitwig Studio depending on OS
    * Fixed: Push2Display: Start of Bitwig Studio did not work on Mac
    * Fixed: Light intensity on monochrome buttons

# 6.00
* Initial support for the Push 2 hardware. Note the necessary installation instructions for the Push 2!

# 5.02
* New view for editing the loop of a clip. This is the default view for audio tracks.
* Fixed: Scaling of knobs did not work in combination with Shift.
* Fixed: Setting of positive values for Clip Shuffle Accent.
* Fixed: Enable of groove did not work
* Fixed: Endless selection of different tracks when left/right buttons were quickly pushed
* Fixed: Group navigation in clip mode was not working.
* Fixed: Stepping out of device hierarchy required an unnecessary additional button push. Furthermore, the layer in the Bitwig UI was shown one step too late.
* Fixed: Device Layer mode was not restored when temporarily left (e.g. to tempo)
* Fixed: Display of note range names was broken in Play and Sequencer view.
* Fixed: Doublick on Playbutton to rewind did not work when playback was stopped.
* Fixed: Confirming / Cancelling of browser was missing. Press now Browse again to Confirm or Select+Browse to Cancel.
* Fixed: Crossfader B could not be selected in Crossfader mode

# 5.01
* Fine (Shift pressed) changed from 0.5 to 0.25
* Fixed: Changing direct parameters works again (still broken non continuous parameters).
* Fixed: Crossfader B could not be selected
* Fixed: No more flickering of 2nd row buttons in Device mode.
* Fixed: If _Fader_ mode was selected the ribbon lights were not updated if the volume of the track changed. Furthermore, if VUs were enabled they were also not reflected on the ribbon.
* Fixed: The crossfader value was not updated on the ribbon in Session mode.
* Fixed: Notes did not cover the full range (octave range extended).
* Fixed: Prevented midi error with VUs if track is clipping

# 5.0
Compatible with Bitwig 1.2.
* Support for groups
* Support for new browser
* Window open/close button in device modes is now only lit when it is an external plugin
* Press Delete + Pad In Session Mode to delete the clip
* Reordered the selectable views (when you press 'Note')
* New program change view: Press "Note" -> "PrgChang"; Pads send program change; Scene buttons switch banks; Pressing scene button twice toggles 0-63 and 64-127.
* Select+Play      : Toggle Punch In
* Select+Shift+Play: Toggle Punch Out
* Added Volume Fader Control of current track as a ribbon option.
* Activated ribbon for all views.
* When switching plugins the selected device mode is remembered, also available as a setting
* Several options for Footswitch 2 in the settings:
    * Toggle Play
    * Toggle Record
    * Stop All Clips
    * Toggle Clip Overdub
    * Undo
    * Tap Tempo
    * New Button
    * Clip Based Looper:
        - If there is no clip in the selected slot, pressing the foot pedal creates a clip and begins Overdub mode. Releasing it ends Overdub mode.
        - If there is a clip in the selected slot, pressing the foot pedal enables Overdub. Releasing it turn Overdub off.

* Touching a parameter knob now displays an on screen notification
* Deactivated the knobs above the tempo and play position values in navigation mode to prevent accidental changes while using the small knobs
* Implemented Sends for Instrument layers.
* Fixed: Automation Touch Mode was not working.
* Fixed: Creation of new clips in other time signatures than 4/4 was broken
* Fixed: Resetting of parameters in device layers and drum pads did not work
* Fixed: Parameter Bank "Fixed" was not selected when a different mode than "Common" was selected
* Fixed: Displayed 1 octave too low when changing octaves up/down.

# 4.4
Compatible with Bitwig 1.1.8.
* New play mode 'Piano' with keyboard like layout
* New scale offsets by 8ths
* Added new settings option to convert the Poly Aftertouch of the pads to Channel Aftertouch or a CC.
* Bugfix: Fixed track navigation for effect tracks.
* Bugfix: Fixed behaviour of Master button: Does no longer select master button if long pressed to enter frames mode. Previous mode gets correctly restored if pressed again.
* Bugfix: Fixed position of note range display in Play mode.

# 4.3
Compatible with Bitwig 1.1.6.
* Drumpads now use the colors set in the drum machine.
* Pressing SELECT and a drum pad now also selects the device drum channel in the display.
* Added possibility to toggle between Devices and Parameter-Pages with Shift+DeviceIn for multi output VST plugins.
* Mute/Solo + Drumpad does mute/solo the drumpad.
* Several improvements/fixes with drum pad and layer navigation.
* On track bank change the 1st channel of the bank is selected.
* Adapted monitoring of VST direct parameters to work with 1.1.5 API.
* Removed selection of clip with same index when changing tracks because of some nasty side effects.
* Fixed lighting of right arrow for track navigation
* Fixed that all LEDS turn green after adding an Instrument via drag and drop into the arrangement view.

# 4.2
* New preference setting to return to zero when stop is pressed.
* New preference setting to display (or not) the crossfader parameter in the track.
* Bugfix: Clip recording did not start when pad was pressed if Bitwig was not already playing.
* Bugfix: When switching the ribbon from Pitchbend to CC the ribbon lights were not initialised correctly.
* Bugfix: Two green colors had the same value on the Push.

# 4.1
Compatible with Bitwig 1.1.2.
* Completely rewrote bank selection and navigation of devices (Ableton style)
* Rewrote device selection (Ableton style) but has some open issues due to API limitations:
     * Devices are not correctly selected on the display if are duplicates with the same name
     * Direct parameters might get screwed
     * Devices in a layer are not displayed with names (there are always 8 dummy names)
* Drum pads in drum view now show mute/solo and active/exists states. To make this work the primary device needs to be the drum machine (which is normally the case).
* Rewrote patch selection mode which makes use of the touch capability of the value buttons.
* Long press User button to adjust the pad sensitivity. Also configurable in the script settings.
* Frame mode (keep Master pressed) now follows selected panel layout and has additional options.
* Shift+Browse toggles Browser. Toggling Inspector is now available in Frame mode. Pressing Browse now always enters preset selection.
* Select+Shift+1st button row to de-/activate a track
* 1st button on 2nd row in device modes dis-/enables device. Except in Macro mode.
* 8th button on 2nd row in device modes displays VST window. Except in Macro mode.
* In flipped Session mode the 2nd button row controls now the Scene starts (before it was the 1st). In that mode the Scene buttons now always control Mute or Solo.
* Currently playing measure in Drum- and Note sequencer is now drawn in green.
* Added 2nd mixed mode to Ribbon: Pitch/CC
* Long press Automation button to bring up the Automation dialog which allows you to change the automation mode.
* If the tempo or play position knobs are touched their values are displayed (and can also be changed with the knobs above them).
* Bugfix: Lighting of Automation button is now working as expected
* Bugfix: Mapping of macros is now only possible in Macro mode
* Bugfix: Reset of crossfader setting not working (Delete + Touch)
* Bugfix: Device parameter bank selection: 8th button was active but has no functionality.

# 4.0
Compatible with Bitwig 1.1.
* Performance increase.
* To change the play views press note and select one from the display.
* New sequencer: Raindrops
* Toggle monitor and auto monitor: Keep pressed Select in Volume, Pan or Track mode. First row toggles Monitor, second row Auto Monitor.
* Added display of note range when changing octaves in drum sequencer.
* Added display of note range when changing octaves in note sequencer.
* Note range in note sequencer can now also be changed with the octave up/down buttons.
* Polyphonic Aftertouch of Pads in Play mode is now sent to Bitwig
* Frame mode (long press Master) allows now to change Arranger and Mixer settings. Also the layout states are now displayed.
* Shift+Browse toggles Inspector.
* Quantize button is working but only if clip is already focused in editor.
* Replaced tap tempo with new native function.
* Add Track: Adds a new instrument track
* Shift+Add Track: Adds a new effect track
* Select+Add Track: Adds a new audio track
* Ribbon, Accent and Scale settings are now editable in the Preferences dialog.
* The LEDs of the ribbon are now used depending on the selected ribbon mode
* Added crossfade mode (press Volume twice)
* Added crossfade parameter to track mode. Removed 1 send channel.
* In Session mode the ribbon controls the crossfader.
* In Note and Drum Sequencer you can now change the loop.
* Press Clip to modify clip properties (loop, play, etc.)
* Hold Delete and Touch Encoder to reset value works now in all device modes.
* Hold Delete and Touch Encoder to reset value in Volume, Pan, Send and Track modes.
* Switching tracks remembers the last selected view (play, drum, sequencer). Also a clip on that track will be selected.
* Fixed and improved parameter page selection and display.
* The Fixed Length selection is now activated with a normal button press. No long press required.
* Preset browser: Display of the next 3 presets. Hold Shift + control buttons to move quickly through the presets and categories.
* On track change the clip at the same index as on the previous track is selected.
* Added [Shift + Metronome] to toggle metronome ticks.
* Added [Shift + Automation] Toggles the clip launcher automation write enabled state of the transport.
* Added [Select + Automation] Resets any automation overrides.
* Added [Delete + Encoder0, Encoder1 touch]  MasterMode reset volume, pan.
* Added [Delete + Encoder9] reset Master track volume in any mode. 
* Bugfix: Device mode buttons did not work when in Session view.
* Added [Shift + Ribbon] to center the crossfader.
* Switched functionality of Duplicate and Double buttons
* Bugfix: Enabled state of Groove had to be pressed twice.
* BugFix: Accent toggle was reversed.

# 3.33
Compatible with Bitwig 1.0.14.
* Shift+Small Knob 1: Fine adjust tempo
* Bugfix: Added missing implementation of light states of cursors in Play mode.
* Bugfix: Corrected colors of rec armed tracks and clip states in Session mode.
* Bugfix: Corrected colors of Solo buttons.

# 3.30
* Press Track button twice to toggle between editing of normal tracks and effect tracks. To toggle VUs press now Shift+Track.
* Playing sequencer notes are now reflected on the Play and Drum grid.
* The names of the Send tracks are now displayed.
* Non existing track columns are now fully blank.
* Pan & Send button only steps through existing sends tracks.
* Hold Select + Drum Rack pad to select its notes without triggering the pad (Drum View)
* Hold Delete + Drum Rack pad to delete the midi notes of the current clip on that 'pad'.
* 8 track window now scrolls to the newly selected track (selected in Bitwig).
* Memory savings due to change from inline functions to class functions.
* Bugfix: Hold the delete key and touch a knob to reset its value in Device Mode was broken.

# 3.20
* Hold Session while in Note mode to switch temporarily to Session mode
* Knobs change values now by how fast you turn them.
* If no track is selected a text is now displayed.
* Decreased refresh rate of display. Improves responsiveness.
* Bugfix: Frame and Device mode had incorrect button colors due to last color refactor.
* Bugfix: Master Knob temporary mode behavior not returning to all previous modes.
* Bugfix: Full maximum value range of knobs might not have been reached.

# 3.10
* Press Shift+Touchstrip to change its behaviour
* Added dis-/enabling Modulation Sources (Device -> Modulate)
* If the master volume button is touched the master menu is temporarily displayed.
* Flipping Session also flips the rec-enable and scene start buttons
* Return to arrangement is on 2nd row (was on 1st) to be consistent with flipped mode
* Stop is also on 2nd row (was on 1st) to be consistent with flipped mode
* Holding down Arrow buttons in all Views now scroll the specific view.
* Added [Shift + Encoder] for fine value adjustments.
* Device mode displays page name
* Bugfix: "Pan&Send" needed to be pressed twice to switch from Pan to Send1.
* Ableton Live workflow with track selection, record arm, and mute/solo functions.
  * Mute/Solo buttons now toggle 2nd row mute/solo state,
  * Single press of a first row button selects the track, another press on the selected track arms for recording, another press disarms track.
  * The non selected armed tracks will be dim red while the selected armed track will be bright red.
  * The selected track unarmed will be dim yellow and the selected track will be bright orange.

# 3.00
* Sequencer Mode now uses Scales.
* Press Device twice to select editing of device parameters, common and envelope parameter, user parameters and macros
* The played keys are lighting red if global or clip recording (does not work if recording clip is outside of the monitored 8x8 matrix).
* Changed behaviour of new button: It creates now a new clip on the selected track and slot, starts play and enables overdub.
* Long press Accent to change fixed accent value.
* Press Shift+Quantize to access the Groove options.
* Double click Play to move play cursor to start of song.
* Footswitch 2 now triggers the new button.
* Small fix for tap tempo.
* Fixed that right/left arrows incorrectly refresh playing pads
* Fixed turning off blinking when switching from Session to other views. 

# 2.50
* Added Drum Sequencer (Press Shift + Note).
* Patch browsing (In Device mode press Browse).
* Toggle perspectives and panels (Keep Master pressed).
* Added more Scales and Chromatic mode for all of them.
* Color scheme of note sequencer is harmonized with drum sequencer.
* Accent button: If active velocity is always max in Sequencer and Play modes.
* Option to flip session mode to match arrangement view (press Session button twice).
* Footswitch 1: Sends sustain
* Footswitch 2: Toggle record
* Volume, Track and Master mode display now VU meters. Press one of these buttons twice to turn off.

# 2.00
* Added indication on editable parameters, macros, volumes, etc.
* Added macro control (press Device twice)
* Shift+Record toggles launcher overdub.
* Stop: Keep pressed and select one of the 8 tracks. The playing clip on that track stops.
* Shift+Stop: Stops all playing clips.
* Sequencer Mode:
  * Use the Scene buttons to change the grids resolution.
* Session Mode:
  * Hold _New_ button and press an empty slot (pad) to create a new clip. Before choose the length by holding the _Fixed Length_ button.
  * If Select is pressed when pressing a pad it is only selected and not started.
  * Shift + 1st row button returns track to arrangement sequencer.
* Improved track selection on bank change.
* Improved display and pad redraw performance.
* Fixed lighting of Mute and Solo buttons.
* Fixed hang after script restart.

# 1.51
* More scales.

# 1.50
* Added Sequencer Mode.
* Fixed Shift behaviour.

# 1.02
* Added auto configuration string for Linux.
* Performance improvements.

# 1.01
* Shift + Undo now executes Redo.