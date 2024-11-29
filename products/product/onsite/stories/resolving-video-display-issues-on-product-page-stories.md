# Resolving Video Display Issues on Product Page Stories

## Understanding the Issue

If you notice that all your videos are showing up on the product page stories instead of just the stories per the style, it is likely due to the preview page within the app not holding the product ID set in your product page stories. This can cause all the stories to be displayed rather than the specific ones intended for each product.

## Solution

### Preview Page

The preview page within the app is designed to show all the stories because it does not retain the product ID. This is a known behavior and is not indicative of an error in your setup.

### Staging Site Configuration

To ensure that the correct stories are displayed on your staging site, you need to verify that the Tolstoy app block or stories are properly configured in your Shopify theme. Follow these steps:

1. **Access Your Shopify Theme**: Go to your Shopify admin panel and navigate to the 'Themes' section.
2. **Edit Code**: Click on 'Actions' and then 'Edit Code' for the theme you are using.
3. **Locate Tolstoy App Block**: Find the section where the Tolstoy app block or stories are integrated.
4. **Verify Configuration**: Ensure that the configuration settings are correct and that the product ID is properly set for each product page story.

By following these steps, you can ensure that only the relevant stories are displayed for each product, providing a more tailored and accurate experience for your users.