## For users

### Install DXVK for Windows games

Wine not packaged on Flathub and until then for running Windows games in Minigalaxy we need to use `com.valvesoftware.Steam.CompatibilityTool.Proton` with some limitations and workarounds. You can use `winetricks` for installing some essentials. To install DXVK for Minigalaxy use the following commands:

```bash
$ flatpak run --command=sh io.github.sharkwouter.Minigalaxy
$ winetricks dxvk
$ exit
```

### Minigalaxy Dev version

Latest Minigalaxy Dev version available in `flathub-beta`. To install:

```bash
$ flatpak remote-add --user flathub-beta https://flathub.org/beta-repo/flathub-beta.flatpakrepo
$ flatpak install --user flathub-beta io.github.sharkwouter.Minigalaxy
```

To run:

```bash
$ flatpak run io.github.sharkwouter.Minigalaxy//beta
```

In some cases for Dev version due to known [bug](https://github.com/flatpak/flatpak/issues/3094) you need to install `org.gnome.Platform.Compat.i386` manually:

```bash
$ flatpak install --user org.gnome.Platform.Compat.i386//41
```

## For maintainers

### Generate 32bit modules

In order to generate 32bit modules run

```
make
```
