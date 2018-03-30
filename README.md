# pacman-debloating-list
An extremely simple Bash script to facilitate finding useless packages on Arch Linux.

It displays, in a table, all packages (excluding those on the base and base-devel groups), along with their groups and descriptions.

# Requirements / dependencies

No requirements or dependencies outside of a basic Arch Linux install.

# Installation

Run in a terminal window:
```
curl https://raw.githubusercontent.com/joanbm/pacman-debloating-list/master/pacman-debloating-list --output pacman-debloating-list
# If you want to verify the contents of the script for malicious code, here's your last chance...
chmod +x pacman-debloating-list
sudo mv pacman-debloating-list /usr/bin/pacman-debloating-list
```

# Usage

Run in a terminal window:
```
pacman-debloating-list
```

# Sample output
```
aircrack-ng                                       Key cracker for the 802.11 WEP and WPA-PSK protocols
alsa-utils                                        An alternative implementation of Linux sound support
autofs                                            A kernel-based automounter for Linux.
broadcom-wl-dkms                                  Broadcom 802.11 Linux STA wireless driver
catfish                                           Versatile file searching tool
cdrtools                                          Original cdrtools supporting CD, DVD and BluRay burning
create_ap                                         A shell script to create a NATed/Bridged Software Access Point
cups                                              The CUPS Printing System - daemon package
dialog                                            A tool to display dialog boxes from shell scripts
dosfstools                                        DOS filesystem utilities
evince                           gnome            Document viewer (PDF, Postscript, djvu, tiff, dvi, XPS, SyncTex support with gedit, comics books (cbr,cbz,cb7 and cbt))
exo                              xfce4            Extensions to Xfce by os-cillation
file-roller                      gnome            Create and modify archives
filezilla                                         Fast and reliable FTP, FTPS and SFTP client
[...]
xfwm4-themes                     xfce4            A set of additional themes for the Xfce window manager
xorg-xinput                      xorg-apps  xorg  Small commandline tool to configure devices
xpdf                                              Viewer for Portable Document Format (PDF) files
xsane                                             A GTK-based X11 frontend for SANE and plugin for Gimp.
xscreensaver                                      Screen saver and locker for the X Window System
youtube-dl                                        A small command-line program to download videos from YouTube.com and a few more sites
```
