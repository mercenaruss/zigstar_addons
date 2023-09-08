# ZigStar Home Assistant add-on repository

![Supports aarch64 Architecture][aarch64-shield]
![Supports amd64 Architecture][amd64-shield]
![Supports armhf Architecture][armhf-shield]
![Supports armv7 Architecture][armv7-shield]
![Supports i386 Architecture][i386-shield]

Addon-ons for Home Assistant that allow you to easily flash new firmware on your ZigStar Coordinators

[![Open your Home Assistant instance and show the add add-on repository dialog with a specific repository URL pre-filled.](https://my.home-assistant.io/badges/supervisor_add_addon_repository.svg)](https://my.home-assistant.io/redirect/supervisor_add_addon_repository/?repository_url=https%3A%2F%2Fgithub.com%2Fmercenaruss%2Fzigstar_addons)

## Add-ons

This repository contains the following add-ons:

- **[ZigStar TI CC2652 FW Flasher](https://github.com/mercenaruss/zigstar_addons/tree/main/zigstar-cc2652-flasher/README.md)**

  Flash FW to ZigStar TI CC2652 based Coordinators

- **[ZigStar Silicon Labs FW Flasher](/https://github.com/mercenaruss/zigstar_addons/tree/main/zigstar-silabs-flasher/README.md)**

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

Special thanks goes to all authors of 3rd party libraries which are used in this addons:

- [beagleconnect / cc1352 flasher](https://git.beagleboard.org/beagleconnect/cc1352-flasher)
- [JelmerT / cc2538-bsl](https://github.com/JelmerT/cc2538-bsl)

People helping to keep the show on the road - **developers and contributors**:

- [@tube0013](https://github.com/tube0013) for initial CC2652 addon release
- [@home-assistant](https://github.com/home-assistant) for initial release of Silicon Labs Flasher

[aarch64-shield]: https://img.shields.io/badge/aarch64-yes-green.svg
[amd64-shield]: https://img.shields.io/badge/amd64-yes-green.svg
[armhf-shield]: https://img.shields.io/badge/armhf-yes-green.svg
[armv7-shield]: https://img.shields.io/badge/armv7-yes-green.svg
[i386-shield]: https://img.shields.io/badge/i386-yes-green.svg
