# Changelog

## fork (jerji) — 2026-05-28

- Bump base image (Sonoff iHost add-on) `1.0.0` -> `1.0.2`
  (fixes "ASH_ERROR_TIMEOUTS on Zigbee2MQTT first launch" and "zigbee.conf not found").
- Bump `universal-silabs-flasher` `0.0.31` -> `1.0.3` (newest release compatible
  with the bullseye/Python 3.9 base; `1.1.0+` requires Python >= 3.11).
- Update the flasher invocation for the 1.x CLI: dropped `--ensure-exact-version`
  and `--allow-cross-flashing` (removed upstream; cross-flashing is now the default).
- Publish to GHCR only (`ghcr.io/jerji/ihost-multipan-docker`); removed Docker Hub
  login/tags from CI.

### Known limitations

- `config.sh` runs as a cont-init step (before the flasher service), so the
  flasher's `/tmp/known-baudrate` hint is not consumed. Set `BAUDRATE` explicitly
  to match your firmware (iHost default `115200`).

---

Upstream add-on changelog:
https://github.com/iHost-Open-Source-Project/hassio-ihost-addon/tree/master/hassio-ihost-silabs-multiprotocol/CHANGELOG.md
