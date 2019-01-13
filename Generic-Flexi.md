# Bitwig Studio | Generic Flexi

Supports any MIDI controller with 1 midi in-/output.

Open the settings to configure your device. First, select the input and output of your MIDI controller.
You have 200 slots to map buttons, knobs, faders, etc. to a function in Bitwig.

Select the slot in which you want to put a mapping.

To assign a slot press a button or move a knob/fader on your controller. You should see the transmitted
MIDI CC, note or Program Change (other MIDI data types are not supported) that was sent by your controller.

Click the Set button to assign this MIDI values to the selected slot. After that select the function you 
want to assign.
If you want to clear a slot, set the MIDI trigger type to "Off".

**IMPORTANT**: Your settings are not automatically stored!

# Storing and loading a configuration

* In the **Ex-/Import section** enter a file name in the text field to store to. On Windows and Mac you can click on the Select button to choose a file. On Linux you have to type the file name. Make sure you choose a name in a writable folder.
* Click on Export to store the settings.
* Click on Import to load a configuration (make sure you export your current configuration first).

# The parameters are as follows:

* Type: MIDI status type, which triggers the function: CC, a note, program change command or pitchbend
* Number: The CC, note or Program change number, which should trigger the function (ignored for pitchbend)
* Midi Channel: The midi channel (1-16), on which the MIDI message should be accepted/received
* Knob Mode: This option only applies to continuous functions like changing the volume of a track. Depending on the possibilities of your controller knob you need to choose the matching mode.
* Function: Choose a function from the different categories that should be executed, when the configured MIDI message is received.
* Send value to device: This option only applies to continuous functions like changing the volume of a track. If it is enabled, the current value is sent to the controller with the configured CC.

