# iK3MO Admin Studio — signed Windows updates

This is a **distribution-only** repository. The original iK3MO application source remains private.

## For moderators

If the installed app has no **فحص التحديثات** button, install the bootstrap **once**:

1. Download [iK3MO Admin Studio 0.5.9 bootstrap](https://raw.githubusercontent.com/iiXDreemB52/ik3mo-admin-studio-updates/main/bootstrap/0.5.9.zip).
2. Close the program completely and extract the ZIP.
3. Run `APPLY-UPDATE.cmd`; this patches the same installed application, without uninstalling or clearing user data.
4. Reopen the application using the original shortcut.

Then the app checks for signed updates on startup and periodically. Press **تحديث الآن** when an update is available. The installer verifies the file's Ed25519-signed metadata and SHA-256 and stores a backup. If it cannot confirm the new app started, it attempts rollback.

For public release metadata: [latest.json](latest.json). Downloaded binaries are published under [files](files/).

**Important:** Initial bootstrap is compatible with the Windows Electron 44.7.2 app only. Do not apply it to a different application or an incompatible engine release.
