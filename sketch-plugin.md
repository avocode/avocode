# Avocode Sketch Plugin 3
## Installation & Update
1. Completely Quit Sketch
2. Download the latest plugin version

   [<img src="https://upx.cz/Bfo" width="241" height="59">](https://manager.avocode.com/download/sketch-plugin/mac/)
3. Open the DMG and double click the sketchplugin file inside. It should open your Sketch automatically and install / update the plugin
4. Open the plugin in menu `Plugins -> Avocode Sync 3.8`

## Known bugs
- You need to quit and re-launch sketch after you used the old plugin (2.1.x) before opening Avocode Sync 3
- If you duplicate already synced document (or artboard) to a new document it will still sync to the original design. You can fix this by syncing to a different project or by running [custom workaround script](sync-as-new-design.md)
- Sketch Pages are not exported at all, we might add that later if there is enough interest. Please [vote here](http://avocode.uservoice.com/forums/277080-feature-voting/suggestions/11634147-support-exporting-pages-in-sketch-extension-3) if you need that feature
- If you use Sketch from App Store, the plugin will not launch due to sandboxing issues. Use the build from http://sketchapp.com/ please, Sketch is now [leaving App Store](http://blog.sketchapp.com/post/134322691555/leaving-the-mac-app-store) anyways
 
## Reporting bugs
Please report bugs to team@avocode.com and include the `sketch-panels.log` file from Sketch Plugins folder

Plugin folder can be accessed from Sketch menu Plugins -> Manage Plugins and in the window click the Settings icon in bottom left corner and select Show Plugins Folder...

If there is no `sketch-panels.log` it means the extension did not launch properly, please try opening the Console App -> All Messages and look for any errors when you launch the extension.


## Changelog

### 3.8.0 (Jul 20, 2016)
- Support Sketch 3.9

### 3.7.0 (May 27, 2016)
- Fixed another issue with text layers that could cause whole artboard sync to fail in some rare cases

### 3.6.0 (May 25, 2016)
- Fixed an issue that could lead to documents synced into each other even when you change a project
- Fixed opening on Yosemite (with Safari 9.1.1 update) [#879](https://github.com/avocode/avocode/issues/879)

### 3.5.0 (May 5, 2016)
- Fixed multiple issues that could prevent synced pages/artboards from appearing in Avocode
- Improved logging so we can debug new issues more easily

### 3.4.0 (April 14, 2016)
- Fixed sync of text layers that could cause whole artboard to fail in some cases [#827](https://github.com/avocode/avocode/issues/827) [#803](https://github.com/avocode/avocode/issues/803)
- If you don't quit sketch before update, it should be handled better (no document open would be showed otherwise). This fix will only affect future updates
- Updated DMG to mention that you need to Quit Sketch before installation

### 3.3.0 (March 8, 2016)
- With this release Sketch Plugin 3 is officially out of beta
- Added Cancel button to sync
- Added a label that tells you when your last sync happened
- New browser login that should fix all the previous problems with authorization
- Fixed progress bar that was stuck at the beginning
- Fixed window modality bug (now it doesn't overlap other apps, only Sketch)

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
- faster plugin loading
- added new succes state after the syncing is complete
- Sketch Beta support
- detect plugin framework collision and prevent from running in that case (if you run old one in the same Sketch session)

### 3.0.0-prerelease2 (December 1, 2015)
- hide social login. When we release the plugin, Avocode App will login the plugin for you
- fixed aspect ratio of artboard thumbnails
- when you update document, artboards you synced in the past will be preserved
- build is about 40% smaller
- add update checker
- sync progress bar
- new window size and some other style fixes

### 3.0.0-prerelease1 (November 19, 2015)
- initial beta release
