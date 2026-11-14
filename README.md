# bojanowski.me Flatpak repository

This repository hosts the Flatpak repository for apps by Tomasz Bojanowski,
published with GitHub Pages at <https://flatpak.bojanowski.me/>:

- [Vumi](https://github.com/TomaszBojanowski/vumi), a GNOME music player for
  your own Navidrome or Subsonic server;
- [openExpress](https://github.com/TomaszBojanowski/openExpress), an unofficial
  Garmin Express client for Linux;
- [Baseboard](https://github.com/TomaszBojanowski/baseboard), a native GNOME
  app for the sensors and fans of MSI motherboards on Linux.

For source code, issues and documentation, see the repositories of the apps.

## Installation

Vumi:

```sh
flatpak install --user https://flatpak.bojanowski.me/io.github.tomaszbojanowski.Vumi.flatpakref
```

openExpress:

```sh
flatpak remote-add --user --if-not-exists flathub https://dl.flathub.org/repo/flathub.flatpakrepo
flatpak remote-add --user --if-not-exists bojanowski https://flatpak.bojanowski.me/bojanowski.flatpakrepo
flatpak install --user bojanowski io.github.tomaszbojanowski.OpenExpress
```

Baseboard:

```sh
flatpak install --user https://flatpak.bojanowski.me/me.bojanowski.Baseboard.flatpakref
```

`openexpress.flatpakrepo` stays for installations that added the repository
under the name `openexpress`: it is the same repository.

Updates arrive through a regular `flatpak update`. The GNOME runtime comes
from Flathub.

The repository is signed with the key
`2EEA A178 A4C8 C394 74DA 5D97 5A17 0A42 2BEA C494`, also in `bojanowski.gpg`
(and `openexpress.gpg`, the same key).

## Trademarks

MSI and MSI product names are trademarks of Micro-Star International Co.,
Ltd. Baseboard is an independent project and is not affiliated with or
endorsed by MSI.
