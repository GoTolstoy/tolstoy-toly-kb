## Integrating Tolstoy with Live Chat

Ready to integrate live chat with your Tolstoy? If you're using Intercom, Gorgias, tawk.to, LiveChat, HelpScout, Drift, or HubSpot, you can simply add this chat feature through your Tolstoy builder:

1. In Tolstoy Dashboard, go to Onsite, select the Tolstoy Widget that you want to integrate the chat with, then go to the Videos tab.
   ![image](https://github.com/user-attachments/assets/f93d7193-cb2b-4c75-897c-37600b91aa32)

2. Click on the circled button to open the drop-down menu of answer options.
   ![image](https://github.com/user-attachments/assets/e90425a6-9287-416d-b1e8-42ac06d53927)

3. Select Other and then Chat.
   ![image](https://github.com/user-attachments/assets/d92b44c0-ea0e-49c2-9e28-19ae1cd8b684)
   ![image](https://github.com/user-attachments/assets/f6da4008-0522-44ae-b714-901fa854576d)

4. Open up this new drop-down menu to see the available live chat platforms you can connect to.
   ![image](https://github.com/user-attachments/assets/3ab91065-0cdd-4455-ab2a-14e3583d6b73)

5. Choose the live chat platform that you want to use and click Save!
   ![image](https://github.com/user-attachments/assets/c3c90c38-1c2a-4a91-9be2-7b8d41451c12)

As long as you have the live chat platform installed on the site that you selected, you're good to go. Users can click on the button, and it will automatically open up the live chat.

### Integrating Tolstoy with a Different Live Chat Platform

If the platform you use isn't mentioned above, then add the following code to your site to enable live chat within your Tolstoy:

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
