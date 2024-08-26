# Tolstoy Widget JavaScript SDK

## Introduction

This document outlines the JavaScript SDK for the Tolstoy widget, a customizable floating widget that can be integrated into websites. The SDK provides various methods to configure and control the widget's behavior.

## Widget Configuration

### Settings

The Tolstoy widget supports several configuration options that can be set using the `window.tolstoySettings` object. Here are the available settings:

| Setting | Type | Default | Description |
|---------|------|---------|-------------|
| `alwaysShow` | boolean | `true` | If set to `true`, the widget will continue to show even if a user has previously closed it. |
| `loadHidden` | boolean | `true` | If set to `true`, the widget will load without being initially visible. |
| `stopPreviewLoop` | boolean | `true` | If set to `true`, it prevents the preview window from looping endlessly. |
| `noCloseOption` | boolean | `true` | If set to `true`, it removes the option for users to close the widget. |

#### Example: Setting Widget Configuration

To configure the widget, add the following code to your page:

```javascript
// Configure Tolstoy widget settings
window.tolstoySettings = {
  // Always show the widget, even if the user has closed it before
  alwaysShow: true,
  
  // Load the widget in a hidden state initially
  // This allows you to control when it becomes visible
  loadHidden: true,
  
  // Prevent the preview from looping continuously
  // This can be useful to avoid distracting users
  stopPreviewLoop: true,
  
  // Remove the close button from the widget
  // Use this if you want the widget to be always accessible
  noCloseOption: true,
};

// Note: These settings should be set before the Tolstoy widget script is loaded
// or immediately after it's loaded, but before any interactions with the widget
```

## Widget Methods

The Tolstoy widget provides several methods to control its behavior. These methods are accessed through the `window.tolstoyWidget` object.

### start()

Starts the widget, expands it, and begins playback immediately.

```javascript
// Start the Tolstoy widget
window.tolstoyWidget.start();

// This method does the following:
// 1. Makes the widget visible if it was hidden
// 2. Expands the widget to its full size
// 3. Begins playing the widget content immediately
// Use this when you want to proactively show the widget to the user
```

### startPart(partNumber)

Starts the widget at a specific part number, expands it, and begins playback immediately. If the widget is already open, it will start playing the specified part.

```javascript
// Start the Tolstoy widget at part 2
window.tolstoyWidget.startPart(2);

// This method:
// 1. Makes the widget visible if it was hidden
// 2. Expands the widget to its full size
// 3. Jumps to the specified part (in this case, part 2)
// 4. Begins playing from that part immediately
// Useful for directing users to specific content within the widget
```

### show()

Displays the widget bubble if it was loaded hidden or previously closed.

```javascript
// Show the Tolstoy widget
window.tolstoyWidget.show();

// This method:
// 1. Makes the widget bubble visible on the page
// 2. Does not expand the widget or start playback
// Use this to reveal the widget after it was initially loaded hidden
// or if it was previously hidden using the hide() method
```

### hide()

Hides the widget bubble from the screen.

```javascript
// Hide the Tolstoy widget
window.tolstoyWidget.hide();

// This method:
// 1. Hides the widget bubble from view
// 2. The widget remains loaded and configured, just not visible
// Useful for temporarily removing the widget from the user's view
// without fully unloading it
```

### recreate(tolstoyWidgetId, settings)

Loads a new widget with a different Tolstoy ID. Remember to replace `{{TOLSTOY_ID}}` with your actual Tolstoy widget ID.

```javascript
// Recreate the Tolstoy widget with a new ID
window.tolstoyWidget.recreate("{{TOLSTOY_ID}}");

// This method:
// 1. Unloads the current widget (if any)
// 2. Loads a new widget with the specified Tolstoy ID
// 3. Applies any new settings provided (optional)
// Useful for dynamically changing the widget content without reloading the page
// Make sure to replace {{TOLSTOY_ID}} with your actual Tolstoy widget ID
```

### on(eventType, callback)

Registers a callback function to be triggered on a specific event.

#### Parameters:

- `eventType`: String - The type of event to listen for. Supported events are:
  - `"onWidgetOpen"`: Triggered when the widget is opened
  - `"onWidgetClose"`: Triggered when the widget is closed
  - `"onWidgetReady"`: Triggered when the widget is ready
  - `"onTolstoyClose"`: Triggered when the Tolstoy bubble is closed
- `callback`: Function - The function to be executed when the event occurs

```javascript
// Register a callback for when the widget opens
window.tolstoyWidget.on("onWidgetOpen", () => {
  console.log("Tolstoy Widget Opened");
  
  // You can perform any actions here that you want to occur
  // when the widget is opened. For example:
  // - Track an analytics event
  // - Update page content
  // - Trigger other page behaviors
});

// This method allows you to hook into key widget events
// and extend its functionality or integrate it with other
// parts of your website or application
```

## Additional Functionality

### Reject Cookie Policy

This method can be used when a user rejects the cookie policy.

```javascript
// Notify the widget that the cookie policy has been rejected
window.tolstoyWidget.postMessage({ eventName: "tolstoy_reject_cookie_policy" });

// This method:
// 1. Sends a message to the Tolstoy widget
// 2. Informs the widget that the user has rejected the cookie policy
// 3. Allows the widget to adjust its behavior accordingly (e.g., not setting cookies)

// Use this method when you have a separate cookie consent mechanism
// and need to inform the Tolstoy widget of the user's choice
```

## Best Practices

1. Always ensure that the Tolstoy widget script is loaded before using any of these methods.
2. Use the `onWidgetReady` event to make sure the widget is fully loaded before interacting with it.
3. Consider user experience when configuring settings like `alwaysShow` and `noCloseOption`.
4. Test the widget thoroughly in different scenarios to ensure it behaves as expected.

## Troubleshooting

If you encounter issues with the Tolstoy widget:

1. Check the browser console for any error messages.
2. Verify that the Tolstoy widget script is correctly loaded and initialized.
3. Ensure that you're using the correct Tolstoy ID when initializing or recreating the widget.
4. If problems persist, contact Tolstoy support for further assistance.
