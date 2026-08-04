# Migrating to or from this fork

Home Assistant identifies an add-on by **(repository, slug)**. This fork uses
a different slug (`vaultwarden`) than upstream's (`bitwarden`), and
the repository also differs. Home Assistant treats them as **separate add-ons with
separate data directories**. Your vault, attachments, and admin token do
**not** carry over automatically.

## From upstream to this fork

1. In the upstream add-on's web vault, **export your vault** (Settings →
   Export Vault). If you use file attachments, download those separately —
   they are not included in the export.
2. **Stop** the upstream add-on but leave it installed.
3. Add this fork's repository to Home Assistant
   (Settings → Add-ons → Add-on Store → ⋮ → Repositories) and install
   the Vaultwarden add-on from it.
4. Start the new add-on. Complete initial setup and retrieve the admin token
   from the logs.
5. **Import your vault** into the new add-on's web vault. Re-upload any
   attachments. Verify 2FA devices still work.
6. Confirm everything is working before uninstalling the upstream add-on.

## From this fork to upstream (or another fork)

The same procedure applies in reverse. Export, install the target, import,
verify, then uninstall the source.

## Notes

- The SQLite database, attachments, and configuration live under different
  paths for each repository's add-on. There is no way to share them
  in place.
- Keep the old add-on stopped-but-installed until you have fully verified
  the new one. Uninstalling deletes its data directory.
