# Using Carousels on GemPages

This article provides a detailed guide on how to effectively use carousels on GemPages, covering all steps from creation to publication, including code snippets and troubleshooting tips.

## Step 1: Create the Carousel
- Go to the Tolstoy Dashboard.
- Select 'Onsite' and create a Carousel.

## Step 2: Publish the Carousel
- Click the **Publish** button after creation.
- Copy the Publish ID.

## Step 3: Add to GemPages
- Open your Shopify store and navigate to the GemPages app.
- Edit the page where you want to add the Carousel.

## Step 4: Insert Tolstoy Carousel
- In GemPages, add a new HTML/Liquid element to the page.
- Paste the following code snippet, replacing `YOUR_PUBLISH_ID` with the Publish ID you copied:

   ```html
   <div id='tolstoy-carousel' data-tolstoy-id='YOUR_PUBLISH_ID'></div>
   <script src='https://cdn.gotolstoy.com/loader.js' async></script>
   ```

## Step 5: Save and Publish
- Save your changes in GemPages and publish the page.

## Troubleshooting
- If the carousel does not display correctly, ensure that the Publish ID is correctly inserted.
- Check for any syntax errors in the HTML code.
- Ensure that the GemPages and Tolstoy scripts are not being blocked by any browser extensions.

By following these steps, you can successfully integrate a Tolstoy carousel into your GemPages site, enhancing the visual appeal and functionality of your pages.