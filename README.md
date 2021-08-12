# anaconda-installation-ubuntu20.04

This repository includes an installation document for Anaconda on Ubuntu 20.04.

## 1. Download Anaconda 

Create a directory to download the Anaconda Installation file. \(Optional\)

```text
mkdir downloads 
cd downloads
```

Find the latest version of Anaconda from the xxx site before running the code. Change the link if there is a new version. 

```text
wget https://repo.anaconda.com/archive/Anaconda3-2021.05-Linux-x86_64.sh
```

#### Find Download Link

The link of the installer of the relevant operating system can be found as follows.

![](.gitbook/assets/image%20%283%29.png)

## 2. Edit File Permissions

To be able to run anaconda3-xxx.sh you need to give users execute permission.

```text
sudo chmod +x Anaconda3-2021.05-Linux-x86_64.sh
```

You need to change the owner of the directory you choose for Anaconda installation or you can give your user permissions on this directory. The directory chosen for our case is "/data" and the directory's owner has been changed.

```text
sudo chown -R hfdeniz:hfdeniz /data
```

## 3. Installing Anaconda

Go to the download directory and run Anaconda-xxx-xxx.sh file.

```text
cd downloads
./Anaconda3-2021.05-Linux-x86_64.sh
```

* To accept the agreement, press Enter until the directory is asked.
* It will suggest you an installation directory, you can change it. In our case, I typed "/data/anaconda3" as the install directory.
* Finally, it will ask you, whether you want to run initialize or not. You can type YES.

You need to source .bashrc file after installation.

```text
source ./bashrc
```

If the base conda environment automatically is opened, installation complete!



