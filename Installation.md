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
5. Alternatively, select **Add controller manually**
6. See device specific additional installation notes below.

## Arturia Beatstep / Beatstep Pro

Load the respective template from the folder _resources/beatstep_ into the device by using Arturias Midi Control Center.
Only Beatstep Pro: In the Device Settings Tab set the User Midi Channel to 3.

## Ableton Push

If you added the controller manually, choose **Ableton -> Push** or  **Ableton -> Push 2** depending on your specific controller. On **Push 1** make sure that for MIDI in- and output the 2nd port is selected (**MIDIIN2 (Ableton Push)** and **MIDIOUT2 (Ableton Push)** on Windows). For **Push 2** it is the first port.

### Installation on Linux
Accessing USB requires root access. To run the Application as a normal user copy the file `99-userusbdevices.rules` to the folder `/etc/udev/rules.d/`.
It gives the group **audio** access to the Push 2 controller. Make sure that your user is a member of that group and the group does exist. A more in-depth explanation can be found [here](http://usb4java.org/faq.html).
After you have copied the file reboot your computer.

## Novation Lauchpad

* Pro: If you added the controller manually, choose the 2nd port (*MIDIIN2 (Launchpad Pro)* and *MIDIOUT2 (Launchpad Pro)* on Windows).
* Make sure the Launchpad sends on Midi Channel 1

## Open Sound Control (OSC)

1. Select a midi input port. It is not really important which one you choose because it is just used to insert midi notes into Bitwig received as an OSC command. Best thing is to use a virtual midi port.
2. Adjust the IP-addresses and ports of your computer and the client device you want to use. NOTE: You need to restart the extension if you made a change!

The ZIP file has a folder _osc_ which contains example files for Cycling 74s Max, TouchOSC and Open Stage Control.

## Native Instruments Komplete Kontrol Mk II

1. Map the first automation parameter to the first parameter of the first parameter page.
2. In the Bitwig settings set SETTINGS -> Plug-ins -> "Independent plug-in host process for" NOT to "Each plug-in".
Also see the setup tutorial here: https://youtu.be/4kUuio1BOQk

