# Terminal Update Widget

This is a fork of Discover's (formerly known as Muon) notifier plasmoid which you can find [here](https://github.com/KDE/discover/tree/master/notifier/plasmoid). This fork aims to use Ubuntu's ```update-manager``` instead of `plasma-discover --mode update`.  It is named _Terminal update widget_ because it is a fork from a version that used a terminal and ```apt-get``` commands instead. It still needs ```plasma-discover``` to be installed to periodically check for updates in the background.

One will probably want to disable ```update-manager```'s [Phased updates](https://wiki.ubuntu.com/PhasedUpdates) behaviour as it might cause updates reported by Discover not being displayed and installed by update-manager. To do so, add a file in ```/etc/apt/apt.conf.d``` containing ```Update-Manager::Always-Include-Phased-Updates "true";```
