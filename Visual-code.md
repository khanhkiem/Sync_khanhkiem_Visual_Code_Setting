# Introduction
This is a tutorial to sync my visual code setting to your visual code

# Requirement
Install Settings Sync extension to your Visual Studio Code for syncing:  
> https://marketplace.visualstudio.com/items?itemName=Shan.code-settings-sync*

# Download to sync Visual Studio Code setting
**CAUTION** You must pay attention to my guide, especially **step 2**
1. Go to setting sync, scroll down, find and follow his "Download your setting" instruction, using my *Gist ID:  
    > c52c1c8bc3a67c165fa630782b61e114*.
1. You may encounter merge conflict in setting.js, I strongly recommend you concat 2 setting.js file (or discard the one that contain only "sync setting").
1. Reload visual code to install synced extension.

# Sync system setting
**CAUTION** You should sync visual code setting again, everytime you sync my new system setting, to ensure that you don't miss any new visual code setting that related to system setting.
You may encounter some system requirement for these extension (system library, dependency, etc..). This session will guide you to install them

## Shell
- Install go 1.9:
    > https://golang.org/dl/
- Install shfmt:
    > go get -u mvdan.cc/sh/cmd/shfmt

## C++
- Install clang 3.8  
    > sudo apt-get install clang  
- Check if clang version is 3.8  
    > sudo apt-get install clang  

## Arduino
- Install Arduino IDE, read this guide carefully, especially the last section:  
    > https://www.arduino.cc/en/Guide/Linux
- Open Visual code
- Ctrl + , to access your user setting
- Edit "arduino.path" field, for example:
    > "arduino.path": "/home/khanh/Downloads/arduino-1.8.4"
- Connect your Arduino Board, for example:
    > Arduino Uno
- Press F1 search for Arduino: Select Serial Port
- Make sure /dev/ttyACM0 does appears, choose it. If not, reconnect your Board until it appears
- Press F1 search for Arduino: Change Board Type
- Select Arduino Uno
- Code then press F1 search for Arduino: Upload or Ctrl + Alt + U

## Python
- Install Anaconda Distribution:
    > https://www.continuum.io/downloads
- Install TensorFlow, Deep learning library, follow "Installing with Anaconda" section only:
    > https://www.tensorflow.org/install/install_linux

## Node.js and npm
- Follow their instruction
    >  https://docs.npmjs.com/getting-started/installing-node

## ReactJS
- Read [this](https://code.visualstudio.com/docs/nodejs/reactjs-tutorial)

# Bug fixing
- Sync Update (Ctrl + Alt + U) not working, open terminal and copy paste this command:
    > *chmod +x ~/.vscode/extensions/Shan.code-settings-sync-2.8.2/node_modules/opn/xdg-open*

# Latex
- Read [this](https://www.tug.org/texlive/quickinstall.html)
- Install to ~/ dir
- Fix bug formatter
    ```shell
    sudo perl -MCPAN -e 'install "File::HomeDir"'
    sudo perl -MCPAN -e 'install "Unicode::GCString"'
    ```


# Change log
- Check my commit on Github to track my change

# Contact
- Facebook:  
    > https://www.facebook.com/khanhkiem1211
- Email:  
    > nguyencaominhkhanh@gmail.com*
