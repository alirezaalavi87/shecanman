How this fork differs from upstream:
- Add compatibility with NetworkManager
- Fix issue with running with `sudo` by copying to `usr/sbin`
- Rewrite in `sh` so it is portable across systems without `bash`

# ShecanMan

A simple lightweight utility script to use [Shecan](https://www.shecan.ir) DNS servers temporarily on Linux.

![screenshot](screenshots/Screenshot-v0.1.2.png)

## Download

Download the latest version as below:

```shell script
git clone https://github.com/alirezaalavi87/shecanman.git
cd shecanman
chmod +x shecanman
```

## Installation

**Installation is optional**, but lets ShecanMan to be accessible from everywhere:

```shell script
sudo sh shecanman install
```

If you don't want to access ShecanMan system-wide, you can continue using it locally.

## Usage

ShecanMan lets you switch on/off Shecan.ir DNS configs temporarily on linux.

Usage: `shecanman [command]`

Commands:

- `on` - Switch on Shecan DNS configs; keeps a backup of current configs.
- `off` - Switch off Shecan DNS; This will restore previous DNS configs.
- `status` - Show current status; Check whether ShecanMan is on.
- `install` - Install ShecanMan system-wide, so you can call it everywhere.
- `uninstall` - Uninstall ShecanMan, so that it's longer accessible system-wide.
- `version` - Show ShecanMan version.
- `help` - Show help.

## Disclaimer

I have nothing to do with [Shecan](https://www.shecan.ir) team!
