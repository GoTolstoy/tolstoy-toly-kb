# Fixing Carousel Arrow Alignment on Collection Pages

If you're experiencing issues with the alignment of carousel arrows on your collection pages, you can resolve this by adding a specific CSS code snippet. This adjustment will ensure that the arrows are properly aligned, enhancing the overall user experience on your site.

To fix the alignment, add the following CSS code to your stylesheet:

```
.tolstoy-next-button {
  margin-bottom: 7px !important;
}
```

This code targets the `tolstoy-next-button` class and adjusts the bottom margin to 7 pixels, ensuring the arrows are correctly positioned. Make sure to include the `!important` declaration to override any other styles that might be affecting the alignment.