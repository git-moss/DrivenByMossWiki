Get the latest stable release from: http://www.mossgrabers.de/Software/Bitwig/Bitwig.html

**The version in GitHub might always be in an alpha or beta state, you have been warned!**

# Basic installation

1. Extract the ZIP file. It contains a file named **DrivenByMoss.bwextension**.
2. Copy that file in the following location depending on your OS:
      * Windows	`%USERPROFILE%\Documents\Bitwig Studio\Extensions\`
      * Mac	`~/Documents/Bitwig Studio/Extensions/`
      * Linux   `~/Bitwig Studio/Extensions/`
3. Start Bitwig Studio and open the *Dashboard*. Select *Settings* and *Controllers*.
4. Click on **Autdetect**. Note: Since Bitwig 2 you automatically get a popup notification if a controller is found. 
5. Alternatively, select **Add controller manually**:

See device specific additional installation notes below.

# Arturia Beatstep / Beatstep Pro

Load the respective template fron the folder _resources/beatstep_ into the device by using Arturias Midi Control Center.

# Open Sound Control (OSC) specifics
1. Select a midi input port. It is not really important which one you choose because it is just used to insert midi notes into Bitwig received as an OSC command. Best thing is to use a virtual midi port.
2. Adjust the IP-adresses and ports of your computer and the client device you want to use. NOTE: You need to restart the extension if you made a change!

The ZIP file has a folder _resources/osc_ which contains 1 example file for Cycling 74s Max and 1 example file for TouchOSC (Android and iOS app).

# Novation Lauchpad Pro specifics
If you added the controller manually, choose the 2nd port (*MIDIIN2 (Launchpad Pro)* and *MIDIOUT2 (Launchpad Pro)* on Windows).

# Ableton Push specifics
If you added the controller manually, choose **Ableton -> Push** or  **Ableton -> Push 2** depending on your specific controller. On **Push 1** make sure that for MIDI in- and output the 2nd port is selected (**MIDIIN2 (Ableton Push)** and **MIDIOUT2 (Ableton Push)** on Windows). For **Push 2** it is the first port.

## Additional installation for the Push 2 to support the display

To support the display of the Push 2 you need to run the application Push2Display, which is included in the ZIP file. You find the application in the sub-folder **resources/push2display**.
This application communicates with the extension in Bitwig and the Push 2 display via USB.
If the application is not running you can still use the extension, except that the display will be off.

The application is written in Java to run on Windows, Linux and Mac. Therefore, make sure you have the latest Java Runtime installed (at least 1.8.0_66). OpenJDK will not work since it does not include JavaFX at the moment!
Get it from: http://www.oracle.com/technetwork/java/javase/downloads/index.html (see below for which file to choose)

### Installation on Windows

For the Java installtion choose the file **jdk-8u65-windows-x64.exe** (or newer).
There is a batch file **Run.cmd** provided to start the Push2Display application. Make sure you have the environment variable **JAVA_HOME** set to the installed Java Runtime, e.g. **C:\Program Files\Java\jdk1.8.0_66** on my system. Alternatively, you can also replace the path directly in the batch file. 

####How to add Run.cmd to the start menu on Windows 8/10 with the Bitwig icon:

1. Open the following folder in the Explorer (insert your user name): C:\Users\**<YOUR_USER_NAME_HERE>**\AppData\Roaming\Microsoft\Windows\Start Menu\Programs
2. Drag and drop **Run.cmd** to that folder while holding down the **Alt*-key to create a link
3. Select the link and press F2 to rename it.
4. Name it something like **Bitwig with Push 2**
5. Right click on **Run.cmd** and open the properties dialog
6. Press the button which allows to select a different icon
7. In the upcoming dialog click on the file select button
8. Navigate to the Bitwig installation folder (C:\Program Files (x86)\Bitwig Studio) and select the **Bitwig Studio.exe** file.
9. Select the Bitwig icon and confirm all dialogs.
10. Open up the start menu by pressing the Windows key
11. Type **Bitwig**. **Bitwig with Push 2** should appear now in the search results.
12. Right click on **Bitwig with Push 2** and choose to add it to the start menu

### Installation on Mac

For the Java installation choose the file **jdk-8u66-macosx-x64.dmg** (or newer). The installation adds the Java application automatically to the environment. Therefore, no further configuration is necessary.
You can start the Push2Display application with **run.command** which is included in the folder. You can also copy that file anywhere you like on your disc, e.g. the Desktop.
If you get an error that you do not have access to **run.command**: open a terminal, enter the directory, which contains run.command and execute the following line:
`chmod a+x run.command`

### Installation on Linux

Installing the Oracle JDK on Ubuntu is a bit tricky. I found a simple way here (see the explanation under the header **Using a PPA**): http://askubuntu.com/questions/521145/how-to-install-oracle-java-on-ubuntu-14-04
If you choose this way the Java application should be automatically added to the environment. Therefore, no further configuration is necessary.
You can start the Push2Display application with **run.sh** which is included in the folder. You can also copy that file anywhere you like on your disc, e.g. the Desktop. 

Accessing USB requires root access. Therefore, as a first test open the terminal console and type `sudo ./run.sh`.
To run the Application as a normal user copy the file `99-userusbdevices.rules` to the folder `/etc/udev/rules.d/`.
It gives the group **audio** access to the Push 2 controller. Make sure that your user is a member of that group and the group does exist. A more indepth explanation can be found here: http://usb4java.org/faq.html
After you have copied the file reboot your computer.

### Configuration of the communication port (optional)

The application communicates via the IP port 7000 with the extension. If for any case this port is already in use on your system you can change it. To do so first change it in the Push4Bitwig preferences (the first option). After that change it in the application and click on **Apply**.

### Other options

1. Bitwig Path: The absolute path to the Bitwig application. Clicking on Run will then start Bitwig Studio. If you have **Run automatically** enabled and the path is set correctly the application will automatically start Bitwig Studio when you start Push2Display. This feature makes it possible that you have to only start one application when you want to use Bitwig Studio. The correct paths are automatically set depending on your OS. In case you installed Bitwig Studio in a different location you need to adjust that path.

2. Font and color settings: Allows you to adjust the layout of the display

3. Preview: If enabled the content of the display is also shown in the application. This is only intended to be used for debugging. Since it eats up quite some resources of the CPU you should disable it.
