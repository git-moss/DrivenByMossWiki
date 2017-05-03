## 1. How can I contact you?

Please put all Push4Bitwig related questions into the related thread on KVR: http://www.kvraudio.com/forum/viewtopic.php?f=268&t=409982

## 2. I want to report a bug or have a feature request

Please use the [[Issues tracker|https://github.com/git-moss/Push4Bitwig/issues]] on GitHub and give clear steps to reproduce. If you have no idea how to create an issue use the forum (see above).

## 3. Sometimes when playing notes, some notes that light up green, and I know they shouldn't be lit up. For example ill press a note and the one directly under it will light up.

Known Bitwig bug which happens randomly. The raw midi data of Push gets also fed to Bitwig Studio. As a workaround select as MIDI input for the track only "Push" (not all midi input). If you find a consistent way to reproduce this bug please report to Bitwig.

## 4. When pressing "select" and a drum pad, its not silently selecting it.

See previous comment.

## 5. When sequencing drums or even playing them in, I can't see a green play head on Push, and Im pretty sure the notes are displayed incorrectly on Push.

Make sure that the clip has the focus (click on it with the mouse). There is currently no way via the API to fix this.

## 6. Why is the feature XYZ not there? Feature XYZ is buggy!

Push4Bitwig contains all the functionality of the Ableton version (and much more!) that is possible with the current Bitwig API. All necessary API changes and extensions are already reported to Bitwig and on their TODO list. It is just a matter of priorities and time. If you want to make sure that your wish or problem is really there you can check https://github.com/git-moss/Push4Bitwig/issues/135 and
https://github.com/teotigraphix/Framework4Bitwig/issues

## 7. My Push is not working at all

Make sure you have selected the correct midi in/out ports. It needs to be number 2! See the [[Installation instructions|Installation]] in the Wiki|Installation.

## 8. I don't like the speed of the knobs. Can I change it?

You can adjust the value to your liking in the file Config.js by changing the value of "Config.fractionValue" to a larger or smaller value, e.g. "5" or "30".
The value when Shift is pressed is set by "Config.fractionMinValue".
The values must be integers (no fractions like 11.5).

## 9. Where is the version number of the installed script?

It's in Push.control.js line 17. Sadly, this information is not yet displayed in Bitwig Studio.
