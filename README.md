## Fork status

This is a maintained fork of [hassio-addons/app-vaultwarden][upstream], which
sometimes lags in chasing issues. The community has responded with temporary
forks, but, due to how Home Assistant manages Apps data, this requires an 
export/import of vaults every time you switch to or from the forks.

The purpose of this permafork is to solely to have a permanent alternative
addon/apps slug that can be updated without relying on upstream.  Any changes
upstream will be quickly merged into here, so think of this as a HEAD that can
both lag and surge ahead.

The build fix and the release pipeline that replaces the `hassio-addons`
reusable workflows were worked out first in [JayTalge's fork][jay-fork].

REMEMBER: because Home Assistant identifies an add-on by repository and slug,
your vault does not follow you. Export from the old add-on and import into this one. 
