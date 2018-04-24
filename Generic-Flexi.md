# Bitwig Studio | Generic Flexi (Unreleased)

Supports any MIDI controller with 1 midi in-/output.

Open the settings to configure your device. First, select the input and output of your MIDI controller.
You have 200 slots to map buttons, knobs, faders, etc. to a function in Bitwig.

To fill a slot press a button or move a knob/fader on your controller. You should see the transmitted 
MIDI CC, note or Program Change (other MIDI data types are not supported) that was sent by your controller.

Click the Add button to move this configuration to the first free slot. Select the function you want to assign.
If you want to clear a slot, set the function to "Off".

The parameters are as follows:
* Type: MIDI status type, which triggers the function: CC, a note or a Program change command
* Number: The CC, note or Program change number, which should trigger the function
* Midi Channel: The midi channel (1-16), on which the MIDI message should be accepted/received
* Knob Mode: This option only applies to continuous functions like changing the volume of a track. Depending on the possibilities of your controller knob you need to choose the matching mode.
* Function: Choose the function that should be executed, when the configured MIDI message is received. Set to "Off" to clear the slot.
* Send value to device: This option only applies to continuous functions like changing the volume of a track. If it is enabled, the current value is sent to the controller with the configured CC.

Storing a configuration:
* In the upper part there is the **Ex-/Import section**
* Enter a file name in the text, where to store the settings to (or read from). On Windows and Mac you can click on the Select button to choose a file. On Linux you have to type the file name.
* Click on Export to store the setting.
* Click on Import to load a configuration (make sure you export your current configuration first)
