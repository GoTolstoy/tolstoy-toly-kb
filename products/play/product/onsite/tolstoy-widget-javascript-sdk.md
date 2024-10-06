# Tolstoy Widget JavaScript SDK

## 1. Introduction

This technical reference guide provides comprehensive documentation for the Tolstoy Widget JavaScript SDK. It is designed to assist developers in integrating and customizing the Tolstoy floating widget into their websites. The guide covers configuration options, available methods, best practices for implementation, and troubleshooting tips.

The Tolstoy widget is a powerful tool for adding interactive, customizable content to your website. Whether you're looking to enhance user engagement, provide product demonstrations, or offer interactive customer support, this SDK gives you the flexibility to tailor the widget to your specific needs.

## 2. Key Concepts and Terminology

Before diving into the technical details, it's important to understand the key concepts and terminology used throughout this guide:

- **Tolstoy Widget**: A customizable floating widget that can be integrated into websites to provide interactive content.
- **Widget Configuration**: Settings that control the widget's behavior and appearance.
- **Widget Methods**: JavaScript functions provided by the SDK to interact with the widget programmatically.
- **Events**: Specific occurrences in the widget's lifecycle that can trigger custom actions.
- **Tolstoy ID**: A unique identifier for your specific widget instance.
- **Widget Bubble**: The initial, collapsed state of the widget that appears on the user's screen.
- **Widget Expansion**: The process of opening the widget from its bubble state to its full-size view.

## 3. Technical Specifications

### 3.1 Widget Configuration

The Tolstoy widget is configured using the `window.tolstoySettings` object. Here are the available settings:

| Setting | Type | Default | Description |
|---------|------|---------|-------------|
| `alwaysShow` | boolean | `true` | Controls whether the widget remains visible after being closed. |
| `loadHidden` | boolean | `true` | Determines if the widget should load in a hidden state. |
| `stopPreviewLoop` | boolean | `true` | Prevents the preview window from looping continuously. |
| `noCloseOption` | boolean | `true` | Removes the option for users to close the widget. |

Example configuration:

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

### 3.2 Widget Methods

The SDK provides several methods to control the widget's behavior, accessible through the `window.tolstoyWidget` object:

#### start()
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

#### startPart(partNumber)
Starts the widget at a specific part number.

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

#### show()
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

#### hide()
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

#### recreate(tolstoyWidgetId, settings)
Loads a new widget with a different Tolstoy ID.

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

#### on(eventType, callback)
Registers a callback function to be triggered on a specific event.

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

Supported event types:
- `"onWidgetOpen"`: Triggered when the widget is opened
- `"onWidgetClose"`: Triggered when the widget is closed
- `"onWidgetReady"`: Triggered when the widget is ready
- `"onTolstoyClose"`: Triggered when the Tolstoy bubble is closed

### 3.3 Additional Functionality

#### Reject Cookie Policy
Use this method when a user rejects the cookie policy:

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

## 4. Best Practices

To ensure optimal performance and user experience when implementing the Tolstoy Widget, consider the following best practices:

1. **Script Loading**: Always ensure that the Tolstoy widget script is loaded before using any of the SDK methods. You can do this by placing the script tag at the end of your HTML body or using async/defer attributes.

2. **Initialization**: Use the `onWidgetReady` event to make sure the widget is fully loaded before interacting with it. This prevents potential errors from calling methods on an uninitialized widget.

   ```javascript
   window.tolstoyWidget.on("onWidgetReady", () => {
     // Widget is ready, safe to call methods now
     console.log("Tolstoy Widget is ready");
   });
   ```

3. **User Experience**: Carefully consider settings like `alwaysShow` and `noCloseOption`. While these can increase engagement, they may also frustrate users if not implemented thoughtfully.

4. **Performance**: If you're not using the widget immediately on page load, consider using the `loadHidden` option to improve initial page load times.

5. **Responsive Design**: Ensure that your website's layout accommodates the widget at various screen sizes. The widget should not obstruct important content or functionality.

6. **Testing**: Thoroughly test the widget in different scenarios and on various devices to ensure consistent behavior across your user base.

7. **Error Handling**: Implement try-catch blocks when calling widget methods to gracefully handle any potential errors.

   ```javascript
   try {
     window.tolstoyWidget.start();
   } catch (error) {
     console.error("Error starting Tolstoy widget:", error);
     // Handle the error appropriately
   }
   ```

8. **Analytics Integration**: Utilize the event callbacks to integrate with your analytics tools, allowing you to track widget usage and user engagement.

## 5. Troubleshooting

If you encounter issues with the Tolstoy widget, follow these troubleshooting steps:

1. **Check Console Errors**: Open your browser's developer tools and check the console for any error messages related to the Tolstoy widget.

2. **Verify Script Loading**: Ensure that the Tolstoy widget script is correctly loaded and initialized. You should see no 404 errors related to the script in your network tab.

3. **Confirm Tolstoy ID**: Double-check that you're using the correct Tolstoy ID when initializing or recreating the widget. An incorrect ID will prevent the widget from loading properly.

4. **Test in Incognito Mode**: If the widget isn't appearing, try loading your page in an incognito/private browsing window to rule out any caching issues or conflicts with browser extensions.

5. **Check for Conflicts**: If you're using other JavaScript libraries or widgets, temporarily disable them to see if they're conflicting with the Tolstoy widget.

6. **Validate Configuration**: Review your `window.tolstoySettings` object to ensure all properties are set correctly.

7. **Browser Compatibility**: Test the widget in different browsers to identify any browser-specific issues.

If problems persist after following these steps, contact Tolstoy support for further assistance. Be prepared to provide:
- Your Tolstoy widget ID
- A description of the issue
- Steps to reproduce the problem
- Any relevant console errors
- Browser and device information

## 6. Related Resources

For more information and support, refer to these additional resources:

- [Tolstoy Official Website](https://www.gotolstoy.com/)
- [Tolstoy Developer Documentation](https://developers.gotolstoy.com/welcome)

For further assistance or to report issues, please contact Tolstoy support through their official channels.

By following this guide and leveraging the provided resources, you should be well-equipped to integrate and customize the Tolstoy Widget effectively in your web projects.