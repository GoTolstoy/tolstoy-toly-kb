# Adding a Quick Purchase Button to Product Pages Using Tolstoy

## Introduction
Adding a quick purchase button to your product pages can significantly enhance the user experience by allowing customers to make purchases with fewer clicks. Tolstoy supports this feature through their JavaScript SDK. This article will guide you through the steps to implement a quick purchase button on your product pages using Tolstoy.

## Step-by-Step Implementation

### Step 1: Subscribe to the Event
First, you need to subscribe to the `tolstoy_spotlight_carousel_quick_shop_click` event. This event is triggered when a user clicks on the quick purchase button.

```javascript
// Subscribe to the quick shop click event
Tolstoy.on('tolstoy_spotlight_carousel_quick_shop_click', function(event) {
    // Your code to handle the event
    console.log('Quick shop button clicked', event);
});
```

### Step 2: Open the Mini Cart Modal
Next, use the `openMiniCartModal` function to open the mini cart modal when the event is triggered. This function will allow users to quickly add items to their cart and proceed to checkout.

```javascript
// Function to open the mini cart modal
function openMiniCartModal(productId) {
    // Your code to open the mini cart modal
    Tolstoy.openMiniCartModal({
        productId: productId
    });
}

// Subscribe to the quick shop click event and open the mini cart modal
Tolstoy.on('tolstoy_spotlight_carousel_quick_shop_click', function(event) {
    openMiniCartModal(event.productId);
});
```

## Conclusion
By following these steps, you can easily add a quick purchase button to your product pages using Tolstoy. This feature will help streamline the purchasing process for your customers, potentially increasing your conversion rates.