# Avocode Sketch Extension 3 Beta

This is a major new version that allows selective syncing of Sketch artboards.

## Installation
1. Download the latest beta version from [here](https://manager.avocode.com/download/sketch-plugin-beta/mac/)
2. Extract the zip file
3. After that you can either install by moving the package or double-clicking the package, see below

### Install by moving the package

1. Open your Sketch and press Plugins -> Manage Plugins and in the window click the Settings icon in bottom left corner and select Show Plugins Folder... (or in Sketch 3.3 and older press Plugins -> Reveal Plugins)
2. Move `Avocode Prerelease.sketchplugin` to this folder
3. You will find the plugin in Plugins -> Avodode Sync Prerelease

### Alternative: Install by double-clicking
Since Sketch 3.4 you can simply double-click the extracted `Avocode Prerelease.sketchplugin` package and Sketch will install it for you. However the installation can take a long time as the package is over 150MB in size with many contained files. You can use the alternative installation guide above to save some time

## Known bugs
- Every time you sync just selected artboards of the documents, other artboards that you could have synced beforehand will disappear from the app. This is a top priority to fix right now
- Social login doesn't work yet, you need to use your email&password
- The UI can be sometimes not styled properly, aspect ratio of artboard thumbnails is often not correct
- It will take quite a lot of time to load first time, the production build work much faster.
- The beta build is quite large, production release will be much smaller
- Pages are not exported at all, we might add that later if there is enough interest
 
## Reporting bugs
Please report bugs to team@avocode.com and include the `sketch-panels.log` file from Sketch Plugins folder

Pugin folder can be accessed from Sketch menu Plugins -> Manage Plugins and in the window click the Settings icon in bottom left corner and select Show Plugins Folder... (or in Sketch 3.3 and older press Plugins -> Reveal Plugins)
