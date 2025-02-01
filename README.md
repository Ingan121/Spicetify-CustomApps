# WMPotify NowPlaying
* WMPotify NowPlaying is a custom app for Spicetify that features WMP-like visualization screen and lyrics overlaid on top of it.
* It is recommended to use this app with the [WMPotify](https://github.com/Ingan121/WMPotify) theme for Spicetify.
    * Using it with other themes is possible too.

## **Installation** / Updating

### **Manual installation using Scripts (recomended):**

#### **Windows (Powershell)**

* WMPotify NowPlaying only:
```powershell
[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12
iex "& { $(iwr -useb 'https://raw.githubusercontent.com/Ingan121/WMPotify/master/installer/install.ps1') } -Install @('wmpvis')"
```

* WMPotify + WMPotify NowPlaying + Windhawk + CEF/Spotify Tweaks mod
    * This script detects whether Spotify, Spiceify, Windhawk, and CEF/Spotify Tweaks mod are installed or not. If not, it will install them.
    * If Windhawk is installed and CEF/Spotify Tweaks mod is up-to-date, the installation of these two will be skipped.

```powershell
[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12
iex "& { $(iwr -useb 'https://raw.githubusercontent.com/Ingan121/WMPotify/master/installer/install.ps1') }"
```

#### **Linux/macOS (Bash)**

* Note: Not tested on macOS yet

* WMPotify NowPlaying only:
```bash
export SKIP_THEME=true
curl -fsSL https://raw.githubusercontent.com/Ingan121/WMPotify/master/installer/install.sh | sh
```

* WMPotify + WMPotify NowPlaying
```bash
curl -fsSL https://raw.githubusercontent.com/Ingan121/WMPotify/master/installer/install.sh | sh
```

### **Manual installation**
* Visit [WMPotify](https://github.com/Ingan121/WMPotify) for the theme installation instructions.

1. Download the latest release from the [releases page](https://github.com/Ingan121/WMPotify/releases)
2. Locate Spicetify directories: use `spicetify config-dir` or `spicetify path userdata`
3. Extract the contents of the WMPotify NowPlaying zip to the `CustomApps\wmpvis` folder in the Spicetify directory. Create the `CustomApps\wmpvis` folder if it doesn't exist.
4. Run the following commands in Command Prompt / PowerShell / Terminal:
    ```cmd
    spicetify config custom_apps wmpvis
    spicetify apply
    ```

## **Uninstallation**
```cmd
spicetify config custom_apps wmpvis-
spicetify apply
```

## Screenshots

* Aero
![wmpvis_aero](wmpvis/screenshots/wmpvis_aero.png)

* Basic
![wmpvis_basic](wmpvis/screenshots/wmpvis_basic.png)

* XP
![wmpvis_xp](wmpvis/screenshots/wmpvis_xp.png)

* Menu
![wmpvis_menu](wmpvis/screenshots/wmpvis_menu_xp.png)

* Bars Visualization
![wmpvis_bars](wmpvis/screenshots/wmpvis_bars_xp.png)
