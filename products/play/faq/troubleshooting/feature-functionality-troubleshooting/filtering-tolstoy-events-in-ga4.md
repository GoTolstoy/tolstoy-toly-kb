## Filtering Tolstoy Events in GA4

To filter Tolstoy events in Google Analytics 4 (GA4), you can use Google Tag Manager (GTM) or manually add code to handle specific events. Here are the steps for each method:

### Using Google Tag Manager (GTM)
1. **Create a Trigger:** In GTM, create a trigger that fires only for the 'tolstoyStarted' event.
2. **Block Other Events:** Set up a blocking trigger to prevent other Tolstoy events from being sent to GA4.
3. **Publish Changes:** Save and publish your changes in GTM.

### Manually Adding Code
1. **Identify Events:** Identify the specific Tolstoy events you want to track, such as 'tolstoyStarted'.
2. **Add Code:** Manually add code to your website to handle these specific events and block others.
3. **Test and Deploy:** Test your implementation to ensure only the desired events are being tracked, then deploy the changes.

By following these steps, you can effectively filter Tolstoy events in GA4 to focus on the most relevant data.