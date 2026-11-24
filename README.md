# ZigStar Home Assistant add-on repository

![Supports aarch64 Architecture][aarch64-shield]
![Supports amd64 Architecture][amd64-shield]

Add-ons for Home Assistant that allow you to easily flash new firmware on your ZigStar Coordinators

[![Open your Home Assistant instance and show the add add-on repository dialog with a specific repository URL pre-filled.](https://my.home-assistant.io/badges/supervisor_add_addon_repository.svg)](https://my.home-assistant.io/redirect/supervisor_add_addon_repository/?repository_url=https%3A%2F%2Fgithub.com%2Fmercenaruss%2Fzigstar_addons)

## Supported architectures

The add-ons are built for `amd64` and `aarch64`. The deprecated `armhf`, `armv7` and `i386` architectures are no longer supported.

## Add-ons

This repository contains the following add-ons:

- **[ZigStar TI CC2652 FW Flasher](https://github.com/mercenaruss/zigstar_addons/tree/main/zigstar-cc2652-flasher/README.md)**

  Flash FW to ZigStar TI CC2652 based Coordinators

- **[ZigStar TI CC2652P7 FW Flasher](https://github.com/mercenaruss/zigstar_addons/tree/main/zigstar-cc2652p7-flasher/README.md)**

  Flash FW to ZigStar TI CC2652P7 based Coordinators (UZG-01 v0.2 and up)

- **[ZigStar Silicon Labs FW Flasher](https://github.com/mercenaruss/zigstar_addons/tree/main/zigstar-silabs-flasher/README.md)**

  Flash FW to ZigStar SiliconLabs EFR32 based Coordinators

## Installation

Adding this add-ons repository to your Home Assistant instance is pretty easy. In the
Home Assistant add-on store, a possibility to add a repository is provided.

Use the following URL to add this repository:

```txt
https://github.com/mercenaruss/zigstar_addons
```

## Contribute

You can contribute to the repo by

- Providing Pull Requests (Features, Proof of Concepts or Fixes)
- Testing newly released features and reporting issues
- Contributing on documentation

## Credits

Special thanks goes to all authors of 3rd party libraries which are used in these add-ons:

- [beagleconnect / cc1352 flasher](https://git.beagleboard.org/beagleconnect/cc1352-flasher)
- [JelmerT / cc2538-bsl](https://github.com/JelmerT/cc2538-bsl)

People helping to keep the show on the road - **developers and contributors**:

- [@tube0013](https://github.com/tube0013) for initial CC2652 addon release
- [@home-assistant](https://github.com/home-assistant) for initial release of Silicon Labs Flasher

[aarch64-shield]: https://img.shields.io/badge/aarch64-yes-green.svg
[amd64-shield]: https://img.shields.io/badge/amd64-yes-green.svg
