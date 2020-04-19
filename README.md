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

- Thanks to b00merang project for themes and icons.
- Thanks to Rener(slipttees) for first script (2016) to build remasters.