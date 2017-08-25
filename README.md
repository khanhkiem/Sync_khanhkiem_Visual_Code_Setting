# Introduction
This is a tutorial to sync my visual code setting to your visual code

# Requirement
1. Install this superb extension to your Visual Studio Code for syncing
- Settings Sync: *https://marketplace.visualstudio.com/items?itemName=Shan.code-settings-sync*
1. Install clang 3.8
- sudo apt-get install clang -> install clang
- sudo apt-get install clang -> check if clang version is 3.8

# Download setting
1. Go to setting sync, scroll down, find and follow his "Download your setting" instruction, using my *Gist ID: c52c1c8bc3a67c165fa630782b61e114*.
1. You may encounter merge conflict in setting.js, I strongly recommend you concat 2 setting.js file (or discard the one that contain only "sync setting").
1. Reload visual code to install synced extension.

# Bug fixing
- Sync Update (Ctrl + Alt + U) not working, open terminal and copy paste this command:  
*chmod +x ~/.vscode/extensions/Shan.code-settings-sync-2.8.2/node_modules/opn/xdg-open*

# Contact
*Facebook: https://www.facebook.com/khanhkiem1211*  
*Email: nguyencaominhkhanh@gmail.com*