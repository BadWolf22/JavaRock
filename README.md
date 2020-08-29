# AndroidJavaRock
Hosting scripts and whatnot to ease the setup and use of GeyserMC and Phantom on **Android** only.  
(Please switch to branch Apple-Only for iOS information)

## Basic Setup

1. Download Termux on your Android device.
1. Open Termux and run commands as listed:
   1. **apt update**
   1. **apt upgrade** (type **y** and press **enter/return** if prompted)
   1. **termux-setup-storage** (press **Allow** when prompted)
   1. **termux-wake-lock** (press **Allow** when prompted)
   1. **pkg install wget** (be sure to type **y** and press **enter/return** if prompted)
1. At this point, run the command **exit** and reopen Termux.
1. Now type **mkdir JavaRock**.
1. Move into the JavaRock directory by typing **cd JavaRock**

## Installing Phantom

1. Run the commands as listed (you may copy-paste into Termux):
   1. **curl "https://raw.githubusercontent.com/BadWolf22/JavaRock/Android-Only/scripts/downloadPhantom.sh" | bash**  
      * (The above line will automatically download the contained scripts, **You do not need to open the link unless you don't trust me XD**)
   1. **nano ./startPhantom.sh**
      1. Drag from the bottom of the window to the top to move the cursor down. Then delete "**[server ip here]**" and type or paste your serverIp:port.
      1. Press the **CTRL** button and type the letter *s*
      1. Press the **CTRL** button and type the letter *x*
   1. **chmod u+x makeScriptsExecutable.sh**
   1. **./makeScriptsExecutable.sh**
1. Phantom is now completely setup, to test it simply type **./startPhantom.sh**  
   **You will type this every time you would like to begin Phantom.**  
   If you see a few messages such as "Listener starting up" everything works perfectly :D.  
   (To stop phantom press the "**CTRL**" button at the bottom of your screen and type the letter **c**)

## Congratulations, you have now downloaded everything you need!

* To begin Phantom:
   1. Open Termux and navigate to your JavaRock folder using **cd JavaRock** 
   1. Ensure your phone does not sleep by using **termux-wake-lock**  
   1. Begin Phantom using **./startPhantom.sh**

## Play the game!
* Everything is now running again, boot up your console and join the lan world.
* Please note that you probably shouldn't play mobile Minecraft on *this device* because Minecraft might eat all the memory and kill Phantom and Geyser.
* Please also note that performance is not guaranteed as it is largely down to your devices power and internet speed.

* Enjoy :D

# Updating
I am sorry to say that sadly the only way to update these programs to the most recent version is to simply uninstall them and start again from the beginning. Sadly, **I**, BadWolf22, must update the scripts to the latest version of Phantom manually. Luckily, this is an extremely simple fix I can do as soon as I am aware that an update is needed.

If anyone from outside my group of friends stumbles upon this repository, please know that you are free to add an issue letting me know it needs to be updated or with any other issues you have. Also feel free to copy the repository or make pull requests :D. *(Note that I am not the creator of Phantom(https://github.com/jhead/phantom))*.

# Uninstallation
Perhaps there may come a time when you no longer need these on your phone taking up storage. In order to uninstall, simply open Termux with no previous sessions open and type the following:
* **rm -rf JavaRock**
