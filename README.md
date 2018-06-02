# pacman-debloating-list
A simple Bash script to facilitate finding useless packages on Arch Linux.

By default, `pacman -Qe` only displays a plain list of installed packages. In contrast, this script:
* Displays a table with all explicitly installed packages, along with their groups and descriptions.
* If all packages in a group are installed, it will only show a single row representing the group.

This significantly increments the signal:noise ratio, by reducing the mental effort of checking packages with obscure names or the packages belonging to common package groups (base, base-devel, xfce4, etc.)

# Requirements / dependencies

The `expac` package is required. Otherwise, there are no requirements or dependencies outside of a basic Arch Linux install.

# One time usage

If you want to use it one time, just copy and paste the contents of the file `pacman-debloating-list` to your terminal.

# Installation

To install it permanently, run in a terminal window:
```
curl https://raw.githubusercontent.com/joanbm/pacman-debloating-list/master/pacman-debloating-list --output pacman-debloating-list
# If you want to verify the contents of the script for malicious code, here's your last chance...
chmod +x pacman-debloating-list
sudo mv pacman-debloating-list /usr/bin/pacman-debloating-list # Or run as root with if you don't have sudo
```

Then, run the following command in a terminal window to execute it whenever you want:
```pacman-debloating-list```

# Sample output
```
(ALL)                            base             (All packages in the group are installed)
(ALL)                            base-devel       (All packages in the group are installed)
(ALL)                            texlive-most     (All packages in the group are installed)
(ALL)                            xfce4            (All packages in the group are installed)
aircrack-ng                                       Key cracker for the 802.11 WEP and WPA-PSK protocols
alsa-utils                                        An alternative implementation of Linux sound support
broadcom-wl-dkms                                  Broadcom 802.11 Linux STA wireless driver
catfish                                           Versatile file searching tool
cdrtools                                          Original cdrtools supporting CD, DVD and BluRay burning
chromium                                          A web browser built for speed, simplicity, and security
create_ap                                         A shell script to create a NATed/Bridged Software Access Point
cups                                              The CUPS Printing System - daemon package
dconf-editor                     gnome-extra      dconf Editor
dosfstools                                        DOS filesystem utilities
evince                           gnome            Document viewer (PDF, Postscript, djvu, tiff, dvi, XPS, SyncTex support with gedi>
[...]
xorg-xinput                      xorg-apps  xorg  Small commandline tool to configure devices
xpdf                                              Viewer for Portable Document Format (PDF) files
xsane                                             A GTK-based X11 frontend for SANE and plugin for Gimp.
xscreensaver                                      Screen saver and locker for the X Window System
youtube-dl                                        A small command-line program to download videos from YouTube.com and a few more sites
```
