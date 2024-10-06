# Preventing Cropped Product Images

When displaying product images, especially within product tiles or grids, images may appear cropped or cut off. This happens because the default CSS behavior might be set to `object-fit: cover`, which ensures the image covers its container but often results in important parts of the image being hidden.

To prevent product images from being cropped and to display the full image within its container, we will change the `object-fit` property to `fill`. This will stretch the image to fit the container, ensuring the entire image is visible.

## CSS Code Implementation

The following CSS code modifies the product image display to prevent cropping:

```css
.tolstoy-product-tile-image {
    object-fit: fill !important;
}
```