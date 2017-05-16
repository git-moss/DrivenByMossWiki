# 5.00
Requires Bitwig 2.1.
* New: Written now in Java
* New: Replaced isQueued with isPlayingQueued and isRecordingQueued

# 4.00
Requires Bitwig 2.0.
* Send
    * Added /browser/filter/{1-6}/wildcard
    * Added /track/{1-8}/canHoldAudioData
    * Added /track/{1-8}/position
    * Added /device/layer/{1-8}/color
    * Added /device/param/{1-8}/modulatedValue
    * Added /project/name
    * Added /project/engine
    * Renamed /browser/preset to /browser/result
    * Removed /device/common/...
    * Removed /device/envelope/...
    * Removed /device/macro/...
    * Removed /device/modulation/...
    * Removed /user/...
* Receive
    * Added /preroll {0,1,2,4}
    * Added /undo
    * Added /redo
    * Added /track/{1-8}/color RGB({0..1},{0..1},{0..1})
    * Added /browser/device/before
    * Added /browser/device/after (same as /browser/device)
    * Added /project/{+,-}
    * Added /project/engine {1,0,-}
    * Renamed /browser/presets to /browser/preset
    * Renamed /browser/devices to /browser/device
    * Removed /device/common/...
    * Removed /device/envelope/...
    * Removed /device/macro/...
    * Removed /device/modulation/...
    * Removed /user/...

# 3.12
Requires Bitwig 1.3.15+
* New: Track scrolls into view when selected
* New: /quantize Quantizes currently selected clip

# 3.11
* Fixed /browser/filter/: Index was 0-5 instead of 1-6 as described in the Wiki.
* Fixed: Bank range in grouped tracks behaves weird (requires Bitwig 1.3.8 RC 2+)

# 3.10
* Added /type attribute to tracks.

# 3.00
Compatible with Bitwig 1.2/1.3.

* BROWSER Actions
    * /browser/presets    Activates the browser to browse for presets
    * /browser/devices    Activates the browser to browse for devices
    * /browser/commit     Commits the current selection in the browser
    * /browser/cancel     Cancels the current browser session
    * /browser/filter/{1-6}/{+,-}
    * /browser/preset/{+,-}
* BROWSER Send
    * /browser/isActive {0,1}
    * /browser/filter/{1-6}/exists
    * /browser/filter/{1-6}/name
    * /browser/filter/{1-6}/item/{1-16}/exists
    * /browser/filter/{1-6}/item/{1-16}/name
    * /browser/filter/{1-6}/item/{1-16}/hits
    * /browser/filter/{1-6}/item/{1-16}/isSelected
    * /browser/preset/{1-16}/exists
    * /browser/preset/{1-16}/name
    * /browser/preset/{1-16}/isSelected
* GROUPS Actions
    * /track/{1-8}/enter
    * /track/parent
* GROUPS Send
    * /track/{1-8}/isGroup
* Added the following messages to be received:
    * /punchIn
    * /punchOut
    * /position/+    Small increase of play position
    * /position/-    Small decrease of play position
    * /position/++   Large increase of play position
    * /position/--   Large decrease of play position
    * /device/layer/{1-8}/selected
    * /device/layer/{1-8}/volume {0-127}
    * /device/layer/{1-8}/pan {0-127}
    * /device/layer/{1-8}/mute {1,0,-}
    * /device/layer/{1-8}/solo {1,0,-}
    * /device/layer/{1-8}/send/{1-8}/volume {0-127}
    * /device/layer/{1-8}/enter
    * /device/layer/parent
    * /device/layer/page/{+,-}
* Added the following message to be sent:
    * /punchIn {1,0}
    * /punchOut {1,0}
    * /scene/{1-8}/exists
    * /scene/{1-8}/name
    * /scene/{1-8}/selected
    * /position
    * /device/layer/{1-8}/exists
    * /device/layer/{1-8}/activated
    * /device/layer/{1-8}/selected
    * /device/layer/{1-8}/name
    * /device/layer/{1-8}/volumeStr
    * /device/layer/{1-8}/volume
    * /device/layer/{1-8}/panStr
    * /device/layer/{1-8}/pan
    * /device/layer/{1-8}/vu
    * /device/layer/{1-8}/mute
    * /device/layer/{1-8}/solo
    * /device/layer/{1-8}/send/{1-8}/volume {0-127}
    * /device/layer/{1-8}/send/{1-8}/volumeStr {text}
    * /send/{1-8}/name

