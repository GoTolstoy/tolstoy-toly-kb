## What are the advanced Tolstoy widget configurations?

If you are looking to manually configure your widget to your preference (always shown, remove the close option, etc.) then you came to the right place! Here's how you can configure your Tolstoy widget on your site:


1. First, find your Tolstoy ID from within your Tolstoy URL (http://player.gotolstoy.com/TOLSTOY_ID), and paste the following code on your site.
                    window.tolstoyWidgetId='TOLSTOY_ID'

2. Choose which of the following configurations you want for your widget, and add pieces following code.
Here's the entire piece of code, including all of the options mentioned below:
 ​
window.tolstoySettings = {
 alwaysShow: true,
 loadHidden: true,
 minified: true,
 stopPreviewLoop: true,
 noCloseOption: true,
};


Here's a breakdown of the options you have to configure your widget, with the corresponding lines of code:
alwaysShow: In case a user closed the widget and you want to keep showing it to him.
To enable, add: alwaysShow: true
loadHidden: load the widget without showing it.
To enable, add: loadHidden: true
minified: show a minified version of the preview.
To enable, add: minified: true
stopPreviewLoop: stop the preview window from endlessly looping.
stopPreviewLoop: true
noCloseOption: no option to close the widget.
noCloseOption: true
3. Choose the following methods you want for your widget, and add the following pieces of code to enable:
start()
start the widget on expanded and plays immediately
 window.tolstoyWidget.start();


show()
show the widget
window.tolstoyWidget.show();


hide()
hide the widget
window.tolstoyWidget.hide();


recreate(tolstoyWidgetId, settings)
load a new widget, settings are optional
window.tolstoyWidget.recreate('TOLSTOY_ID');


on(eventType, callback)
gives option to trigger a callback on chosen events.
Params:
eventType
supported events:
onWidgetOpen - triggers when the widget is opened
onWidgetReady - triggers when the widget is ready
callback
A function to trigger.
Example:
window.tolstoyWidget.on('onWidgetOpen', () => { console.log('Widget Opened') });
