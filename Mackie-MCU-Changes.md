#2.6 (unreleased)
* New: **Option + Record** - Creates a new clip on the selected track and slot, starts play and enables overdub.
* New: **Option + Track selection buttons** - Stop the playing clip on the specific track.
* New: New option in Assignable Buttons: Quantize the currently selected clip.
* New: **Shift + Masterfader** - Changes Metronome Volume
* New: **Option + Read** - Resets any automation overrides.
* Fixed: Button combinations (Shift, etc.) did not work across mutliple MCU devices

#2.5
* New: MCU_NUDGE button executes Tap Tempo
* New: MCU_DROP button executes Duplicate
* New: MCU_GROUP button executes Automation Write
* New: MCU_AUX button switches to Arrange layout.
* New: MCU_BUSSES button switches to Mix layout.
* New: MCU_OUTPUTS button switches to Edit layout.
* New: MCU_F8 button toggles device on/off.
* New: Option + Track (MCU_MODE_IO): Pin cursor track
* New: Option + Device (MCU_MODE_PLUGIN): Pin cursor device

#2.4
* New: Option to deactivate the automatic selection of track when the channel fader is touched.

#2.3
* New: The scrub button switches now through all modes (instead of only Track and Device).
* New: Optimized display updates
* Fixed: Modes did not update on all devices (when multiple ones are in use) when the mode change was not initiated on the main device.

#2.2
* Fixed: Crash when using faders as knobs and no track is selected.

#2.1
* New: Startup mode is now panorama
* New: When you touch a volume fader, volume mode is temporarily activated until you release the fader.
* New: Support to switch editing modes (track, panorama, volume, device) for devices who have no dedicated mode buttons. Option 1 is to enable the new setting to use the vertical zoom buttons to switch editing modes. Option 2 is to assign the new functions "Previous mode" and "Next mode" to function buttons.
* New: Setting to use the faders like the editing knobs (enable for devices which do not have knobs).

#2.0
* New: Support for 1-3 extenders (can be any device which supports the MCU protocol)

#1.3
* Fixed: Tracks were not displayed if a track name contained umlauts.
* Fixed: Text alignment on 2nd display was wrong.
* Fixed: Better text alignment for master mode to not interfere with VU display.

# 1.2
* New: Toggle VU meters with Global View button on MCU
* Fixed: VU meters id not work on Mackie MCU
* Fixed: First row texts were offset by 1
* Fixed: Wrong positioning of beats display if tempo was less than 100.

# 1.1
* New: Support for assignment display
* New: Lighting of SMPTE/BEATS LEDs.
* New: Save button saves the current project
* New: Marker button toggles the display of markers in the arranger
* Fixed: Browser did only show results for Presets (now also devices, samples, etc.).
* Fixed: SMPTE display was off by 1 character

# 1.0
Compatible with Bitwig 2.1.
* Initial release.
