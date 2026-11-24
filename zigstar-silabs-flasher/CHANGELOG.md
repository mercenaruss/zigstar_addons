# Changelog

## 0.1.2

- Download firmware with `curl --fail`, retries and timeouts over HTTPS only; exit with an error instead of reporting success when it fails
- Quote shell variables and use a temporary working directory
- Move base image to Python 3.13 / Alpine 3.22
- Add Russian and Ukrainian translations
- Mark add-on as stable
- Add AppArmor profile
- Fix repository links (`main` branch) and documentation
- Remove unused `flow_control` option and fix `firmware_url` default
- Fix `BUILD_ARCH` build argument in Dockerfile

## 0.1.1

- Remove gpio from config

## 0.1.0

- Initial version release
