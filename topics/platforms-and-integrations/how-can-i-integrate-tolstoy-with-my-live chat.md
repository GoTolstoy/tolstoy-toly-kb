## How to Integrate Tolstoy with Live Chat

Ready to integrate live chat with your Tolstoy? If you're using Intercom, Gorgias, tawk.to, LiveChat, HelpScout, Drift, or HubSpot, you can simply add this chat feature through your Tolstoy builder:

1. In Tolstoy Dashboard > Go to Onsite > select the Tolstoy Widget that you want to integrate the chat > then go to Videos tab.
2. Click on the circled button to open the drop-down menu of answer options. (screenshot image of this step: ![Step 1](https://downloads.intercomcdn.com/i/o/850642889/4727b78e50b717d1e2add1b7/faab633b-39c7-43ae-9f26-52bf9ee1f3b0))
3. Select Other and then, Chat.
4. Open up this new drop-down menu to see the available live chat platforms you can connect to.
5. Choose the live chat platform that you want to use and click Save!

As long as you have the live chat platform installed on the site that you selected, then you're good to go. Users can click on the button, and it will automatically open up the live chat.

### Integrating Tolstoy with a Different Live Chat Platform

If the platform you used isn't mentioned above, then add the following code to your site to enable live chat within your Tolstoy:

**This is an example of the complete code for Drift**:

```javascript
// setting the Tolstoy widget to display
window.tolstoyWidgetId = 'bidu9d2bedptm';
// Hide the chat widget - drift **
window.drift.api.widget.hide();
// Catch button click in Tolstoy
window.addEventListener('message', function(message) {
  if (message.data.name === 'tolstoyAnswerClicked' && message.data.text === 'Chat with me') {
    // show the widget ***
    window.drift.api.toggleChat();
    // hide the Tolstoy
    window.tolstoyWidget.hide();
  }
});
</script>
<script async src="https://widget.gotolstoy.com/widget.js"></script>
```
As this is an example code for Drift, you will need to replace the lines of code in bold (labeled with **) that match the code for your specific platform for hiding and opening the chat widget.

Note: The text "Chat with me" within the code should match the text you display on the button you use in your Tolstoy to open live chat.

Place this code where you want it to appear on your site!