# 2.20
Compatible with Bitwig 1.1.8.
* Added the following messages to be received:
    * /vkb_midi/{Channel:0-16}/cc/{CC:0-127} {Value:0-127}
    * /vkb_midi/{Channel:0-16}/aftertouch/{Note:0-127} {Pressure:0-127}
    * /vkb_midi/{Channel:0-16}/pitchbend {Pitch:0-127 (No-Bend:64)}
    * /vkb_midi/velocity {0-127 (0 disables fixed velocity, 1-127 fixes the velocity to the value)}
    * /track/vu {0,1} En-/Disable VU-Meter notifications
    * /refresh flushes all values to the clients
    * /track/toggleBank Toggles between the Audio/Instrument and Effect track bank
* Added the following message to be sent:
    * /track/{1-8}/exists
    * /track/{1-8}/canHoldNotes
    * /track/selected/{attribute} Sends all attributes of the currently selected track of the active track bank
    * /vkb_midi/note/{0-127}/color RGB(r,g,b) Sends different colors for root notes, scale notes, out-of-scale notes, pressed or sequence notes (in red if recording is enabled).
* Support for arrays as values (thanks to Carroll Vance)
* Support for OSC bundles (thanks to Carroll Vance)
* Fixed some message alignment bugs (thanks to Carroll Vance)
* Fixed track navigation for effect tracks.

# 2.10
Compatible with Bitwig 1.1.6.
* Added the following messages to be received:
    * /action/{action-id}, executes one action from the action list (e.g. /action/Save). Replace spaces in action-ids with a dash (e.g. /action/Select-All).

# 2.00
Compatible with Bitwig 1.1.3.
* Added the following messages to be received:
    * /crossfade {0-127}
    * /autowrite {0,1}, removed /track/{1-8}/autowrite
    * /automationWriteMode/{latch,touch,write}
    * Adding bank scrolling by 1 (/track/bank/+), scrolling by 8 is now /track/bank/page/+
    * /track/{1-8}/activated {0,1}
    * /track/{1-8}/crossfadeMode/{A,B,AB} {1}
    * /track/{1-8}/volume/indicate {0,1}
    * /track/{1-8}/pan/indicate {0,1}
    * /track/{1-8}/send/{1-8}/volume/indicate {0,1}
    * /track/indicate/volume {0,1}  Indicate the volumes of all 8 tracks
    * /track/indicate/pan {0,1}  Indicate the pans of all 8 tracks
    * /track/indicate/send/{1-8} {0,1}  Indicate send 1-8 of all 8 tracks
    * Renamed /track/{1-8}/slot/ to /track/{1-8}/clip/
    * /track/{1-8}/clip/{1-N}/record
    * /track/{1-8}/clip/{1-N}/select
    * /track/{1-8}/clip/stop
    * /track/{1-8}/clip/returntoarrangement
    * /track/stop
    * /master/volume/indicate {0,1}
    * /master/pan/indicate {0,1}
    * /device/window
    * /device/common/{1-8}/value {0-127}
    * /device/common/{1-8}/indicate {0,1}
    * /device/envelope/{1-8}/value {0-127}
    * /device/envelope/{1-8}/indicate {0,1}
    * /device/macro/{1-8}/value {0-127}
    * /device/macro/{1-8}/indicate {0,1}
    * /device/modulation/{1-8}/value {0,1}
    * /device/param/{1-8}/indicate {0,1}
    * /device/indicate/param {0,1}
    * /device/indicate/common {0,1}
    * /device/indicate/envelope {0,1}
    * /device/indicate/macro {0,1}
    * The primary device is now also supported via /primary with the same options as /device
    * /user/param/{1-8}/value {0-127}
    * /user/param/{1-8}/indicate {0,1}
    * /user/indicate/param {0,1}
    * /layout/{arrange,mix,edit}
    * /panel/noteEditor
    * /panel/automationEditor
    * /panel/devices
    * /panel/mixer
    * /panel/fullscreen
    * /arranger/cueMarkerVisibility
    * /arranger/playbackFollow
    * /arranger/trackRowHeight
    * /arranger/clipLauncherSectionVisibility
    * /arranger/timeLineVisibility
    * /arranger/ioSectionVisibility
    * /arranger/effectTracksVisibility
    * /mixer/clipLauncherSectionVisibility
    * /mixer/crossFadeSectionVisibility
    * /mixer/deviceSectionVisibility
    * /mixer/sendsSectionVisibility
    * /mixer/ioSectionVisibility
    * /mixer/meterSectionVisibility
    * /scene/+, /scene/- step now by 1 not 8
    * /scene/bank/+, /scene/bank/- step by 8
    * /autowrite/launcher

