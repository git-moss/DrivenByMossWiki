Bitwig Studio script to support the OSC protocol.

Get the latest stable release from: http://www.mossgrabers.de/Software/Bitwig/Bitwig.html

## The following OSC messages are sent from the script

### Global

* /project/name
* /project/engine


### Transport

* /play {1,0}
* /record {1,0}
* /repeat {1,0}
* /click {1,0}
* /click/volume {0-127}
* /click/volumeStr {text}
* /click/preroll {0,1}
* /punchIn {1,0}
* /punchOut {1,0}
* /preroll {0,1,2,4}
* /overdub {1,0}
* /overdub/launcher {1,0}
* /crossfade {0-127}
* /autowrite {0,1}
* /autowrite/launcher {0,1}
* /automationWriteMode {latch,touch,write}
* /time/str {text}
* /time/signature
* /tempo/raw {0-666}
* /quantize


### Layout and panels

* /layout {arrange,mix,edit}
* /arranger/playbackFollow {0,1}
* /arranger/trackRowHeight {0,1}
* /arranger/cueMarkerVisibility {0,1}
* /arranger/clipLauncherSectionVisibility {0,1}
* /arranger/timeLineVisibility {0,1}
* /arranger/ioSectionVisibility {0,1}
* /arranger/effectTracksVisibility {0,1}
* /mixer/clipLauncherSectionVisibility {0,1}
* /mixer/crossFadeSectionVisibility {0,1}
* /mixer/deviceSectionVisibility {0,1}
* /mixer/sendsSectionVisibility {0,1}
* /mixer/ioSectionVisibility {0,1}
* /mixer/meterSectionVisibility {0,1}


### Track

* /track/{1-8}/name
* /track/{1-8}/type
* /track/{1-8}/isGroup
* /track/{1-8}/activated
* /track/{1-8}/exists
* /track/{1-8}/canHoldNotes
* /track/{1-8}/canHoldAudioData
* /track/{1-8}/position
* /track/{1-8}/selected
* /track/{1-8}/volume {0-127}
* /track/{1-8}/volumeStr {text}
* /track/{1-8}/pan {0-127}
* /track/{1-8}/panStr {text}
* /track/{1-8}/mute {1,0}
* /track/{1-8}/solo {1,0}
* /track/{1-8}/recarm {1,0}
* /track/{1-8}/monitor
* /track/{1-8}/autoMonitor
* /track/{1-8}/crossfadeMode/{A,B,AB}
* /track/{1-8}/vu
* /track/{1-8}/color   with rgb(r,g,b). r,g,b = 0..255
* /track/{1-8}/send/{1-8}/volume {0-127}
* /track/{1-8}/send/{1-8}/volumeStr {text}
* /track/{1-8}/send/{1-8}/name {text}

* /track/selected/{attribute}    Sends all attributes (as above) of the currently selected track of the active track bank

* /master/...         as above, except sends


### Scene

* /scene/{1-8}/exists
* /scene/{1-8}/name
* /scene/{1-8}/selected


### Slots

* /track/{1-8}/clip/{1-N}/name
* /track/{1-8}/clip/{1-N}/isSelected {1,0}
* /track/{1-8}/clip/{1-N}/hasContent
* /track/{1-8}/clip/{1-N}/color             with rgb(r,g,b). r,g,b = 0..255
* /track/{1-8}/clip/{1-N}/isPlaying
* /track/{1-8}/clip/{1-N}/isRecording
* /track/{1-8}/clip/{1-N}/isPlayingQueued
* /track/{1-8}/clip/{1-N}/isStopQueued      (does not work)
* /track/{1-8}/clip/{1-N}/isRecordingQueued


### Device

* /device/exists {0,1}
* /device/name {text}
* /device/bypass {0,1}
* /device/window {0,1}
* /device/expand
* /device/param/{1-8}/name {text}
* /device/param/{1-8}/value {0-127}
* /device/param/{1-8}/valueStr {text}
* /device/param/{1-8}/modulatedValue
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
* /device/layer/{1-8}/color
* /device/layer/{1-8}/send/{1-8}/volume {0-127}
* /device/layer/{1-8}/send/{1-8}/volumeStr {text}
* /device/layer/selected/...    Same attributes as for a layer
* /device/drumpad/{1-16}/...    Same attributes as for a layer
* /device/drumpad/selected/...  Same attributes as for a layer
* /device/page/selected {1-8}
* /device/page/{1-8}/ {name}
* /device/page/selected/name {name}
* /device/sibling/{1-8}/name {name}
* /device/sibling/{1-8}/selected {0,1}


