# linux wallpaper engine 
## wpe on everything other linux beside kde (f.e. gnome, hyprland, lxqt)
(precompiled from: https://github.com/Almamu/linux-wallpaperengine)

<img width="2702" height="1566" alt="2025-08-29_18-06" src="https://github.com/user-attachments/assets/9c607e9e-a42a-4204-8315-b08a9fcf94be" />


# installation / usage (debian)
> wget https://github.com/slynobody/linux_wallpaper_engine__precompiled/releases/download/0.8/int_linux_wallpaper_engine_amd64.deb
> 
> sudo apt install ./int_linux_wallpaper_engine_amd64.deb
> 
> cd /usr/local/bin/wpe

in wpe-dir, call the app + output-device followed by wallpaper-id, example:
> ./linux-wallpaperengine --screen-root eDP-1 3462267053

# 🔧 Options

| Option | Description |
|--------|-------------|
| `--silent` | Mute background audio |
| `--volume <val>` | Set audio volume |
| `--noautomute` | Don't mute when other apps play audio |
| `--no-audio-processing` | Disable audio reactive features |
| `--fps <val>` | Limit frame rate |
| `--window <XxYxWxH>` | Run in windowed mode with custom size/position |
| `--screen-root <screen>` | Set as background for specific screen |
| `--bg <id/path>` | Assign a background to a specific screen (use after `--screen-root`) |
| `--scaling <mode>` | Wallpaper scaling: `stretch`, `fit`, `fill`, or `default` |
| `--clamping <mode>` | Set texture clamping: `clamp`, `border`, `repeat` |
| `--assets-dir <path>` | Set custom path for assets |
| `--screenshot <file>` | Save screenshot (PNG, JPEG, BMP) |
| `--list-properties` | Show customizable properties of a wallpaper |
| `--set-property name=value` | Override a specific property |
| `--disable-mouse` | Disable mouse interaction |
| `--disable-parallax` | Disable parallax effect on backgrounds that support it |
| `--no-fullscreen-pause` | Prevent pausing while fullscreen apps are running |

## error: 'wallpaper not found'
wpe should be installed in one of these places
> ~/.steam/steam/steamapps/common
> 
> ~/.local/share/Steam/steamapps/common
> 
> ~/.var/app/com.valvesoftware.Steam/.local/share/Steam/steamapps/common
> 
> ~/snap/steam/common/.local/share/Steam/steamapps/common

if installed elsewere, do a symlink of the 'asset'-folder to /usr/local/bin/wpe & run wpe by folder
> ./linux-wallpaperengine --screen-root eDP-1 ~/backgrounds/1845706469/

## error: Failed to initialize GLEW: Unknown error
just ignore (wayland *is* supported): working wallpapers should simply show up (web-wallpapers have errors).

# Disclaimer
1. Use at your own risk!
2. This is for educational and research purposes only!
3. No responsibility taken for any local customizations of the git!
> 
<a href="https://artsandculture.google.com/experiment/viola-the-bird/nAEJVwNkp-FnrQ?cp=e30."><img src="https://images.pling.com/img/00/00/78/78/79/2160403/proxy-image1.jpeg"/></a>
