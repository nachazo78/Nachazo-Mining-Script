# Nachazo Mining Script based on deen0x script ![image](https://github.com/nachazo78/nachazo78/blob/main/argentina.png)

Al the work is from Deen0X. I change some scripts to use in my windows rigs runing nicehas!
For example scheduled task script is disable because i use scheduled task for running scripts ;)

Debloat and Optimization Script for machines running Windows 10 for mining purposes

Download package
[DNXDO_mining_Script.zip](https://github.com/nachazo78/Nachazo-Mining-Script/archive/refs/tags/v1.2.zip)

This Script help to gain performance on your system, in two main ways:
- First one, debloat windows. For this, i based on the W4RH4WK work on their project
https://github.com/W4RH4WK/Debloat-Windows-10
- Second, i included many tweaks for improve performance on windows, focused on setup a mining pc, or trying to get usable old machines such tablets, netbooks, old pcs, etc, that don´t have so much resources but can install windows 10.

As extra, there are some Utils included with the package that may be interesting for users to run on their system

# This script will modify your windows 10 installation

![image](https://user-images.githubusercontent.com/3720302/138956331-15ae85fe-4dcc-421d-8e2d-dbe241e0f224.png)


# How it works?

The main script will scan two main folders,  looking for files (subscripts) that will execute.

These files can be .cmd, .bat, .reg, .ps1, etc, anything that can be launched from the main script (cmd)

There are two main folders:
- Scripts: This contain all scripts that will be launched by the main script
- Utils: This contain extra scripts considered as Util/Tool, because will not impact directly on the performance and most of them are accessory to the installation.

Inside each main folder, there are two subfolders
- Enabled: Scripts that will be executed are included on this folder
- Disabled: If you don´t want to run some script, instead of editing or deleting, move it from Enabled folder to this one. The main script will not execute any of the scripts on this folder.

# Run modes

The script can be executed in two modes:

![image](https://user-images.githubusercontent.com/3720302/138956430-5aba8351-254b-40a2-b8c7-5509316d1fd0.png)

- Safe: This mode is less invasive, because will not in-deep modify the system. This will not gain the same level of performance than Normal mode.
- Normal: This will run all enabled scripts and utils. This will in-deep modify the system and cannot be undone.

The main script determine if a script is safe or not, simply checking if the file is named "*.safe.*"
example:
Set SystemResponsiveness for Gaming.Safe.cmd
This script will be considered safe, because their filename ends in "*.Safe.*", this case, ".Safe.cmd"

If you consider some script is safe to run on your system, simply add ".Safe" before the extension.

# Main Screen Execution

The main screen of the Script will show the subscripts launched, and a little info about the kind of subscript (the first letter of the extension, to know if a Reg file, Cmd, Bat, Ps1, etc correspond to this script)

![image](https://user-images.githubusercontent.com/3720302/138957308-d7f77f5d-b6b5-4ed6-be6d-03c4eda83144.png)

The "OK" text simply indicate that the script finalized. This will not be consider info about the result of the SubScript itself.
The "." indicate that the subscript is not a file. Is part of the main script.

# Window mode for SubScripts

The script will ask for window mode for running SubScripts.
The modes can be:

![image](https://user-images.githubusercontent.com/3720302/138958109-5521e651-1c22-4c76-908b-9a9fc74ead75.png)

- Normal: Windows will open as normal, showing all the content of the SubScript excecution.
- Min: Windows will open minimized, and you only will see the general script page.

![image](https://user-images.githubusercontent.com/3720302/138957577-af8dfe5c-4b87-4851-9756-24a83d0997d1.png)
This case the subscripts are running in minimized mode.

![image](https://user-images.githubusercontent.com/3720302/138958783-18310202-6516-4f98-9f8d-04f97e2942de.png)
This case the subscripts are running in normal mode.

Note: On some windows subscripts may appear some errors/red text/etc. Don't worry, this is normal.

# Windows Start Menu Entry

The script adds a new Windows Start Menu entry, for launch again the script when you want.

![image](https://user-images.githubusercontent.com/3720302/138959091-751cf1b2-fa9d-4dba-b6b9-1681313820f4.png)

# New feature: create restore point

Now, before running all the scripts, there is an option to create a restore point of the system
The script will enable the service for creating and managing restore points, and then will create a restorepoint with the default settings.

Thanks to TuberViejuner for this suggestion.

# Note about virtual memory

This script set the virtual memory on 20gb.
Thinking on mining 20gb is the safe amount of Vram for mining.


Hope you found useful this script.

Nachazo78
