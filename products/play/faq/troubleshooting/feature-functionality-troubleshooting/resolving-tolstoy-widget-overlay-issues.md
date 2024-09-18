# Resolving Tolstoy Widget Overlay Issues

When integrating the Tolstoy widget into a website, a common technical issue that may arise is the widget covering overlay elements such as email capture pop-ups and mini cart drawers. This can disrupt the user experience by making these important elements inaccessible.

## Solution

The issue was resolved by adjusting the widget's **z-index**. The z-index is a CSS property that controls the vertical stacking order of elements on a web page. By setting an appropriate z-index value for the Tolstoy widget, it ensures that the widget does not cover other overlay elements.

### Steps to Adjust the z-index
1. **Identify the z-index values**: Determine the z-index values of the overlay elements that are being covered by the Tolstoy widget.
2. **Set the widget's z-index**: Adjust the z-index of the Tolstoy widget to a value that is lower than the overlay elements. This can be done through CSS.

```css
/* Example CSS to adjust the z-index of the Tolstoy widget */
.tolstoy-widget {
  z-index: 1000; /* Set this value appropriately */
}
```

3. **Test the changes**: After adjusting the z-index, test the website to ensure that the overlay elements are no longer covered by the Tolstoy widget.

By following these steps, the issue of the Tolstoy widget covering overlay elements can be effectively resolved, ensuring a seamless user experience.