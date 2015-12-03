# Avocode Sketch Extension 3 Beta
This is a major new version that allows selective syncing of Sketch artboards. It can be installed alongside the old extension version 2. This is how it looks:

![screenshot](https://1670620568.rsc.cdn77.org/new-sketch/68484a3cb2344bd9978b8481467a6b50/preview.png)

## Installation
1. If your trial expired already and you want to try this version, give us an email at team@avocode.com and we will extend your trial.
2. Completely Quit Sketch
3. Download the latest beta version from [here](https://manager.avocode.com/download/sketch-plugin-beta/mac/)
4. Open the DMG and double click the sketchplugin file inside. It will take a while to install (will copy about 100MB of data, Sketch 3.4+ is required) and should open your Sketch afterwards
5. Open the extension in menu Plugins -> Avocode Sync Prerelease

## Changelog
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

## Known bugs
- [#549 Plugin doesn't allow me to select anything on Yosemite](https://github.com/avocode/avocode/issues/549) - see [workaround](https://github.com/avocode/avocode/issues/549#issuecomment-161592860)
- The UI can be sometimes not styled properly
- After you sync a sketch document to a project once, you cannot change it to another project
- It will take quite a lot of time to load first time, the production build work much faster.
- Pages are not exported at all, we might add that later if there is enough interest
- App Store Sketch is not be able to open the extension due to sandboxing issues. Use the build from http://sketchapp.com/ please, Sketch is now [leaving App Store anyway](http://blog.sketchapp.com/post/134322691555/leaving-the-mac-app-store)
 
## Reporting bugs
Please report bugs to team@avocode.com and include the `sketch-panels.log` file from Sketch Plugins folder

Pugin folder can be accessed from Sketch menu Plugins -> Manage Plugins and in the window click the Settings icon in bottom left corner and select Show Plugins Folder... (or in Sketch 3.3 and older press Plugins -> Reveal Plugins)
