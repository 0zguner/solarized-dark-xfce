Numix Solarized is a is a modern flat theme with a combination of light and dark elements. It supports Gnome, Unity, XFCE and Openbox. It is based on the Numix theme by Satyajit Sahoo (satyajit.happy@gmail.com).


### Manual installation

Extract the zip file to the themes directory i.e. `/usr/share/themes/`

To set the theme in Gnome, run the following commands in Terminal,

```
gsettings set org.gnome.desktop.interface gtk-theme "Numix"
gsettings set org.gnome.desktop.wm.preferences theme "Numix"
```

To set the theme in Xfce, run the following commands in Terminal,

```
xfconf-query -c xsettings -p /Net/ThemeName -s "Numix"
xfconf-query -c xfwm4 -p /general/theme -s "Numix"
```

### Requirements

GTK+ 3.6 or above

Murrine theme engine

### Code and license

License: GPL-3.0+
