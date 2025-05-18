# WindowsThemeSetup
My current windows theme setup.

This setup is supposed to be as non destructive to base windows as much as possible and everything can be uninstalled from windows itself, restore point is not needed yes, but it is always a good thing to make one before doing something like this just in case.

![image](https://github.com/SouravDutta2206/WindowsThemeSetup/blob/main/image/collage.png)

This setup was done on Windows 11 Home Edition 24H2 

## Installations

### Wallpaper

Wallpaper - [Fern Wallpaper Unsplashed](https://unsplash.com/photos/green-fern-plant-AOhBMkQlzgM)

### Nerfonts
Install the JetBrainsMono Nerd Fonts from this page - [nerdfonts](https://www.nerdfonts.com/font-downloads)

### Yasb - Top bar
Yasb - [Yasb repo](https://github.com/amnweb/yasb)

follow the instructon there to install yasb and then get the yasb configs from [here](https://github.com/SouravDutta2206/WindowsThemeSetup/tree/241e1d3a62dbae682dbd7131be8528d872784134/Yasl) and put them in 

```
%USERPROFILE%\.config\yasb
```

restart yasb 

### Flow Launcher - Spotlight Search 

Install [Flow Launcher](https://www.flowlauncher.com/) and then install the [onsetGlaze](https://github.com/abhidahal/onsetGlaze.flow) theme for it.

### Nilesoft Shell - Right click context Menus

Install [Nilesoft shell](https://web.archive.org/web/20250328110621/https://nilesoft.org/download) either from this page or just use winget in powershell or cmd
```
winget install nilesoft.shell
```
if default installation was done go to this path or find your shell.exe's location, the imports folder will be there

```
C:\Program Files\Nilesoft Shell\imports
```
find the file theme.nss in a text editor as administrator and delete everything and paste this in and save the file 
```
theme
{
	name="modern"

    dark=auto
	background
	{
		color=auto
		opacity=0
		effect=2
	}
	item
	{
		opacity = 1
	}
	image.align=2
}
```
### Windhawk - Start menu, taskbar, notification center

install [Windhawk](windhawk.net)

install these mods:-
- Windows 11 Start Menu Styler
  * Settings > Theme - TranslucentStartMenu
  * Advanced > Custom process inclusion list - put ```SearchHost.exe``` here  
- Windows 11 Notification Center Styler
  * Settings > Theme - TranslucentShell
- Windows 11 Taskbar Styler
  * Settings > Theme - TranslucentTaskbar

### ExplorerBlurMica and DWMBlurGlass - Windows Explorer and top bar of most windows (not all)
install [ExplorerBlurMica](https://github.com/Maplespe/ExplorerBlurMica) and [DWMBlurGlass](https://github.com/Maplespe/DWMBlurGlass) according to the instructions on page

For DWMBlurGlass download the symbol files from the symbol tab

In general tab, set Blur radius to enable and its value to 25, disable Aero reflection effect.

### Rainmeter - clock widget

Install [Rainmeter](https://docs.rainmeter.net/manual/installing-rainmeter/)

Install the skins from [here](https://github.com/SouravDutta2206/WindowsThemeSetup/tree/61db8172a0d3a5c5d1c1a52d2cc5f7579ba92bac/Rainmeter)

These are edited versions of these skins 
- [Enmon](https://www.deviantart.com/apexxx-sensei/art/Enmon-760139205)
- [Medel](https://www.deviantart.com/apexxx-sensei/art/Medel-772303866)
  
Choose one and load the layout from the layout tab. 

### Windows Terminal 
If not installed, install [Terminal](https://apps.microsoft.com/detail/9n0dx20hk701?hl=en-US&gl=US) from Microsoft Store

Open terminal, open terminal settings 

go to Appearence and set ```Use acrylic material in the tab row``` to enable.

Under Profiles, in Defaults 
- set ```Font Face``` to ```JetBrainsMonoNL Nerd Font```
- ```Font Size``` to 10
- ```Background Opacity``` to 0%
- ```Enable acrylic material``` to enable

### Fastfetch - terminal info display

use winget to install [fastfetch](https://github.com/fastfetch-cli/fastfetch) from terminal

```winget install fastfetch```

Restart your terminal and type in ```fastfetch```, if it shows system info good

run this command, it will generate and give the location of the config file

```fastfetch --get-config```

get the fastfetch config file from [here](https://github.com/SouravDutta2206/WindowsThemeSetup/blob/97f8a42e717dcb944a17b538bba742b19871ecc6/fastfetch/config.jsonc) and replace the generated one.

### Spicetify - Spotify Customization

install [spotify](https://www.spotify.com/ca-en/download/other/) from the official spotify website not the microsoft store version (uninstall it if you have it)

install [Spicetify](https://spicetify.app/docs/getting-started/) using powershell and also install the marketplace.

install the [WebNowPlaying](https://github.com/marcopixel/monstercat-visualizer/wiki/WebNowPlaying-Spotify) plugin support, this is required by most music player related Rainmeter skins so its good to have enabled.

Open Spotify and from the Spicetify Marketplace theme section install the ```Lucid``` Theme

in Lucid Settings (gear icon first thing on the right side of the search bar)
- Background
  * Background > Mode - Solid Color
  * Background > Background Color - R = 0 , G = 0 , B = 0 (black) and Alpha - 100
  * Color > Tonal Color - Disable, Custom Color - Enable, Select Custom Color - R = 13, G = 47, B = 48 (Dark Turquoise-ish)
- Interface
  * Home > New Home Style - enable

### Zen Browser - My Default browser

Install Zen Browser from [here](https://zen-browser.app/download/)

Zen Mods -
- Navbar Margin
- Transparent Zen

To force dark theme on all webpages install the Dark Reader extension from the extension store.

### Betterdiscord and MicaForEveryone - Discord Theme
This is optional cause you don't need MicaForEveryone for anything else other than discord so if you don't use discord skip both.

have Discord installed and install [BetterDiscord](https://betterdiscord.app/)

- Open Discord
- Go to settings
- Go down to the new betterdiscord settings
- In themes section search for and install ```Discord Mica``` Theme
- In the settings section under window preferences set ```Enable Transparency``` to enable, your discord should be completely see through.
- Install [MicaForEveryone](https://github.com/MicaForEveryone/MicaForEveryone) and make everything default, add a rule for Discord and set backdrop type to Mica and Corner preference to Rounded.


