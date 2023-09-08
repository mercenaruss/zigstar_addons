# ZigStar TI CC2652 Flasher Add-on

## Installation

Click on the button below:

[![Open your Home Assistant instance and show the add add-on repository dialog with a specific repository URL pre-filled.](https://my.home-assistant.io/badges/supervisor_add_addon_repository.svg)](https://my.home-assistant.io/redirect/supervisor_add_addon_repository/?repository_url=https%3A%2F%2Fgithub.com%2Fmercenaruss%2Fzigstar_addons)

Or, in your Home Assistant, navigate to _Configuration_ > _Add-ons, Backups & Supervisor_ > _Add-on Store_ > _..._ > _Repositories_ and add `https://github.com/mercenaruss/zigstar_addons` to the list.

1. Navigate in your Home Assistant frontend to **Settings** -> **Add-ons, Backup & Supervisor** -> **Add-on Store**.
2. Find the "ZigStar TI CC2652 FW Flasher" add-on and click it.
3. Click on the "INSTALL" button.

## How to use

The add-on needs a TI CC2652 wireless module accessible through a network
serial port (defined by IP address and port) or other USB-based wireless adapters.

# For Network connected coordinator:
1. In the add-on configuration enter the IP_ADDRESS:port in the Network Device entry form
2. Select any serial device to make the form happy
3. Select to enable the ESPHome trigger of the bootloader for network coordinators.
   (note may not work with all ZigStar  ESPHome firmware versions versions, If not open the coordinator's
   web frontend in a browser and trigger the BSL/Bootloader mode there)
4. Enter in the url for the Z-Stack Firmware - be sure to use the raw GitHub link
   example: https://github.com/Koenkk/Z-Stack-firmware/raw/7398d834eb3a790876c280293c4181da96cc7114/coordinator/Z-Stack_3.x.0/bin/CC1352P2_CC2652P_launchpad_coordinator_20221226.zip
5. Start the add-on.
6. Monitor the flash by going to the addon log page and refreshing periodically.

# For USB Attached Coordinator
1. In the add-on configuration enter some text into the Network Device entry form to make the form happy
2. Select the correct serial device from the list of devices detect, Toggle the switch to enable USB Flash
   (Coordinator must be in bootloader mode before addon is started, hold BSL button while plugging into USB)
3. Enter in the url for the Z-Stack Firmware - be sure to use the raw GitHub link
   example: https://github.com/Koenkk/Z-Stack-firmware/raw/7398d834eb3a790876c280293c4181da96cc7114/coordinator/Z-Stack_3.x.0/bin/CC1352P2_CC2652P_launchpad_coordinator_20221226.zip
4. Start the add-on.
5. Monitor the flash by going to the addon log page, and refreshing periodically.

## Configuration

Add-on configuration:

| Configuration             | Description                                                      |
|---------------------------|------------------------------------------------------------------|
| device                    | Serial service where the Silicon Labs radio is attached          |
| network_device            | Network Serial port (IP_ADDRESS:PORT)                            |
| flow_control              | If hardware flow control should be enabled (depends on firmware) |
| firmware_url (mandatory)  | Custom URL to flash firmware from                                |

## Support

Got questions?

