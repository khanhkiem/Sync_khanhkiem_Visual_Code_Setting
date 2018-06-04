# Log in as root
http://www.configserverfirewall.com/ubuntu-linux/enable-ubuntu-desktop-root-login/

# Background
1. Download [this](https://drive.google.com/open?id=0B0GZEBA9RrHnRVZESXVwVXNtNTQ)

# Google chrome
1. Account nguyencaominhkhanh@gmail.com

# Unity Tweak Tool
1. Install following [this](http://ask.xmodulo.com/install-unity-tweak-tool-ubuntu-desktop.html):
    ```shell
    sudo apt-get install unity-tweak-tool
    ```
1. Download this [Ark theme](http://www.omgubuntu.co.uk/2016/06/install-latest-arc-gtk-theme-ubuntu-16-04):
    ```shell
    sudo sh -c "echo 'deb http://download.opensuse.org/repositories/home:/Horst3180/xUbuntu_16.04/ /' >> /etc/apt/sources.list.d/arc-theme.list"
    sudo apt-get update && sudo apt-get install arc-theme
    ```
1. Open Unity Tweak Tool
1. Select Overview -> Window Manager -> Window Snapping
1. Config for yourself
1. Select Overview -> Apeearence -> Theme -> Ark-dark

# Unikey
1. Install unikey, using this [tutorial](https://nguyenhuuhoang.com/huong-dan-cai-bo-go-tieng-viet-tren-ubuntu-16-04-lts-ibus-unikey/):
    ```shell
    sudo apt-get install ibus-unikey
    ibus restart
    ```

# Github 
1. Install Git
    ```shell
    sudo apt-get install git  
    ```
1. Create SSH key following this [tutorial](https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/)
1. Git config:
    ```shell
    git config --global user.email buidoigiauco@gmail.com  
    git config --global user.name khanhkiem
    ```

# Postgres
```shell
sudo apt-get install postgresql pgadmin3
sudo -u postgres createuser --interactive
createdb khanhcao
psql
\password khanhcao 
```

# Bluetooth off on startup
```shell
sudo gedit /etc/rc.local
```

Add this line before exit 0
```shell
rfkill block bluetooth
```

## NVIDIA    
- Download nvidia driver, cudatoolkit, cudnn from nvidia homepage
- Ctrl + Alt + F1
- cd to driver.run dir
    ```shell
    sudo service lightdm stop
    sudo init 3
    sudo ./driver.run --no-opengl-files
    ```
- cd to cudatoolkit.deb dir
    '''shell
    sudo dpkg -i ./cuda-repo-..
    sudo apt-key add /var/cuda-repo.../7fa2af80.pub
    sudo apt-get update
    sudo apt-get install cuda-toolkit-...
    '''
- cd to libcudnn.deb dir
    '''shell
    sudo dpkg -i ./libcudnn-...
    '''
