# ESP32-StarterKit
A repository with everything you need to get started with the CompSoc ESP-32 starter kits. Follow this getting-started guide in order 

**Contents:**
1) [Setting up your environment](#section1)
2) [Downloading the Git Repo](#section2)
3) [Uploading to your ESP32](#section3)

## <a id="section1">Setting up your environment</a>

### Download an IDE
Download either [Visual Studio Code](https://code.visualstudio.com) (Recommended) or [Atom](https://atom.io)

Or if you're a mac user with [homebrew](https://brew.sh):
```
brew cask install visual-studio-code
```
*homebrew is a package manager for mac, if you're ComSci with a mac, you NEED this*

### Installing PlatformIO
Open VSCode and click navigate to the extensions menu:
![Visual Studio Code](https://i.imgur.com/qYN61Ov.png "Visual Studio Code")

Search `platform` in the search bar, click `install` under PlatformIO IDE:
![PlatfromIO Extension](https://i.imgur.com/QdjrJ34.png "Visual Studio Code")

VSCode will have to be reloaded during the PlatformIO installation (possibly twice):
![Reload PlatformIO](https://i.imgur.com/k3HPd3j.png "Visual Studion Code")


### Installing the Espressif platform
*Espressif is the company that makes the hardware and firmware for the ESP-32*

Once PlatformIO has been successfully installed you will see the PlatformIO interface open on the welcome screen.
Next we need to install the tools which allows us to compile code suitable for the ESP32 (don't worry, PlatformIO does all the tricky stuff for you in the background, so we can concentrate on drawing dickbutts!)

Navigate to the Platform manager and click `Install Embedded Platform`:
![Installing Espressif Platform](https://i.imgur.com/T0fXphj.png "Visual Studio Code")

Search for `Espressif`, and click on `Espressif 32`:
![Installing Espressif Platform](https://i.imgur.com/nxiMjNE.png.png)

Click `install` and let it do it's thing:
![Installing Espressif Platfrom](https://i.imgur.com/SJjU9X3.png)

----

## <a id="section2">Downloading the Git Repo</a>

Make sure you have [git](https://git-scm.com) installed

Open a new terminal (mac/linux) or CMD (windows) window in a project folder of your choosing and enter: 
`git clone https://github.com/cardiff-compsoc/ESP32-StarterKit.git`

This will copy all the files in this repository onto your computer.

----


## <a id="section3">Uploading to your ESP32</a>

In the repository you just downloaded, right click on `OLED-Demo.ini`, and open with Visual Studio Code

Make sure your ESP32 is connected to your computer and click the **-->** in the blue bottom task-bar

PlatformIO will download the libraries you need automatically, and attempt to upload the program to your ESP32.

It might fail the first time, so give it another go and hopefully it will upload successfully.

To upload again, make sure you close the terminal window using the rubbish-bin icon.
