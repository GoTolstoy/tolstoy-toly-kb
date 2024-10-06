## Triggering an Event When a Product is Added to Cart Through a Tolstoy Video Card

Here's the code to subscribe to our events.

```javascript
function openMiniCartModal(productHandle) {
    if (window.CustomCartHandler && typeof window.CustomCartHandler.openMiniCart === "function") {
        window.CustomCartHandler.openMiniCart(productHandle);
    } else {
        console.error("CustomCartHandler or openMiniCart method is not available");
    }
}

function subscribeToQuickShopClick() {
    window.tolstoyWidget.subscribe(
        "tolstoy_spotlight_carousel_quick_shop_click",
        function(eventData) {
            if (eventData.product && eventData.product.handle) {
                openMiniCartModal(eventData.product.handle);
            } else {
                console.error("Product handle is not available in the event");
            }
        },
        { disableDefault: true }
    );
}

if (window.tolstoyWidget) {
    subscribeToQuickShopClick();
} else {
    window.addEventListener("tolstoyWidgetReady", subscribeToQuickShopClick);
}
```