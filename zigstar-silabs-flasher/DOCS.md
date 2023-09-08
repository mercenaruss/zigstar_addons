# ZigStar Add-on: Silicon Labs Flasher Add-on

## Installation

Click on the button below:

[![Open your Home Assistant instance and show the add add-on repository dialog with a specific repository URL pre-filled.](https://my.home-assistant.io/badges/supervisor_add_addon_repository.svg)](https://my.home-assistant.io/redirect/supervisor_add_addon_repository/?repository_url=https%3A%2F%2Fgithub.com%2Fmercenaruss%2Fzigstar_addons)

Or, in your Home Assistant, navigate to _Configuration_ > _Add-ons, Backups & Supervisor_ > _Add-on Store_ > _..._ > _Repositories_ and add `https://github.com/mercenaruss/zigstar_addons` to the list.

1. Navigate in your Home Assistant frontend to **Settings** -> **Add-ons, Backup & Supervisor** -> **Add-on Store**.
2. Find the "ZigStar Silicon Labs FW Flasher" add-on and click it.
3. Click on the "INSTALL" button.

## How to use

The add-on needs a Silicon Labs based wireless module accessible through a network
serial port defined by IP addres and port or other USB based wireless adapters.

*Disable ZHA or Z2M*

# For Network connected coordinator:
1. In the add-on configuration enter the IP_ADDRESS:port in the Network Device entry form
2. Select any serial device to make the form happy
3. Paste the link the the firmware .GBL file to be used for the update and press `Save`.
4. Start the add-on.
5. Monitor the flash by going to the addon log page, and refreshing periodically.

# For USB Attaced Coordinator
1. In the add-on configuratione enter some text into the Network Device entry form to kmake the form happy
2. Select the correct serial device from the list of devices detect, Toggle the switch to enable USB Flash
3. Paste the link the the firmware .GBL file to be used for the update and press `Save`.
4. Start the add-on.
5. Monitor the flash by going to the addon log page, and refreshing periodically.



## Configuration

Add-on configuration:

| Configuration      | Description                                            |
|--------------------|--------------------------------------------------------|
| device             | Serial service where the Silicon Labs radio is attached |
| network_device     | Network Serial port (IP_ADDRESS:PORT)   
| baudrate           | Serial port baudrate (depends on firmware)   |
| flow_control       | If hardware flow control should be enabled (depends on firmware) |
| firmware_url       | Custom URL to flash firmware from                      |

## Support


