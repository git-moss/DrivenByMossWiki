# Installation

Get the latest stable release from [my homepage](http://www.mossgrabers.de/Software/Bitwig/Bitwig.html).

> **The version in GitHub might always be in an alpha or beta state, you have been warned!**

## Basic installation

1. Extract the ZIP file. It contains a file named **DrivenByMoss.bwextension**.
2. Copy that file in the following location depending on your OS:
   * Windows: `%USERPROFILE%\Documents\Bitwig Studio\Extensions\`
   * Mac: `~/Documents/Bitwig Studio/Extensions/`
   * Linux:   `~/Bitwig Studio/Extensions/`
3. Start Bitwig Studio and open the *Dashboard*. Select *Settings* and *Controllers*.
4. If **Autdetect** is enabled for most of the controllers you automatically get a popup notification.
5. Alternatively, select **Add controller manually**; See device specific additional installation notes below.

## Arturia Beatstep / Beatstep Pro

Load the respective template from the folder _resources/beatstep_ into the device by using Arturias Midi Control Center.
Only Beatstep Pro: In the Device Settings Tab set the User Midi Channel to 3.

## Open Sound Control (OSC) specifics

1. Select a midi input port. It is not really important which one you choose because it is just used to insert midi notes into Bitwig received as an OSC command. Best thing is to use a virtual midi port.
2. Adjust the IP-addresses and ports of your computer and the client device you want to use. NOTE: You need to restart the extension if you made a change!

The ZIP file has a folder _osc_ which contains example files for Cycling 74s Max, TouchOSC and Open Stage Control.

## Novation Lauchpad specifics

* Pro: If you added the controller manually, choose the 2nd port (*MIDIIN2 (Launchpad Pro)* and *MIDIOUT2 (Launchpad Pro)* on Windows).
* Make sure the Launchpad sends on Midi Channel 1

## Ableton Push specifics

If you added the controller manually, choose **Ableton -> Push** or  **Ableton -> Push 2** depending on your specific controller. On **Push 1** make sure that for MIDI in- and output the 2nd port is selected (**MIDIIN2 (Ableton Push)** and **MIDIOUT2 (Ableton Push)** on Windows). For **Push 2** it is the first port.