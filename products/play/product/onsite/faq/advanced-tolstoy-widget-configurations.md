## Advanced Tolstoy Widget Configurations

If you are looking to manually configure your widget to your preference (always shown, remove the close option, etc.), then you have come to the right place! Here's how you can configure your Tolstoy widget on your site:

1. First, find your Tolstoy ID from within your Tolstoy URL (`http://player.gotolstoy.com/TOLSTOY_ID`), and paste the following code on your site:

    ```javascript
    window.tolstoyWidgetId = 'TOLSTOY_ID';
    ```

2. Choose which of the following configurations you want for your widget, and add the corresponding pieces of code. Here's the entire piece of code, including all of the options mentioned below:

    ```javascript
    window.tolstoySettings = {
        alwaysShow: true,
        loadHidden: true,
        minified: true,
        stopPreviewLoop: true,
        noCloseOption: true,
    };
    ```

### Configuration Options

Here's a breakdown of the options you have to configure your widget, with the corresponding lines of code:

- **alwaysShow**: In case a user closed the widget and you want to keep showing it to them.
    - To enable, add: `alwaysShow: true`
- **loadHidden**: Load the widget without showing it.
    - To enable, add: `loadHidden: true`
- **minified**: Show a minified version of the preview.
    - To enable, add: `minified: true`
- **stopPreviewLoop**: Stop the preview window from endlessly looping.
    - To enable, add: `stopPreviewLoop: true`
- **noCloseOption**: No option to close the widget.
    - To enable, add: `noCloseOption: true`

3. Choose the following methods you want for your widget, and add the following pieces of code to enable them:

- **start()**: Start the widget on expanded and play immediately.
    ```javascript
    window.tolstoyWidget.start();
    ```

- **show()**: Show the widget.
    ```javascript
    window.tolstoyWidget.show();
    ```

- **hide()**: Hide the widget.
    ```javascript
    window.tolstoyWidget.hide();
    ```

- **recreate(tolstoyWidgetId, settings)**: Load a new widget; settings are optional.
    ```javascript
    window.tolstoyWidget.recreate('TOLSTOY_ID');
    ```

- **on(eventType, callback)**: Gives the option to trigger a callback on chosen events.

    **Params:**
    - **eventType**: Supported events:
        - `onWidgetOpen` - triggers when the widget is opened
        - `onWidgetReady` - triggers when the widget is ready
    - **callback**: A function to trigger.

    **Example:**
    ```javascript
    window.tolstoyWidget.on('onWidgetOpen', () => { console.log('Widget Opened'); });
    ```
