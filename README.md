# Spotify-Adblocker-for-MacOS

              ```
### INSTALL : bash (install file)
              ```
              
### UPDATE : same as install
### UNINSTALL : bash (uninstall file)

### Features:
- Blocks all banner/video/audio ads within the app
- Blocks logging (Sentry, etc)
- Unlocks the skip function for any track
- Blocks Spotify automatic updates (optional)
- Hides podcasts, episodes and audiobooks on Home Screen (optional)

Note:
CYXblocker-Mac now requires codesign to sign the binaries after patching.
For this, you will need to have Xcode installed on your mac.
To install xcode, use the following command in terminal:
xcode-select --install
If you have already installed xcode, you can skip this step.
If you have Intel mac, you can try skipping codesign by using the -S flag.

Optional Install Arguments:
-f Force patch -- forces re-patching if backup detected
-h Hide podcasts, episodes and audiobooks on home screen
-P Path to Spotify.app -- set custom Spotify app path
-u Block updated -- blocks automatic updates
-S Skip Codesign -- only to be used if you have intel mac

Notes:
Audio/video ads during Podcast playback are currently NOT blocked with CYXblocker.
Spicetify users: When using CYXblocker-Mac + Spicetify, the current script requires running SpotX first.
DISCLAIMER
Ad blocking is the main concern of this repo. Any other feature provided by CYXblocker-Mac or consequence of using those features will be the sole responsibility of the user, not BlockTheSpot/SpotX/SpotX-Mac.
