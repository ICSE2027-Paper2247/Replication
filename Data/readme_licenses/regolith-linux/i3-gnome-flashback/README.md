# i3-gnome-flashback [![LICENSE](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)

Allows you to use i3 in a GNOME-Flashback session. Large parts of this are based on the existing [`i3-gnome`](https://github.com/lvillani/i3-gnome) project.

This has been tested working on GNOME version **40**.

# Installation

For Arch users see the [AUR package](https://aur.archlinux.org/packages/i3-gnome-flashback/) for a more easy intallation.

For Ubuntu (19.10), ensure prerequisites are installed:

```
sudo apt install i3 gnome-flashback build-essential
```

Then install i3-gnome-flashback:

```
sudo make install
```

For other distributions, clone this repository and run `make install` with root privileges.

# Notes

To understand how the files in this repo work to initialize an i3 and GNOME session, refer to this [GNOME wiki](https://wiki.gnome.org/Projects/SessionManagement/RequiredComponents) on session management.

The default session for `i3-GNOME-Flashback` installs a set of configuration defaults for GSettings/dconf, e.g.:

  - Desktop icon handling is disabled for GNOME Flashback, due to incompatibilities with i3, and control of the root window is instead given to `gnome-control-center`, which handles setting the user-defined wallpaper, among other things.

  - Window buttons for minimize and maximize have been removed, leaving only the close button, as the former are ineffectual in i3.

Setup for these configuration defaults is handled via GSettings overrides, which are described in
further detail
[here](https://help.gnome.org/admin/system-admin-guide/stable/dconf-custom-defaults.html.en) and
[here](https://help.gnome.org/admin/system-admin-guide/stable/overrides.html.en).
