+++
title = 'How to change Ubuntu UI to MacOS-themed'
date = 2024-01-27T18:06:30-05:00
draft = false
+++

In this blog, I will show how to change Ubuntu UI to MacOS alike. Ubuntu is great for work and productivity, but its UI is very basic. Luckily, thanks to the community, there are tools that can tweak Ubuntu UI to look like MacOS. Here is an example of the end result:

![](./images/desktop.png)

First, we need to install `gnome-tweaks` and `gnome-shell-extension-manager`:

```sh
sudo apt install gnome-tweaks gnome-shell-extension-manager
```

Next, clone the [WhiteSur-gtk-theme](https://github.com/vinceliuice/WhiteSur-gtk-theme) repo, open the repo and run the installation script:

```sh
./install.sh -m -t all -l -c Dark -N stable --normal --round -i ubuntu
```

Once it is done, it is time to run the tweaks script:

```sh
sudo ./tweaks.sh -g
sudo ./tweaks.sh -f
```

The next step is to install MacOS Icon pack from [https://www.gnome-look.org/p/2023325](https://www.gnome-look.org/p/2023325). Once downloaded, go to your home directory and create a `.icon` folder and move the downloaded icon packs into the folder. You can press `ctrl+h` to view hidden folders in the file browser.

![](./images/icon.png)
![](./images/icon-1.png)

Now, let's customize the UI by installing a few extensions. Open `Gnome Extensions Manager`:
![](./images/extension-1.png)
![](./images/extension-2.png)

Install `blur my shell` and `user themes`:
![](./images/blur-my-shell.png)
![](./images/user-themes.png)

Open the tweaks app from the app browser and make the following changes:
![](./images/tweaks.png)
![](./images/tweaks-1.png)

From here, you can play around with different settings in tweaks and customize it.

Finally, you can dowload MacOS wallpapers here: [https://512pixels.net/projects/default-mac-wallpapers-in-5k/](https://512pixels.net/projects/default-mac-wallpapers-in-5k/).
