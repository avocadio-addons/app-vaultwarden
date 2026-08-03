# Changelog

## 0.28.1

- ⬆️ Update Vaultwarden to 1.37.1
- 🐛 Bump stale Debian package pins that no longer exist on the mirror and
  broke the build: `libpq5` 17.9 -> 17.10, `nginx` deb13u2 -> deb13u7
- 🏗️ Build and publish the add-on image from this fork to
  `ghcr.io/avocadio-addons/bitwarden`
- 🔧 Replace the `hassio-addons/workflows` build and release callers, which
  cannot run from a fork, with a self-contained CI, stamp and deploy pipeline
- ⬆️ Watch upstream for changes and raise them as a pull request

Upstream shipped 1.36.0 as add-on 0.27.0 and then stalled. The 1.37.0 pin bump
that upstream never released is folded into this release, so 0.28.0 does not
exist here.

## 0.27.0

- ⬆️ Update Vaultwarden to 1.36.0
