# Avocode Sketch Extension 3 Beta
This is a major new version that allows selective syncing of Sketch artboards. It can be installed alongside the old extension version 2. This is how it looks:

<img src="https://upx.cz/BfD" width="760" height="642">

## Installation & Update
1. Completely Quit Sketch
2. Download the latest beta version

   [<img src="https://upx.cz/Bfo" width="241" height="59">](https://manager.avocode.com/download/sketch-plugin-beta/mac/)
3. Open the DMG and double click the sketchplugin file inside. It should open your Sketch automatically and install / update the extension
4. Open the extension in menu `Plugins -> Avocode Sync 3.2`
   
   <img src="https://upx.cz/BZk" width="224" height="126">

## Known bugs
- The older extension is not removed and remains installed alongside the new one
- You need to quit and re-launch sketch after you used the old extension (2.1.x) before opening Avocode Sync 3
- Sketch Pages are not exported at all, we might add that later if there is enough interest. Please [vote here](http://avocode.uservoice.com/forums/277080-feature-voting/suggestions/11634147-support-exporting-pages-in-sketch-extension-3) if you need that feature
- If you use Sketch from App Store, the extension will not launch due to sandboxing issues. Use the build from http://sketchapp.com/ please, Sketch is now [leaving App Store](http://blog.sketchapp.com/post/134322691555/leaving-the-mac-app-store) anyways
 
## Reporting bugs
Please report bugs to team@avocode.com and include the `sketch-panels.log` file from Sketch Plugins folder

Pugin folder can be accessed from Sketch menu Plugins -> Manage Plugins and in the window click the Settings icon in bottom left corner and select Show Plugins Folder...


## Changelog
### 3.2.0 (February 10, 2016)
- Added fix for users with Yosemite that were not able to control plugin correctly. In this version of Mac OS, plugin UI opens in Safari and works without problems.
- Fixed bug with Avocode setting all layers visibility to visible.
- Added handling for inactive accounts (expired trial, unpaid plan)
- Few UI improvements

### 3.1.0 (January 29, 2016)
- Fixed some errors that prevented 3.0.0 to launch
- Changed the DMG and menu text

### 3.0.0 (January 29, 2016)
- Brings back support for Sketch 3.4 and still supports latest Sketch 3.5.1
- Fixed few glitches with selecting project that made synced document not appear from Avocode App

### 3.0.0-prerelease4 (January 22, 2016)
- Sketch 3.5 support
- Important note: this breaks Sketch 3.4 support at the moment! In case you need to remain using Sketch 3.4 (e.g. on OSX 10.9) don't update to this version

### 3.0.0-prerelease3 (January 11, 2016)
- you can now change project of already synced documents
- faster extension loading
- added new succes state after the syncing is complete
- Sketch Beta support
- detect plugin framework collision and prevent from running in that case (if you run old one in the same Sketch session)

### 3.0.0-prerelease2 (December 1, 2015)
- hide social login. When we release the plugin, Avocode App will login the extension for you
- fixed aspect ratio of artboard thumbnails
- when you update document, artboards you synced in the past will be preserved
- build is about 40% smaller
- add update checker
- sync progress bar
- new window size and some other style fixes

### 3.0.0-prerelease1 (November 19, 2015)
- initial beta release
