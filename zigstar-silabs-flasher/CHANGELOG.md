# Changelog

## 0.1.2

- Download firmware with `curl --fail`, retries and timeouts over HTTPS only; exit with an error instead of reporting success when it fails
- Quote shell variables and use a temporary working directory
- Move base image to Python 3.13 / Alpine 3.22
- Add Russian and Ukrainian translations
- Add AppArmor profile
- **Breaking:** the `armhf`, `armv7` and `i386` architectures are no longer supported; only `amd64` and `aarch64` are built
- Move base image into the Dockerfile
- Fix repository links (`main` branch) and documentation
- Remove unused `flow_control` option and fix `firmware_url` default
- Fix `BUILD_ARCH` build argument in Dockerfile

## 0.1.1

- Remove gpio from config

## 0.1.0

- Initial version release
