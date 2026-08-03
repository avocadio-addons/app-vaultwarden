# Changelog

## 0.27.0.1

- Permafork of hassio-addons/app-vaultwarden based on upstream v0.27.0
- Vaultwarden 1.36.0 -> 1.37.1
- Bump stale Debian package pins: libpq5 17.9 -> 17.10,
  nginx deb13u2 -> deb13u7
- Self-contained CI, deploy, and upstream-sync pipeline replacing
  the hassio-addons/workflows callers a fork cannot use
- Slug changed from bitwarden to vaultwarden
- Migration docs, fork-local links, image published to
  ghcr.io/avocadio-addons/vaultwarden
