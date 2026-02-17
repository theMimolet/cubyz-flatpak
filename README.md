# Unofficial Cubyz Flatpak

Unofficial Flatpak packaging of [Cubyz](https://github.com/PixelGuys/Cubyz), an open-world voxel game.

> [!NOTE]
> Cubyz is made by [PixelGuys](https://github.com/PixelGuys). The official releases can be found [here](https://github.com/PixelGuys/Cubyz/releases).

## Installation

This repo is still experimental and may change at any time.

It can be taken down at any time if there are any issues with it existing.

Here are the commands to install it :
```sh
# Add the repository
flatpak remote-add --user --no-gpg-verify cubyz-flatpak https://raw.githack.com/theMimolet/cubyz-flatpak/gh-pages/

# Install Cubyz
flatpak install cubyz-flatpak io.github.pixelguys.Cubyz
```

## Data Location

Game data (saves, configuration) is stored in:
```
~/.var/app/io.github.pixelguys.Cubyz/.cubyz/
```

## Known Issues

- **Logs folder**: Due to Flatpak's immutable sandbox, the logs folder cannot be created in the game directory. This doesn't affect gameplay, and logs are still visible when running from the terminal with `flatpak run io.github.pixelguys.Cubyz`.