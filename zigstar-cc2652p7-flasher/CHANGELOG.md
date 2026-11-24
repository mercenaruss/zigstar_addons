# Changelog

## 0.2.1

- Download firmware with `curl --fail`, retries and timeouts over HTTPS only; exit with an error instead of reporting success when it fails
- Quote shell variables and use a temporary working directory
- Add optional `baudrate` setting for modules wired directly to a UART
- Add optional IEEE address writing (`write_ieee`, `ieee`)
- Move base image to Python 3.13 / Alpine 3.22
- Use firmware from the TubesZB repository (20250321 builds, pinned commit) with SHA256 verification
- Add AppArmor profile
- **Breaking:** the `armhf`, `armv7` and `i386` architectures are no longer supported; only `amd64` and `aarch64` are built
- Move base image into the Dockerfile
- Fix "Missing required option" when saving a network-only configuration (no default `null` options)
- Fix repository links (`main` branch) and documentation

## 0.2.0

- Increased the chip flashing speed by 5 to 10 times compared to previous versions

## 0.1.0

- Initial addon release
