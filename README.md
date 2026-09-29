# hoppscotch-bin

Arch Linux package for the [Hoppscotch](https://hoppscotch.io) desktop app, repackaged from the upstream `.deb` in [hoppscotch/releases](https://github.com/hoppscotch/releases/releases).

## Install

```sh
git clone https://github.com/<user>/hoppscotch-bin.git
cd hoppscotch-bin
makepkg -si
```

## Update

```sh
git pull
makepkg -si
```

## Uninstall

```sh
sudo pacman -Rns hoppscotch-bin
```

## Dependencies

- `webkit2gtk-4.1`
- `gtk3`

## Automation

`.github/workflows/update.yml` checks upstream daily, bumps `_tag`, resets `pkgrel`, regenerates `sha256sums` and `.SRCINFO`, and commits the change.
