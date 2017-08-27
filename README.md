# Introduction
This is a tutorial to sync my visual code setting to your visual code

# Requirement
Install this superb extension to your Visual Studio Code for syncing
    - Settings Sync: *https://marketplace.visualstudio.com/items?itemName=Shan.code-settings-sync*

# Download to sync Visual Studio Code setting
**CAUTION** You must pay attention to my guide, especially **step 2**
1. Go to setting sync, scroll down, find and follow his "Download your setting" instruction, using my *Gist ID: c52c1c8bc3a67c165fa630782b61e114*.
1. You may encounter merge conflict in setting.js, I strongly recommend you concat 2 setting.js file (or discard the one that contain only "sync setting").
1. Reload visual code to install synced extension.

# Sync system setting
You may encounter some system requirement for these extension (system library, dependency, etc..). This session will guide you to install them

1. Install clang 3.8
    - sudo apt-get install clang -> install clang
    - sudo apt-get install clang -> check if clang version is 3.8
1. Install cuda driver 375 (or newer) if you have NVIDIA GPU:
    - Run sudo add-apt-repository ppa:graphics-drivers/ppa
    - sudo apt-get update.
    - sudo apt-get install nvidia-375.

Further step is for Python only 

3. Install Anaconda Distribution: *https://www.continuum.io/downloads*

Further step is for using python to program NVIDIA GPU

4. Install CUDA Toolkit 8.0:
    - conda install cudatoolkit

Further step is for using tensorflow-gpu-support

5. Install cuDNN 6:
    - conda install cudnn
1. Install TensorFlow, follow "Installing with Anaconda" section only: *https://www.tensorflow.org/install/install_linux*

# Bug fixing
1. Sync Update (Ctrl + Alt + U) not working, open terminal and copy paste this command:
    - *chmod +x ~/.vscode/extensions/Shan.code-settings-sync-2.8.2/node_modules/opn/xdg-open*

# Contact
*Facebook: https://www.facebook.com/khanhkiem1211*  
*Email: nguyencaominhkhanh@gmail.com*