### Browser
* /browser/isActive {0,1}
* /browser/filter/{1-6}/wildcard
* /browser/filter/{1-6}/exists
* /browser/filter/{1-6}/name
* /browser/filter/{1-6}/item/{1-16}/exists
* /browser/filter/{1-6}/item/{1-16}/name
* /browser/filter/{1-6}/item/{1-16}/hits
* /browser/filter/{1-6}/item/{1-16}/isSelected
* /browser/result/{1-16}/exists
* /browser/result/{1-16}/name
* /browser/result/{1-16}/isSelected
* /browser/tab {name}                               The name of the selected browser tab


### Play

/vkb_midi/note/{0-127}/color rgb(r,g,b)   Sends different colors for root notes, scale notes, out-of-scale notes, pressed or sequence notes (in red if recording is enabled).


## The following OSC messages can be received by the script

### Global

* /preroll {0,1,2,4}
* /undo
* /redo
* /project/{+,-}            Switch to the next/previous opened project
* /project/engine {1,0,-}   De-/Activate the audio engine

### Transport

* /stop {1,-}
* /play {1,-}
* /restart {1,-}
* /repeat {1,-}
* /click {1,-}              1 = Enable, No value ("-") = Toggle
* /click/volume
* /click/preroll {-,1}      Toggles click in preroll
* /punchIn {1,-}
* /punchOut {1,-}
* /record {1,-}
* /overdub {1,-}
* /overdub/launcher {1,-}
* /crossfade {0-127}
* /autowrite {0,1}
* /automationWriteMode {latch,touch,write}
* /tempo/raw {0-666}
* /tempo/tap
* /position/{+,-}           Small in-/decrease of play position
* /position/{++,--}         Large in-/decrease of play position
* /position {-2,-1,1,2}     Small in-/decrease of play position for -1 and 1, large for all other values


### Layout and panels

* /layout/{arrange,mix,edit}
* /panel/noteEditor {0,1}
* /panel/automationEditor {0,1}
* /panel/devices {0,1}
* /panel/mixer {0,1}
* /panel/fullscreen {0,1}
* /arranger/cueMarkerVisibility {0,1}
* /arranger/playbackFollow {0,1}
* /arranger/trackRowHeight {0,1}
* /arranger/clipLauncherSectionVisibility {0,1}
* /arranger/timeLineVisibility {0,1}
* /arranger/ioSectionVisibility {0,1}
* /arranger/effectTracksVisibility {0,1}
* /mixer/clipLauncherSectionVisibility {0,1}
* /mixer/crossFadeSectionVisibility {0,1}
* /mixer/deviceSectionVisibility {0,1}
* /mixer/sendsSectionVisibility {0,1}
* /mixer/ioSectionVisibility {0,1}
* /mixer/meterSectionVisibility {0,1}


### Track

* /track/bank/{+,-}                 Scrolls bank by 1
* /track/bank/page/{+,-}            Scrolls bank by 8
* /track/{1-8}/color rgb(r,g,b)     with r,g,b = 0..255
* /track/{+,-}                      Select the next/previous track
* /track/vu {0,1}                   En-/Disable VU-Meter notifications
* /track/toggleBank                 Toggles between the Audio/Instrument and Effect track bank
* /track/add/audio
* /track/add/effect
* /track/add/instrument
* /track/{1-8}/activated {0,1}
* /track/{1-8}/select
* /track/{1-8}/volume {0-127}
* /track/{1-8}/volume/indicate {0,1}
* /track/{1-8}/volume/reset
* /track/{1-8}/volume/touched {0,1}
* /track/{1-8}/pan {0-127}
* /track/{1-8}/pan/indicate {0,1}
* /track/{1-8}/pan/reset
* /track/{1-8}/pan/touched {0,1}
* /track/{1-8}/mute {1,0,-}
* /track/{1-8}/solo {1,0,-}
* /track/{1-8}/recarm {1,0,-}
* /track/{1-8}/monitor
* /track/{1-8}/autoMonitor
* /track/{1-8}/crossfadeMode/{A,B,AB} {1}
* /track/{1-8}/send/{1-8}/volume {0-127}
* /track/{1-8}/send/{1-8}/volume/indicate {0,1}
* /track/{1-8}/clip/{1-N}/launch
* /track/{1-8}/clip/{1-N}/record
* /track/{1-8}/clip/{1-N}/select
* /track/{1-8}/clip/stop
* /track/{1-8}/clip/returntoarrangement
* /track/stop
* /track/indicate/volume {0,1}      Indicate the volumes of all 8 tracks
* /track/indicate/pan {0,1}         Indicate the pans of all 8 tracks
* /track/indicate/send/{1-8} {0,1}  Indicate send 1-8 of all 8 tracks

