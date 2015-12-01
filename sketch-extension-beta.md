# Avocode Sketch Extension 3 Beta

This is a major new version that allows selective syncing of Sketch artboards. It can be installed alongside the old extension version 2.

## Installation
1. Download the latest beta version from [here](https://manager.avocode.com/download/sketch-plugin-beta/mac/)
2. Open the DMG
3. Double click the sketchplugin file inside. It will take a while to install (Sketch 3.4+ is required)

## Changelog
### 3.0.0-prerelease2
- hide social login. When we release the plugin, Avocode App will login the extension for you
- fixed aspect ratio of artboard thumbnails
- when you update document, artboards you synced in the past will be preserved
- build is about 40% smaller
- add update checker
- sync progress bar
- new window size and some other style fixes

### 3.0.0-prerelease1
- initial beta release

## Known bugs
- App Store Sketch might not be able to open the extension due to sandboxing. Use the build from http://sketchapp.com/ if possible
- The UI can be sometimes not styled properly
- It will take quite a lot of time to load first time, the production build work much faster.
- The beta build is quite large, production release will be much smaller
- Pages are not exported at all, we might add that later if there is enough interest
 
## Reporting bugs
Please report bugs to team@avocode.com and include the `sketch-panels.log` file from Sketch Plugins folder

Pugin folder can be accessed from Sketch menu Plugins -> Manage Plugins and in the window click the Settings icon in bottom left corner and select Show Plugins Folder... (or in Sketch 3.3 and older press Plugins -> Reveal Plugins)
