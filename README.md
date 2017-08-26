# Introduction
This is a tutorial to sync my visual code setting to your visual code

# Requirement
1. Install this superb extension to your Visual Studio Code for syncing
    - Settings Sync: *https://marketplace.visualstudio.com/items?itemName=Shan.code-settings-sync*
1. Install clang 3.8
    - sudo apt-get install clang -> install clang
    - sudo apt-get install clang -> check if clang version is 3.8
1. Python only:  
    1. Install cuda driver (current version is 384.69):
        - Download: *http://www.nvidia.com/Download/index.aspx?lang=en-us*
        - Install: *https://askubuntu.com/questions/149206/how-to-install-nvidia-run*
    1. Install Anaconda Distribution: *https://www.continuum.io/downloads*
    1. Install cudaToolkit: 
        - conda install cudatoolkit
# Download setting
**CAUTION** You must pay attention to my guide, especially **step 2**
1. Go to setting sync, scroll down, find and follow his "Download your setting" instruction, using my *Gist ID: c52c1c8bc3a67c165fa630782b61e114*.
1. You may encounter merge conflict in setting.js, I strongly recommend you concat 2 setting.js file (or discard the one that contain only "sync setting").
1. Reload visual code to install synced extension.
# Bug fixing
1. Sync Update (Ctrl + Alt + U) not working, open terminal and copy paste this command:
    - *chmod +x ~/.vscode/extensions/Shan.code-settings-sync-2.8.2/node_modules/opn/xdg-open*

# Contact
*Facebook: https://www.facebook.com/khanhkiem1211*  
*Email: nguyencaominhkhanh@gmail.com*
