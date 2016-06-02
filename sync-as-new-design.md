You can use this script to unlink document from any Avocode design and Sync it as a new separate design.

1. Open the Sketch document you want to sync as a new design
2. Go to Plugins -> Custom Plugin...
3. Copy & Paste the code below and press the Run button

```javascript
var params = {
        clearTags: !0
    },
    doc = context.document,
    cmd = context.command;
if (params.artboardFilter && 0 !== params.artboardFilter.length || (params.artboardFilter = !1), doc) {
    for (var MSArtboardGroupClass = MSArtboardGroup["class"](), fileURL = doc.fileURL(), output = {
            name: String(doc.displayName()),
            path: String(fileURL.path()),
            pages: [],
            tempDir: params.tempDir
        }, pages = doc.pages(), i = 0, pageCount = pages.count(), page, pageID, artboards, pageData, pageManagerLink, pageManagerID; pageCount > i; ++i) {
        if (page = pages[i], pageID = String(page.objectID()), artboards = page.artboards(), params.clearTags && cmd.setValue_forKey_onLayer_forPluginIdentifier({
                pageID: pageID,
                managerID: "unassigned"
            }, "managerLink", page, "avocode"), pageManagerLink = cmd.valueForKey_onLayer_forPluginIdentifier("managerLink", page, "avocode"), pageManagerID = null, pageManagerLink && pageManagerLink.pageID == pageID && (pageManagerID = String(pageManagerLink.managerID)), pageData = {
                name: String(page.name()),
                pageID: pageID,
                managerID: pageManagerID,
                artboards: [],
                previewCount: 0
            }, !params.skipArtboards)
            for (var j = 0, artboardCount = artboards.count(), artboard, artboardID, artboardManagerLink, artboardManagerID; artboardCount > j; ++j) artboard = artboards[j], artboard.isKindOfClass(MSArtboardGroupClass) && (artboardID = String(artboard.objectID()), (params.artboardFilter === !1 || params.artboardFilter.indexOf(artboardID) > -1) && (params.clearTags && cmd.setValue_forKey_onLayer_forPluginIdentifier({
                artboardID: artboardID,
                managerID: "unassigned"
            }, "managerLink", artboard, "avocode"), artboardManagerLink = cmd.valueForKey_onLayer_forPluginIdentifier("managerLink", artboard, "avocode"), artboardManagerID = null, artboardManagerLink && artboardManagerLink.artboardID == artboardID && (artboardManagerID = String(artboardManagerLink.managerID)), artboardData = {
                artboardID: artboardID,
                pageID: pageID,
                name: String(artboard.name()),
                managerID: artboardManagerID
            }, pageData.artboards.push(artboardData)));
        pageData.artboards.length > 0 && output.pages.push(pageData)
    }
    print('Successfully removed Avocode link from this document')
    print('')
    print(JSON.stringify(output))
} else print("false");
```
