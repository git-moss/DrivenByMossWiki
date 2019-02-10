# Generic Flexi - Changes

## 2.2 (unreleased)

Compatible with Bitwig 2.4.

* New: Added commands to control Browser filter columns 7 and 8.
* New: Added Browser mode.
* New: Select buttons in Parametermode select parameter pages instead of devices.
* Fixed: Removed duplicated function "Transport: Set Crossfader", use "Master: Crossfader" instead.
* Fixed: Mode knobs did always use relative mode 1, even if 2 or 3 was selected.
* Fixed: Values of Track-, Volume- and Parametermode were not reflected correctly back to the device.
* Fixed: Prevent console warnings when values go out of bounds in relative modes.

## 2.1

Compatible with Bitwig 2.4.

* New: Added command: "Device: Parameters"

## 2.0

Compatible with Bitwig 2.4.

* New: Completely new settings user interface
* New: Support for modes: Track, Volume, Panorama, Send 1-8, Parameters
* New: Support for using Pitchbend as a controller
* New: Added command: "Master: Crossfader"
* Fixed: Blocking notes which are mapped to a command did only work after restart.
* Fixed: "Send value to device" did always send on midi channel 1.

## 1.2

Compatible with Bitwig 2.4.

* New: Added commands for markers
* New: Added commands for device parameter page selection
* New: Set indication for volume, pan, sends and parameters only if a command is configured

## 1.1

Compatible with Bitwig 2.3.

* New: Track: Scroll Track
* New: Device: Scroll device
* New: Device: Scroll Parameter Bank
* New: Browser: Scroll Filter in Column 1
* New: Browser: Scroll Filter in Column 2
* New: Browser: Scroll Filter in Column 3
* New: Browser: Scroll Filter in Column 4
* New: Browser: Scroll Filter in Column 5
* New: Browser: Scroll Filter in Column 6
* New: Browser: Scroll preset
* New: Browser: Scroll tab
* New: Clip: Scroll clips
* New: Added indication of selected parameters
* Fixed: Relative modes of "Track Selected: Set Send X" did not work

## 1.0

Compatible with Bitwig 2.3.

* Initial release.
