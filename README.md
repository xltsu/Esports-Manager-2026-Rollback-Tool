# eltsu's em26 rollback tool

[Download the latest version](https://github.com/xltsu/project/releases/latest)

A small Windows tool for switching between older Steam builds of Esports Manager 2026.

Pick a version, download it with your own Steam account, then install it from the same menu. The tool keeps a backup of your current game folder so you can switch back later.

## Getting started

1. Download the `.exe` and run it. You don't need to install anything else.
2. Check that the game folder is correct. Use **Browse folder** if it wasn't found automatically.
3. Select a build and click **Download version**. Scan the QR code with the Steam mobile app to sign in.
4. Back up your saves separately and close both Steam and the game.
5. Click **Install selected**. Use **Restore backup** to return to your most recent backup.

You need the Steam version of the game on your account. This tool doesn't include any game files.

## Files and backups

On the first launch, the app creates an `em26rollbacktool` folder in your Windows **Documents** folder. It stores the download helper, downloaded builds and app data there. The downloaded `.exe` can stay wherever you put it.

Game folder backups are kept beside your Steam installation of the game, in folders named `.eltsu-backup-...`. Save files aren't included in those backups.

## A few things to know

- The menu includes 10 Windows builds. Dates are the UTC dates recorded by SteamDB; the manifest ID identifies each build.
- The build list doesn't update automatically.
- Steam may update the game again when you launch it. The tool doesn't block Steam updates.
- Some older builds may no longer be available to download.
- Old builds and newer saves may not work together. Keep a separate copy of your saves.
- The installed label tracks changes made by this tool. It won't detect a later Steam update.

Windows x64 is required. The app and download helper have been checked locally, but authenticated game downloads and gameplay still need testing. The executable is unsigned.

## Support

If you find it useful, you can [buy me a coffee](https://ko-fi.com/eltsu). Thanks for the support.

## Credits

Downloads use [DepotDownloader](https://github.com/SteamRE/DepotDownloader), made by SteamRE. Version 3.4.0 is bundled with the app under GPL-2.0, and its license is extracted with the helper on first launch. Its [corresponding source code is available here](https://github.com/SteamRE/DepotDownloader/tree/DepotDownloader_3.4.0).

Version information comes from [SteamDB](https://steamdb.info/app/2749950/patchnotes/). This is an unofficial tool and isn't affiliated with Steam, Valve or the game's developers.
