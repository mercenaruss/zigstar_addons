# Changelog

## 0.2.1

- Download firmware with `curl --fail`, retries and timeouts over HTTPS only; exit with an error instead of reporting success when it fails
- Quote shell variables and use a temporary working directory
- Add optional IEEE address writing (`write_ieee`, `ieee`)
- Move base image to Python 3.13 / Alpine 3.22
- Use firmware from the TubesZB repository (20250321 builds, pinned commit) with SHA256 verification
- Mark add-on as stable
- Add AppArmor profile
- Fix repository links (`main` branch) and documentation

## 0.2.0

- Increased the chip flashing speed by 5 to 10 times compared to previous versions

## 0.1.0

- Initial addon release
