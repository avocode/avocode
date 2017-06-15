# Avocode Sketch Plugin
## Installation & Update
1. Completely Quit Sketch
2. [Download the latest Avocode macOS desktop app update](https://avocode.com/download).
The Sketch plugin is bundled with the Avocode desktop app, so you don't have to download anything else.
3. Double click on the downloaded DMG file to install it and the Sketch plugin will be installed automatically installed with it.
4. Open your Sketch app and go to 'Plugins' in the top window menu. The Avocode plugin should be there.

Note that the Sketch plugin requires you to have Avocode desktop app (2.14.3 and later) and Sketch (41 and later), therefore it works only on macOS. Direct upload of Sketch files also for Windows and Linux - independent on the Sketch app - is coming soon.
 
## How to upload Sketch designs to Avocode?
You can now sync artboards via a simple shortcut. Either CMD+E to upload selected artboards, or CMD+ALT+E to upload all artboards within the Sketch file. The Avocode app will launch so you can add the artboards to a particular project.
[Learn more about syncing Sketch designs to Avocode](https://help.avocode.com/projects-and-designs/design-upload/upload-sketch-designs-via-avocode-sketch-plugin).


## Changelog
### 43.0.0 (June 14, 2017)
- Sketch 41 Support
- Bundled and installed automatically with the Avocode macOS desktop app
- Faster upload which doesn't freeze Sketch app during design upload
- Shortcut to upload selected artboards (CMD + E)
- Shortcut to upload all artboards from a Sketch file (CMD + ALT + E)
- Seamless UX (no UI - the shortcut will automatically launch Avocode so you can add the artboard to a particular project)
- [Read more](https://help.avocode.com/projects-and-designs/design-upload/upload-sketch-designs-via-avocode-sketch-plugin)

### 42.0.0 (January 25, 2017)
- Sketch 42 Support on El Capitan 10.11.6
- when you hover over Artboard name, the full name will be showed

### 41.0.0 (November 8, 2016)
- Sketch 41 Support
- changed versioning to mirror supported Sketch version. Sketch 39 and 40 are still supported by this version.

### 3.9.0 (September 14, 2016)
- Sketch 40 Support

### 3.8.0 (July 20, 2016)
- Sketch 39 Support

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
