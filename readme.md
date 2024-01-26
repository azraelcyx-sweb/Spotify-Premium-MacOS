  <p align="center">
  <a href="https://github.com/CYXSpotiBlocker-CLI/CYXSpotiBlocker-Mac"><img src="https://raw.githubusercontent.com/CYXSpotiBlocker-CLI/CYXSpotiBlocker-commons/main/.github/Pic/Logo/logo-mac.png" />
</p>

<p align="center">        
      <a href="https://discord.gg/eYudMwgYtY"><img src="https://discord.com/api/guilds/807273906872123412/widget.png"></a>
      </p>

---

<center>
    <h4 align="center">A multi-featured adblocker for the Spotify macOS application.</h4>
    <p align="center">
        <strong>Last updated:</strong> 18 October 2023<br>
        <strong>Last tested version:</strong> 1.2.22.982
    </p> 
</center>

## We need collaborators.

- We are running short of people who can collaborate and maintain this project. If you are good with bash scripting, please create an issue here or contact red.dev in discord.

### Features:

- Blocks all banner/video/audio ads within the app
- Blocks logging (Sentry, etc)
- Unlocks the skip function for any track
- Blocks Spotify automatic updates (optional)
- Hides podcasts, episodes and audiobooks on Home Screen (optional)

### Installation/Update:

- Close Spotify completely.
- Run The following command in Terminal:

```
bash <(curl -sSL https://raw.githubusercontent.com/CYXSpotiBlocker-CLI/CYXSpotiBlocker-Mac/main/install.sh)
```

#### Note:

- CYXSpotiBlocker-Mac now requires codesign to sign the binaries after patching.
- For this, you will need to have Xcode installed on your mac.
- To install xcode, use the following command in terminal:

```
xcode-select --install
```

- If you have already installed xcode, you can skip this step.
- If you have Intel mac, you can try skipping codesign by using the `-S` flag.

#### Optional Install Arguments:

`-f` Force patch -- forces re-patching if backup detected  
`-h` Hide podcasts, episodes and audiobooks on home screen  
`-P` Path to Spotify.app -- set custom Spotify app path  
`-u` Block updated -- blocks automatic updates  
`-S` Skip Codesign -- only to be used if you have intel mac

Use any combination of flags.  
The following example clears app cache, adds experimental features, leaves new UI enabled and blocks updates:

```
bash <(curl -sSL https://raw.githubusercontent.com/CYXSpotiBlocker-CLI/CYXSpotiBlocker-Mac/main/install.sh) -hu
```

### Uninstall:

- Close Spotify completely.
- Run The following command in Terminal:

```
bash <(curl -sSL https://raw.githubusercontent.com/CYXSpotiBlocker-CLI/CYXSpotiBlocker-Mac/main/uninstall.sh)
```

or

- Reinstall Spotify

### Notes:

- Audio/video ads during Podcast playback are currently NOT blocked with CYXSpotiBlocker.
- Spicetify users: When using CYXSpotiBlocker-Mac + Spicetify, the current script requires running CYXSpotiBlocker first.

### DISCLAIMER

- Ad blocking is the main concern of this repo. Any other feature provided by CYXSpotiBlocker-Mac or consequence of using those features will be the sole responsibility of the user, not BlockTheSpot/CYXSpotiBlocker/CYXSpotiBlocker-Mac.
