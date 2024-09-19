## Collection page videos

[Video tutorial](https://www.loom.com/share/03c040bdf4e441ccb7f998805bd84d1d?sid=16e0d010-e4d5-447f-bf22-3b4f3058ffb2)


Collection page videos allow brands to enhance their collection pages with dynamic video content, replacing static product images with engaging videos. By incorporating videos into your collection pages, you can showcase your products in a visually appealing and interactive way, encouraging customers to click through to your product pages.

Collection page videos seamlessly integrate with your existing product listings and offer the following features:

- Replace product images with videos on collection pages
- Limit the number of videos per page to avoid overwhelming customers
- Space out videos across the collection page for a balanced presentation

**Set-up**


Assigning Videos to Products

To assign a video to a product for use on collection pages, follow these simple steps:

1. Open a Collection videos project in the Onsite tab.

2. Navigate to the Videos section in your admin panel

3. Select the product you want to assign a video to and choose the desired video for the product

4 The selected video will appear and be associated with the product

Once you’ve implemented the code in your liquid, the videos will replace the product images whenever the product is loaded on the collection page (regardless of if it’s in e.g. Bestsellers or Lipsticks), subject to the restrictions set in the Design configuration (see below).

**Configuring Collection Page Video Settings**

To customize the behavior and appearance of collection page videos:

1. Go to the Design section in your admin panel

2. Adjust the following settings as needed:

- Auto-play: Enable or disable automatic video playback

- Playback mode: Choose between consecutive (one after another) or simultaneous playback

- Delay: Set a delay before video playback begins (if auto-play is enabled)

- Product image display: Show the product image when the video isn't yet playing on Autoplay

- Maximum videos per page: Limit the number of videos displayed on a single collection page

- Minimum product spacing: Set the minimum number of products between videos

- Please note, the two below features require the code to be implemented carefully by a developer, above the product card’s <a>

--Click behavior: Determine if clicking the video sends users to the product page or plays/pauses the video

--Controls: Add play or mute buttons as needed

**Installation:**

Please consult with a developer to add the below code or reach out to our support to implement. Exact implementation will depend on your site’s setup for the videos to replace the product images.

Please note, for the video controls and click-through analytics to be functional, the code must be placed above the product card’s <a>

1. Go to your theme’s liquid section of the main collection product grid
![image](https://github.com/user-attachments/assets/2daf9bfe-e24f-41b4-afa0-3792b092480e)


2. Find the section within the liquid code where the product cards are rendered to identify product card file
![image](https://github.com/user-attachments/assets/04b9d9c9-4a06-45f4-a463-f0ed989d1d81)

3. Go to the product card’s liquid file and search for an img
![image](https://github.com/user-attachments/assets/c581c269-bd2f-49fe-adab-c23807183f57)


4. Put the provided code in the same container as the image as first 
![image](https://github.com/user-attachments/assets/dd99055e-f547-4216-9118-b477033c97d6)


**Best Practices**

To make the most of the collection page video feature, consider the following best practices:

- Select high-quality, visually compelling videos that effectively showcase your products

- Use concise videos that quickly capture the essence of the product

- Experiment with playback settings to find the right balance for your brand and customers

- Regularly update your video content to keep your collection pages fresh and engaging

By following these guidelines and leveraging the collection page video feature, you can create a more dynamic and engaging shopping experience for your customers, potentially increasing product discovery and sales.
