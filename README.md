# Lux HUD

Lux HUD is a collection of [Conky](https://github.com/brndnmtthws/conky) configs that gives you an almost complete system monitoring.

<<<<<<< HEAD
![lux-hud conky configs](https://cdn.pling.com/img/f/2/d/e/82330eecff87f62ccea993d5d50e0626fae2.png)
=======
[![lux-hud conky configs](https://raw.githubusercontent.com/luxwarp/lux-hud/master/screenshot.png)](https://raw.githubusercontent.com/luxwarp/lux-hud/master/screenshot.png)
>>>>>>> development

## Features

-   System info
-   Battery status
-   CPU
-   Memory
-   Disk
-   Network
-   Processes
-   Journal log
-   Time / Calendar

## Requirements

-   Linux
-   [conky >= 1.11](https://github.com/brndnmtthws/conky)
-   Cutive Mono font
    -   [Google fonts](https://fonts.google.com/specimen/Cutive+Mono)
    -   [1001 Free font](https://www.1001freefonts.com/cutive-mono.font)

## Usage

Make sure you have conky and the Cutive Mono font installed on your system.

Download compressed files or use git clone.

```shell
git clone https://github.com/luxwarp/lux-hud.git
```

Place the cloned or uncompressed lux-hud folder inside

`~/.config/conky`

**example of correct file path**

`/home/username/.config/conky/lux-hud/` (all files inside here.)

Go through all .conf files and make sure your own device names are correct like disks / mount points / network interfaces etc. You do need to have some knowledge about how conky works so check out [conky wiki](https://github.com/brndnmtthws/conky/wiki)

Execute the `startall.sh` file in your terminal to run all widgets at once, or use `conky -c /path/to/configfile.conf` command to only launch the one you want, see the `startall.sh` file for how the script loads all conf files.

This collection is developed for a screen resolution of 1920x1080px. So feel free to customize all widgets to fit your screen if they aren't positioned correctly for you.

See [conky wiki](https://github.com/brndnmtthws/conky/wiki) for more information about how to work with conky configurations (widgets)

The background in the screenshot can be found [here](https://pixabay.com/sv/photos/forest-vattenfall-bach-mossa-4068618/)

## FAQ

**Why is all widgets in it's own file?**

Mainly because it's easier to position them on the desktop.  
How ever the bad thing about this is that it requires to run  
multiple conky processes.

**How do I make Lux HUD autostart on boot/login?**

Look up how to create an autostart script on your distribution.  
But most distributions that follows the [FreeDesktop spec](https://www.freedesktop.org/wiki/Specifications/) allows you to create a .desktop file in `~/.config/autostart/` for ex

`~/.config/autostart/luxhud.desktop`

```plaintext
[Desktop Entry]
Name=luxhud
Comment=A complete system monitoring running with conky.
Exec=/home/username/.config/conky/lux-hud/startall.sh
Terminal=false
Type=Application
```

**How do I customize the widgets in Lux HUD?**

Just edit the conf file you want to customize and save. If conky  
is already running the conf file you edit it should update without  
a restart of conky. See [conky wiki](https://github.com/brndnmtthws/conky/wiki) and `man conky` pages for more information  
on what you can do with conky.

**My question is not answered here!**

Feel free to contact me on email mikael.m.carlsson@gmail.com or create an [issue on github](https://github.com/luxwarp/lux-hud/issues).

## License

ISC © 2021 [Mikael Luxwarp Carlsson](https://connumin.com)

## Note

Feel free to contribute the way you want.
