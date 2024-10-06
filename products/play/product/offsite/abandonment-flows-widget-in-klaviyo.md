# Abandonment Flows Widget in Klaviyo

The Abandonment Flows widget in Klaviyo is a powerful new feature that allows you to dynamically populate videos based on product IDs featured in your email flows.

## Getting Started

Select "Abandonment Flows" to begin creating your widget.

![1 1](https://github.com/user-attachments/assets/2e6e556b-b2f1-41f8-b733-b717074dc66f)

Note: This feature is currently only available for Klaviyo users and does not support other email tools.

## Selecting Videos

1. By default, the Product Tagged Playlist will be selected.
2. You'll see different groupings of videos based on product tags.

![1 2](https://github.com/user-attachments/assets/b0968042-f3df-414b-bb47-973fd5b66f67)

## GIF Configuration

Link to:

- For Abandonment Flows, videos only redirect to product pages dynamically, opening the video on that product page.

UTM Parameters:

- Add UTM parameters for tracking and analytics tools like Google Analytics.
- This will help track traffic coming from users who click the GIF to your store.
- Important: After adding UTM parameters, you must re-copy and paste the widget code.

Fallback Playlist:

- Select a fallback playlist to populate the GIF if there are fewer than three videos tagged for a product.
- Example: If you have a 100-product catalog but only 70 have videos, the fallback playlist will be used for the remaining 30 products. If a product has 2 videos, the fallback will only be used for the missing 3rd video.
- Note: Videos from the fallback playlist will redirect to the product page but will not play on the page itself.

![1 3](https://github.com/user-attachments/assets/0ca814c5-c4c9-47cc-94a3-cdfe0dc07f95)

## Video Feed Behavior

To change whether you want the video to open in full screen or picture-in-picture mode:

- Go to the "Video Feed" section
- Toggle the "View Feed in full screen" option as desired

![1 4](https://github.com/user-attachments/assets/c891f8f6-abd8-4d36-9ade-6b7715243ad6)

## Publishing Your Widget

### In Tolstoy

1. Copy the provided code snippet.
2. There's no need to select your email tool, as it's only available for Klaviyo.

![1 5](https://github.com/user-attachments/assets/e1d6205b-d73c-4a7e-8d44-8542998bfc6a)

### In Klaviyo

1. Go to an email flow in Klaviyo.
2. Edit one of the templates.
3. Add the HTML code using either:
   - The source code for a block
   - Native HTML code implementation

![1 6](https://github.com/user-attachments/assets/53557d1e-f8ec-4302-971f-2bc9dfa46765)

![1 7](https://github.com/user-attachments/assets/e08a924a-6e43-40b5-a7db-40240cb12ea5)

### Previewing Your Widget

1. To preview the GIF, click on "Preview and Test" in Klaviyo.
2. Since the widget dynamically populates videos, you can swipe through events to see different implementations for each product.

![1 8](https://github.com/user-attachments/assets/45def35b-6a05-45bc-88e8-9b7b923bdb11)

![1 9](https://github.com/user-attachments/assets/363ff79d-5b13-4311-9412-963420603c08)

## Troubleshooting

If you don't see the GIF even though there is a fallback playlist set up, please contact support for assistance.