# Android Manual Rotation Shell Scripts
A set of two shell scripts that set a rooted android device's user rotation to 270 degrees and 0 degrees when run.

## Instructions (WIP)
I was initially only intending this for personal use, and since I made it a few weeks ago, I'm unsure if the steps are fully accurate. Will test soon!\
Step 1) Use your method of choice to download the scripts onto the  your *rooted* Android device.\
Step 2) Download the [Termux](https://termux.dev/en/) and [Automation](https://f-droid.org/en/packages/com.jens.automation2/) applications and install them on your device.\
Step 3) After giving Termux and Automation the appropriate permissions, chmod 755 the two scripts in Termux.\
Step 4) In Automation, create a new rule and add the task "Run script or executable".\
->Step 4a) Check the box that says "Run as root"\
->Step 4b) In the "Path" input, type "/system/bin/sh"\
->Step 4c) In the "Parameters" tab add the **full path** of the first of your script files (likely /storage/emulated/0/\[Directory\]/\[FileName\])\
Step 5) For the same rule, add a trigger. I personally add "Battery Level Exceeds 100%" so that I only manually run the script.\
Step 6) Before running the first script, complete steps 4 and 5 for the second script so it is easy to undo the rotation.\
Step 7) Turn Automation on in the Overview tab of the app, then long press the rule you created and click "Run manually".
