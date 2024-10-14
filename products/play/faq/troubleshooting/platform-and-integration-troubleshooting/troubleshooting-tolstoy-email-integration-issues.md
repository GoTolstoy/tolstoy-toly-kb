## Troubleshooting Tolstoy Email Integration Issues

When integrating Tolstoy with email platforms, you might encounter situations where the integration works for some emails but fails for others. One common cause of this issue is related to how Klaviyo passes the product ID to Tolstoy.

### Understanding the Issue

For Tolstoy to function correctly, it needs the correct product ID to forward users to the appropriate product page and play the relevant videos. If the variant ID is not correctly passed from Klaviyo to Tolstoy, the integration will fail for those specific emails.

### Steps to Resolve

1. **Check Product ID Passing:** Ensure that Klaviyo is correctly passing the product ID to Tolstoy. This involves verifying the integration settings and the data being sent.
2. **Verify Variant ID:** Make sure that the variant ID is included and correctly formatted in the data passed to Tolstoy.
3. **Test Different Emails:** Send test emails to see if the issue persists across different products and email templates. This can help identify if the problem is isolated to specific products or templates.
4. **Consult Documentation:** Refer to Tolstoy and Klaviyo documentation for detailed instructions on setting up the integration and troubleshooting common issues.

By ensuring that the product and variant IDs are correctly passed from Klaviyo to Tolstoy, you can resolve most integration issues and ensure a seamless experience for your users.