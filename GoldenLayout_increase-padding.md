# How to increase the padding between the windows ?
## 1. GoldenLayout configuration
### Setting by default
```
var layout = new GoldenLayout({
    settings:{
        hasHeaders: true,
        constrainDragToContainer: true,
        reorderEnabled: true,
        selectionEnabled: false,
        popoutWholeStack: false,
        blockedPopoutsThrowError: true,
        closePopoutsOnUnload: true,
        showPopoutIcon: true,
        showMaximiseIcon: true,
        showCloseIcon: true
    },
    dimensions: {
        borderWidth: 5,
        minItemHeight: 10,
        minItemWidth: 10,
        headerHeight: 20,
        dragProxyWidth: 300,
        dragProxyHeight: 200
    },
    labels: {
        close: 'close',
        maximise: 'maximise',
        minimise: 'minimise',
        popout: 'open in new window'
    },
    content: [...]
});
```
Go to [here](http://golden-layout.com/docs/Config.html) for more detail about configuration.

[Here](http://golden-layout.com/docs/ItemConfig.html) is more infomation about **content** property.

## 2. Increase the padding between the windows
### Look at the dimensions property of GoldenLayouts configuration.
```
dimensions: {
    borderWidth: 5, // Adjusting this property the spaces between the windows will be adjusted
}
```