* /track/selected/{attribute}

* /master/... (as above, except sends)


### Cursor Device / Primary Device

* /device/{+,-}
* /device/window        Displays the window for VST plugins (or Bitwig devices with additional popout windows)
* /device/bypass
* /device/expand
* /device/param/{+,-}
* /device/param/bank/page/{+,-}
* /device/param/{1-8}/value {0-127}
* /device/param/{1-8}/indicate {0,1}
* /device/param/{1-8}/reset
* /device/param/{1-8}/touched
* /device/indicate/param {0,1}
* /device/layer/{1-8}/selected
* /device/layer/{1-8}/volume {0-127}
* /device/layer/{1-8}/volume/touched {0,1}
* /device/layer/{1-8}/pan {0-127}
* /device/layer/{1-8}/pan/touched {0,1}
* /device/layer/{1-8}/mute {1,0,-}
* /device/layer/{1-8}/solo {1,0,-}
* /device/layer/{1-8}/send/{1-8}/volume {0-127}
* /device/layer/{1-8}/send/{1-8}/volume/touched {0,1}
* /device/layer/{1-8}/enter
* /device/layer/parent
* /device/layer/{+,-}
* /device/page/selected {1-8}
* /device/bank/page/{+,-}
* /device/layer/page/{+,-}
* /device/drumpad/{1-16}/...  Same attributes as for a layer
* /device/sibling/{1-8}/selected {0,1}

* Same commands apply for the primary device but use /primary/... instead of /device/...


### Scene

* /scene/{1-8}/launch
* /scene/{+,-}          Step by 1
* /scene/bank/{+,-}     Step by 8
* /scene/create         Create a new scene from all playing clips


### Browser Actions
* /browser/preset               Activates the browser to browse for presets of the currently selected device
* /browser/device               Activates the browser to insert a device after the currently selected device
* /browser/device/after         (same as /browser/device)
* /browser/device/before        Activates the browser to insert a device before the currently selected device
* /browser/commit               Commits the current selection in the browser
* /browser/cancel               Cancels the current browser session
* /browser/filter/{1-6}/{+,-}   The columns are as follows: 1: Location, 2: Favorites, 3: Creator, 4: Tags, 5: Devices, 6: Category
* /browser/filter/{1-6}/reset   Resets the filter of the column
* /browser/preset/{+,-}         Select the next/previous preset
* /browser/tab/{+,-}            Select the next/previous tab (Devices/Presets/Multisamples/...)


### Groups Actions
* /track/{1-8}/enter
* /track/parent


### Play

* /vkb_midi/{Channel:0-16}/note/{Note:0-127} {Velocity:0-127}
* /vkb_midi/{Channel:0-16}/note/+    1 octave up
* /vkb_midi/{Channel:0-16}/note/-    1 octave down
* /vkb_midi/{Channel:0-16}/drum/{Note:0-127} {Velocity:0-127}
* /vkb_midi/{Channel:0-16}/drum/+    1 drum octave up
* /vkb_midi/{Channel:0-16}/drum/-    1 drum octave down
* /vkb_midi/{Channel:0-16}/cc/{CC:0-127} {Value:0-127}
* /vkb_midi/{Channel:0-16}/aftertouch/{Note:0-127} {Pressure:0-127}     Sends Poly Aftertouch
* /vkb_midi/{Channel:0-16}/aftertouch {Pressure:0-127}                  Sends Channel Aftertouch
* /vkb_midi/{Channel:0-16}/pitchbend {Pitch:0-127 (No-Bend:64)}
* /vkb_midi/velocity {0-127 (0 disables fixed velocity, 1-127 fixes the velocity to the value)}


### Misc
* /action/{action-id}     Executes one action from the action list (e.g. /action/Save). Replace spaces in action-ids with a dash (e.g. /action/Select-All).
* /refresh    Flushes all values to the clients
