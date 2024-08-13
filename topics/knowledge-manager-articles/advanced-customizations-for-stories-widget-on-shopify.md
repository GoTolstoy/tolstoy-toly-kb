# Advanced Customizations for Stories Widget on Shopify

This guide provides detailed instructions on implementing advanced customizations for the Stories widget on Shopify, with a focus on collapsing the product section by default.

## Introduction
Customizing the Stories widget allows for a tailored shopping experience on your Shopify store. This guide covers the steps needed to modify the widget beyond the standard settings available through the Tolstoy dashboard.

## Collapsing the Product Section by Default
To set the product section of the Stories widget to collapse by default, you will need to modify your Shopify theme's code or add custom JavaScript. Here are the steps:
1. Access your Shopify admin panel.
2. Navigate to 'Online Store' > 'Themes'.
3. Choose 'Edit code' from the Actions menu for your current theme.
4. Locate the file that includes the Stories widget integration (typically involves liquid files or JavaScript snippets).
5. Insert the following JavaScript code snippet at the appropriate place in your file:

```javascript
// JavaScript to collapse the product section in Stories widget
document.addEventListener('DOMContentLoaded', function() {
  var productSection = document.querySelector('.stories-widget .product-section');
  if (productSection) {
    productSection.style.display = 'none';
  }
});
```

## Conclusion
By following these steps, you can customize the Stories widget to collapse the product section by default, enhancing the user experience and aligning with specific design preferences for your Shopify store.