* Added the following messages to be sent:
    * /crossfade
    * /preroll
    * /autowrite, removed /track/{1-8}/autowrite
    * /automationWriteMode
    * /track/{1-8}/activated
    * /track/{1-8}/crossfadeMode/{A,B,AB}
    * /track/{1-8}/clip/{1-N}/color  with RGB(r,g,b). r,g,b = 0..1
    * /track/{1-8}/color             with RGB(r,g,b). r,g,b = 0..1
    * Renamed /track/{1-8}/slot/ to /track/{1-8}/clip/
    * Renamed /track/{1-8}/slot/{S}/isSelected to /track/{1-8}/clip/{S}/selected to be consistent with track.
    * /device/common/{1-8}/name
    * /device/common/{1-8}/value
    * /device/common/{1-8}/valueStr
    * /device/envelope/{1-8}/name
    * /device/envelope/{1-8}/value
    * /device/envelope/{1-8}/valueStr
    * /device/macro/{1-8}/name
    * /device/macro/{1-8}/value
    * /device/macro/{1-8}/valueStr
    * /device/modulation/{1-8}/name
    * /device/modulation/{1-8}/value
    * /device/modulation/{1-8}/valueStr
    * /user/param/{1-8}/name
    * /user/param/{1-8}/value
    * /user/param/{1-8}/valueStr
    * /layout {arrange,mix,edit}
    * /arranger/cueMarkerVisibility
    * /arranger/playbackFollow
    * /arranger/trackRowHeight
    * /arranger/clipLauncherSectionVisibility
    * /arranger/timeLineVisibility
    * /arranger/ioSectionVisibility
    * /arranger/effectTracksVisibility
    * /mixer/clipLauncherSectionVisibility
    * /mixer/crossFadeSectionVisibility
    * /mixer/deviceSectionVisibility
    * /mixer/sendsSectionVisibility
    * /mixer/ioSectionVisibility
    * /mixer/meterSectionVisibility


# 1.20
Compatible with Bitwig 1.1.
* Supports OSC Bundles (as used by Lemur)
* Added the following messages to be received:
    * /tempo/tap
    * /track/add/audio
    * /track/add/effect
    * /track/add/instrument
    * /overdub/launcher
    * /track/{n}/monitor
    * /track/{n}/monitor/auto
    * /master/monitor
    * /master/monitor/auto
    * /indicate/volume
    * /indicate/param
    * /indicate/macro
* Added the following messages to be sent:
    * /device/name
    * /device/bypass
    * /device/category
    * /device/creator
    * /device/preset
    * /repeat
    * /overdub/launcher
    * /overdub
    * /track/{n}/monitor
    * /track/{n}/monitor/auto
    * /master/monitor
    * /master/monitor/auto
* Unified fx, fxparam and device commands:
    * /fx -> /device
    * /fxparam -> /device/param
    * /device/params -> /device/param
* Display of note/drum range when octave is changed
* Clip launch command has to be the word 'launch' as the last part of the path to be consistent with scene launch, e.g. /track/1/clip/2/launch.
* Hosts and Ports can now be configured via the preferences dialog (restart of script required). NOTE: The receiver is not working, you still need to set it in the script!
* Note values are now received linear (not in an 8x8 matrix).
* Bugfix: /play did sometime send wrong values
* Bugfix: Scene commands are now accepted without a value
* Bugfix: Track navigation by page did not select a track

# 1.11
Compatible with Bitwig 1.0.14.
* Tempo can now be set with comma values, e.g.: /tempo/raw 128.55
* Tempo is sent
* Bugfix: Full maximum value range of knobs might not have been reached.

# 1.1
* Added the following messages to be sent out:
    * /fxparam/{1-8}/name {text}
    * /fxparam/{1-8}/value {0-127}
    * /fxparam/{1-8}/valueStr {text}
* Added the following messages to be received:
    * /vkb_midi/{Channel:0-16}/note/+     1 octave up
    * /vkb_midi/{Channel:0-16}/note/-     1 octave down
    * /vkb_midi/{Channel:0-16}/drum/{Note:0-127} {Velocity:0-127}
    * /vkb_midi/{Channel:0-16}/drum/+     1 drum octave up
    * /vkb_midi/{Channel:0-16}/drum/-     1 drum octave down
    * /scene/{1-8}/launch
    * /track/{1-8}/clip/{1-8}/launch
* BitwigOSC.touchosc now shows track names and fx parameter names. I increased the vertical size of the layout depending on your device you might not see the names. If this is the case you need to adjust the layout. Also the transpose of drum pads and keyboard is working.