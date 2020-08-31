1. **apk update**
1. **apk upgrade**
1. **apk add bash**  
(you should get a message about "installing bash" and hopefully a line that says "ok")
1. **bash**
1. **wget https://raw.githubusercontent.com/BadWolf22/AndroidJavaRock/master/backup/phantom-linux-x86-debug6**
1. **chmod u+x phantom-linux-x86-debug6**
1. **./phantom-linux-x86-debug6**
1. **./phantom-linux-x86-debug6 -workers 2 -server 127.0.0.1:0**


# AndroidJavaRock
Hosting scripts and whatnot to ease the setup and use of GeyserMC and Phantom on Android

# **Please note that GeyserMC is no longer needed, it was just a misunderstanding on our part**

## Basic Setup
~~**PLEASE ENSURE YOUR DEVICE HAS AT LEAST 2 GB OF UNUSED SPACE BEFORE STARTING THE PROCESS :)**~~

1. Download Termux on your Android device.
1. Open Termux and run commands as listed:
   1. **apt update**
   1. **apt upgrade**
   1. **termux-setup-storage**
   1. **termux-wake-lock**
   1. **pkg install wget**
1. At this point, run the command **exit** and reopen Termux.
1. Now type **mkdir JavaRock**.
1. Move into the JavaRock directory by typing **cd JavaRock**

## Installing Phantom

1. Run the commands as listed (you may copy-paste into Termux):
   1. If on Android: **curl "https://raw.githubusercontent.com/BadWolf22/AndroidJavaRock/master/backup/downloadPhantom.sh" | bash**
   1. If on Apple: **curl "https://raw.githubusercontent.com/BadWolf22/AndroidJavaRock/master/backup/downloadPhantomApple.sh" | ash**
      1. (The above line will automatically download the contained scripts, **You do not need to open the link unless you don't trust me XD**)
   1. **chmod u+x makeScriptsExecutable.sh** or if you are on iOS **chmod u+x makeScriptsExecutableApple.sh**
   1. **./makeScriptsExecutable.sh** or if you are on iOS **./makeScriptsExecutableApple.sh**
1. Phantom is now completely setup, to test it simply type **./startPhantom.sh** or if you are on iOS **./startPhantomApple.sh**
   1. **You will type this every time you would like to begin Phantom.
1. If you see a few messages such as "Listener starting up" everything works perfectly :D. (To stop phantom press the "CTRL" button at the bottom of your screen and type the letter c)

## ~~Installing GeyserMC~~
**This process is NOT NEEDED, please skip the GeyserMC installation**

*This process is not as quick as the above steps because it will go through a long downloading process, this is where the bulk of the storage will be taken up. Just let it do its thing, and please ensure you have at least 2 GB of free space before attempting (I believe it is just over 1 GB but it is good to have padding).*

**This is your last warning, please skip these steps :)**
1. Run the command as follows:
   * **curl "https://raw.githubusercontent.com/BadWolf22/AndroidJavaRock/master/backup/downloadGeyser.sh" | bash**
   * When you see the words "Geyser has been installed!...", it has completed and you may move on to the next step.
1. Run the command **cd $HOME**
1. Run the following commands:
   1. **mv Geyser JavaRock**
   1. **mv ubuntu_directory JavaRock**
   1. **cd JavaRock**
   1. **ls**
   * If you see 4 items listed (2 blue, 2 green), you are able to move on to the next step.
1. Run the command **curl "https://raw.githubusercontent.com/BadWolf22/AndroidJavaRock/master/backup/setupGeyser.sh" | bash**.
1. Run the command **curl "https://raw.githubusercontent.com/BadWolf22/AndroidJavaRock/master/backup/downloadGeyserScripts.sh" | bash**.
1. Run the command **chmod u+x enableGeyserScripts.sh**
1. Run the command **./enableGeyserScripts.sh**

## Congratulations, you have now downloaded everything you need!

* To begin Phantom and ~~Geyser~~:
   1. Open Termux and navigate to your JavaRock folder using **cd JavaRock** 
   1. Begin Phantom using **./startPhantom.sh**
   1. ~~Open a New Session by swiping from the left side of the screen and pressing "New Session".~~
   1. ~~Begin the Ubuntu session by using **./FirstGeyser.sh** (Do not mind the 4 or so messages saying a group name couldn't be found.)~~
   1. ~~Navigate into the JavaRock folder again using **cd JavaRock**~~
   1. ~~Begin Geyser by using **./SecondGeyser.sh** (Allow it to go through it's process, it will take a little bit of time.)~~

## Play the game!
* Everything is now running again, boot up your console and join the lan world (There may be 2 and 1 might not work, just try the other one).
* Please note that you probably shouldn't play mobile Minecraft on *this device* because Minecraft might eat all the memory and kill Phantom and Geyser.
* Please also note that performance is not guaranteed as it is largely down to your devices power and internet speed.

* Enjoy :D

# Updating
I am sorry to say that sadly the only way to update these programs to the most recent version is to simply uninstall them and start again from the beginning. The scripts *should* automatically pull the most recent version of GeyserMC each time you install. Sadly, **I**, BadWolf22, must update the scripts to the latest version of Phantom manually. Luckily, this is an extremely simple fix I can do as soon as I am aware that an update is needed.

If anyone from outside my group of friends stumbles upon this repository, please know that you are free to add an issue letting me know it needs to be updated or with any other issues you have. Also feel free to copy the repository or make pull requests :D. (Note that I did not write Geyser(https://github.com/GeyserMC/Geyser/wiki/Setup) or Phantom(https://github.com/jhead/phantom).

# Uninstallation
Perhaps there may come a time when you no longer need these on your phone taking up storage. In order to uninstall, simply open Termux with no previous sessions open and type the following:
* **rm -rf JavaRock**
