# iOSJavaRock
Hosting scripts and whatnot to ease the setup and use of GeyserMC and Phantom on **iOS** only.  
(Please switch to branch Android-Only for Android information)

## Basic Setup
* Please be sure to allow commands to complete before moving to the next step!  
  
1. Download [TestFlight](https://apps.apple.com/us/app/testflight/id899247664) on your iOS device.
1. Tap on this [link](https://testflight.apple.com/join/97i7KM8O) on your iOS device.
1. Open iSH (downloaded by the link above) and run commands as listed:
   1. **apk update**
   1. **apk upgrade**
   1. **apk add bash**
   1. **apk add curl**
   1. **apk add wget**
   1. **bash**
1. Now type **mkdir JavaRock**.
1. Move into the JavaRock directory by typing **cd JavaRock**

## Installing Phantom

1. Run the commands as listed (you may copy-paste into iSH):
   1. **curl "https://raw.githubusercontent.com/BadWolf22/JavaRock/iOS-Only/scripts/downloadPhantom.sh" | bash**  
      * (The above line will automatically download the contained scripts, **You do not need to open the link unless you don't trust me XD**)
   1. *you must type the following command or copy paste from the **discord server**:* **sed -i '3s,$,[server ip here],' ./startPhantom.sh**
   1. **chmod u+x makeScriptsExecutable.sh**
   1. **./makeScriptsExecutable.sh**
1. Phantom is now completely setup, to test it simply type **./startPhantom.sh**  
   **You will type this every time you would like to begin Phantom.**  
   If you see a few messages such as "Listener starting up" everything works perfectly :D.  
   (To stop phantom press the "**^**" (up-caret) button at the bottom of your screen and type the letter **c**)

## Congratulations, you have now downloaded everything you need!

* To begin Phantom:
   1. I would recommend ensuring your device will not fall asleep by adjusting the sleep timer to **never**.
   1. I would also recommend not relying on the app running in the background but leave it open in the foreground.
   1. Open iSH and navigate to your JavaRock folder using **cd JavaRock** 
   1. Use the command **bash**
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
Perhaps there may come a time when you no longer need these on your phone taking up storage. In order to uninstall, simply open iSH and type the following:
* **rm -rf JavaRock**
