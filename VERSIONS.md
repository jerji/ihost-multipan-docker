# Versions

This image is tagged to match the **Sonoff iHost add-on** base version it is
built from (the `BASE_VERSION` build arg / `ghcr.io/ihost-open-source-project/
hassio-ihost-silabs-multiprotocol-<arch>` tag).

| container tag | base (iHost add-on) | universal-silabs-flasher | notes                                  |
|---------------|---------------------|--------------------------|----------------------------------------|
| 1.0.2         | 1.0.2               | 1.0.3                    | current; not yet verified on hardware  |
| 1.0.0         | 1.0.0               | 0.0.31                   | previous (antoniocifu)                 |

Firmware for the iHost MG21 multipan radio comes from the Sonoff dongle flasher
repo: https://github.com/iHost-Open-Source-Project/hassio-ihost-sonoff-dongle-flasher/tree/main/firmware-build

The legacy SkyConnect firmware combinations from the original (Home Assistant
add-on) lineage do not apply to this iHost-based image.
