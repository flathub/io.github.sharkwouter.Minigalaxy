## For users

### Wine and Minigalaxy

Since 26 Mar 2022 Minigalaxy switched to native Wine Flathub build. Manually installing DXVK no longer needed. WARNING: old Proton prefixes will not work with Wine.

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
$ flatpak install --user org.gnome.Platform.Compat.i386//42
```

## For maintainers

### Generate 32bit modules

In order to generate 32bit modules run

```
make
```
