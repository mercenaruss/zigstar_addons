# ZigStar TI CC2652P7 Flasher Add-on

## Installation

Click on the button below:

[![Open your Home Assistant instance and show the add add-on repository dialog with a specific repository URL pre-filled.](https://my.home-assistant.io/badges/supervisor_add_addon_repository.svg)](https://my.home-assistant.io/redirect/supervisor_add_addon_repository/?repository_url=https%3A%2F%2Fgithub.com%2Fmercenaruss%2Fzigstar_addons)

Or, in your Home Assistant, navigate to _Configuration_ > _Add-ons, Backups & Supervisor_ > _Add-on Store_ > _..._ > _Repositories_ and add to the list.

```txt
https://github.com/mercenaruss/zigstar_addons
```

1. Navigate in your Home Assistant frontend to **Settings** -> **Add-ons, Backup & Supervisor** -> **Add-on Store**.
2. Find the "ZigStar TI CC2652P7 FW Flasher" add-on and click it.
3. Click on the "INSTALL" button.

## How to use

The add-on needs a TI CC2652P7 wireless module accessible through a network
serial port (defined by IP address and port) or other USB-based wireless adapters.

# For flashing over Network:

1. In the add-on configuration enter the IP_ADDRESS:port in the Network Device entry form
2. Select any serial device to make the form happy
3. Disable USB flashing
4. Select to enable the BSL trigger of the bootloader for network coordinators.
5. **Enable required firmware toggle** or enter the url for the Z-Stack Firmware - be sure to use the raw GitHub link
   example: [copy](https://github.com/Koenkk/Z-Stack-firmware/raw/7398d834eb3a790876c280293c4181da96cc7114/coordinator/Z-Stack_3.x.0/bin/CC1352P2_CC2652P_launchpad_coordinator_20221226.zip)
6. Start the add-on.
7. Flashing procedure will take 5-6 minutes for network devices
8. Monitor the flash by going to the addon log page and refreshing periodically.

# For flashing over USB:

1. In the add-on configuration enter some text into the Network Device entry form to make the form happy
2. Select the correct serial device from the list of devices detect, Toggle the switch to enable USB Flash on UZG-01
   (UZG-01 must be in bootloader mode before addon is started - HOLD 4-8 sec Control button to Enable BSL mode)
3. **Enable required firmware toggle** or enter the url for the Z-Stack Firmware - be sure to use the raw GitHub link
   example: [copy](https://github.com/Koenkk/Z-Stack-firmware/raw/7398d834eb3a790876c280293c4181da96cc7114/coordinator/Z-Stack_3.x.0/bin/CC1352P2_CC2652P_launchpad_coordinator_20221226.zip)
4. Start the add-on.
5. Monitor the flash procedure by going to the addon log page, and refreshing periodically.

## Configuration

Add-on configuration:

| Configuration           | Description                                   |
| ----------------------- | --------------------------------------------- |
| device                  | Serial service where the TI radio is attached |
| network_device          | Network Serial port (IP_ADDRESS:PORT)         |
| firmware_url (optional) | Custom URL to flash firmware from             |

## Support

Got questions?

```

```
