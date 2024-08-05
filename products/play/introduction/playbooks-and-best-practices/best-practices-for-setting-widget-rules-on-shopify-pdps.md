## Best Practices for Setting Widget Rules on Shopify PDPs

When it comes to enhancing the user experience on Product Detail Pages (PDPs), establishing clear widget rules is essential. Widgets can significantly impact how users interact with PDPs. In this article, we will explore the importance of clear widget rules and provide guidance on how to establish them effectively to maintain a positive user experience.

### Setting Widget Rules

- **Include the URL Handle**: The handle is like a user-friendly ID for each product and is always the last part of a Shopify PDP URL. By using the handle, we can easily identify and set rules for the widget to show up on all product pages, regardless of the collection or other factors. This way, the widget will be consistently displayed across all product pages.

    **URL Includes**: `{handle}`  
    **Example**: URL includes: `fairy-floss-pink-hemp-shibari-rope`

    **Structure of a Shopify URL**: `https://${appUrl}/products/${handle}`  
    ![URL Structure](https://downloads.intercomcdn.com/i/o/744522867/40b2b550e1e1bfeb91c35cd3/image.png)

### Example Rules Pages

- **Include Widget on All Specific Product Pages**:  
    **URL**  
    Contains `fairy-floss-pink-hemp-shibari-rope`  
    ![Example Rule](https://downloads.intercomcdn.com/i/o/744503518/a6a0803c59097327d6ddd875/image.png)

- **Display Widget on Base PDP (Without Collection)**:  
    **URL**  
    Equals `https://lolliwraps.com.au/products/fairy-floss-pin`  
    ![Example Rule](https://downloads.intercomcdn.com/i/o/744509692/a5bd5535408671bf0c3b33a5/image.png)

- **Display Widget on PDP Through a Specific Collection**:  
    **URL**  
    Equals `https://lolliwraps.com.au/collections/fairy-floss-pin`  
    ![Example Rule](https://downloads.intercomcdn.com/i/o/744510600/7bca9d406631de2c86bb3c4a/image.png)"
