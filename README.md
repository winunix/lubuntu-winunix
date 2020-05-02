# Lubuntu WinuniX 20.04 LTS

This is a fork from Lubuntu 20.04 LTS with themes and appearance of Windows System. Its for users that want migrate to a free and open source OS, but don't have technical skills.

## Generating the disc

1. Clone this repository.
2. Download the disc `lubuntu_20.04_lts.iso`.
3. Run the file `./main` without superuser.
4. Select the iso `lubuntu_20.04_lts.iso` in run time of compilation.
5. After the end of process your `iso` will available in cache folder.

## Download the disc

If you don't want to build your own disc, you can download the disc [here](#).

# Style guide for development

The project uses this style guide for better maintenance of system.

## Scaffolding

```
lubuntu-winunix/
├── main            <-- Entrypoint of project, use to generate the disc
├── dependencies    <-- Dependencies of project
├── extract-disk    <-- Source code that extract OS from ISO disc
├── deploy-apps     <-- Source code to deploy apps on chroot environment
├── chroot-env      <-- Source code of virtual environment used to customize the ISO disc
├── pack-disk       <-- Responsable for pack the virtual environment into a new disc
├── reset           <-- Remove folders and files that don't are versioned with git
├── cache/          <-- Temp files (Don't versioned!)
├── disk/           <-- Filesystem from extracted ISO disc (Don't versioned!)

├── modules/        <-- Bibliotecas e Apps do projeto
└── libs/           <-- Bibliotecas de terceiros (não versionado!)
```

## Credits

- *Qt Style* : Thanks to Debian Qt/KDE Maintainers of package `qt5-style-plugin-gtk2` on universe repository.
- *GTK 2/3 Theme* : Thanks to [B00merang Project](https://b00merang.weebly.com/windows-10.html) for Modern flat [theme based on Win10](https://github.com/winunix/lubuntu-win10-theme).
- *OpenBox Theme* : Thanks to [B00merang Project](https://b00merang.weebly.com/windows-10.html) for Modern flat [theme based on Win10](https://github.com/winunix/lubuntu-win10-theme).
- *Icons Theme* : Thanks to [B00merang Project](https://b00merang.weebly.com/icons.html) for [icon theme based on material from Win10](https://github.com/winunix/lubuntu-win10-icon-theme).
- *Cursor Theme* : Thanks fo [David Farkas (srzw)](https://www.gnome-look.org/p/999870/) for [Windows 8 cursors](https://github.com/winunix/lubuntu-win8-cursor-theme).
- *LXQt Theme* : Thanks to [Hendra Mayendra Palembang (hendra)](https://www.pling.com/p/1319223/) for [Panel and bigger start menu](https://github.com/winunix/lubuntu-win10-qt-theme).
- *Font* : Thanks to Debian Fonts Task Force for `DejaVu Sans` font from package `fonts-dejavu-core` on universe repository.
- *SDDM Theme* : Thanks to [Alecsandr Александр  Chelyabinsk (BJIacTeJIuH)](https://store.kde.org/p/1250769/) for [Greeter theme](https://github.com/winunix/sddm-theme-win10).
- Thanks to [Rener (slipttees)](https://github.com/slipttee) for first script (2016) to build remasters.