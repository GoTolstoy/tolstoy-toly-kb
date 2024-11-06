##how to fix add to cart not working?


Step 1: Open the Code Editor
Go to: Shopify Admin > Online Store > Themes.
Click Edit Code to open the theme’s code editor.

Step 2: Locate the theme.liquid File
In the theme editor sidebar, under Layout, click on theme.liquid.

Step 3: Insert the Code
Scroll to the end of the <head> section.
Paste the following code just above the </head> tag:

const subscribeToTolstoyAddToCartClick = () => {
  const myCallback = (payload) => {
    // Your logic here
  };

  const options = {};

  window.tolstoyWidget.subscribe("tolstoy_add_to_cart", myCallback, options);
};

if (window.tolstoyWidget) {
  subscribeToTolstoyAddToCartClick();
} else {
  window.addEventListener("tolstoyWidgetReady", () => {
    subscribeToTolstoyAddToCartClick();
    // Additional logic...
  });
}

Step 4: Customize the Code
Find the line in the pasted code that says // Your logic here.
Replace this comment with your own "Add To" function to define the custom functionality.

Step 5: Save the File
Once the code is added and customized, click Save to apply the changes.
