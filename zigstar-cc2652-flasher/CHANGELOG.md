# Changelog

## 0.4.2

- Download firmware with `curl --fail`, retries and timeouts over HTTPS only; exit with an error instead of reporting success when it fails
- Quote shell variables and use a temporary working directory
- Add optional IEEE address writing (`write_ieee`, `ieee`)
- Move base image to Python 3.13 / Alpine 3.22
- Use firmware from the TubesZB repository (20250321 builds, pinned commit) with SHA256 verification
- Mark add-on as stable
- Add AppArmor profile
- Fix repository links (`main` branch) and documentation

## 0.4.1

- Minor upgrade

## 0.4.0

- Increased the chip flashing speed by 5 to 10 times compared to previous versions

## 0.3.0

- Add CC2652P7 firmware toggle for UZG-01 v0.2 and up.
- Add CC2652P Others firmware toggle. Used in Ebyte Modules.

## 0.2.6

- Add firmware firmware description

## 0.2.5

- Fix Ukrainian language code

## 0.2.4

- Add TubesZB support
- Add Russian translation
- Add Ukrainian translation
- Change BSL Timer

## 0.2.3

- Fix bootloader mode for Sonoff ZBDongle-P

## 0.2.2

- Add support for Sonoff ZBDongle-P

## 0.2.1

- Fix addon link

## 0.2.0

- Added option for last KoenK firmware
- Removed flow_control
- Adjusted BSL mode for ZigStar Ethernet Devices
- Changed option descriptions

## 0.1.0

- Initial version release
