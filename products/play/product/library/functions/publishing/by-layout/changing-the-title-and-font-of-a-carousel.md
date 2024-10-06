## Changing the Title and Font of a Carousel

To change the title of your carousel, follow these steps:

1. Click on the **Design** tab, then click **Widget**.
   
   ![image](https://github.com/user-attachments/assets/340b64e1-692d-43e1-81a0-51fd8a48346c)

2. Turn on the toggle for **Title**. You have the option to set the Title Text size, Text weight, and Text color.
   
   ![image](https://github.com/user-attachments/assets/092c04b5-8ec9-4826-b197-59e49ef2a03f)

3. Turn on the toggle for the **Tile Name**. You can change the location, text size, and text color.
   
   ![image](https://github.com/user-attachments/assets/1f4c82e4-78a2-4d0a-85af-8c545ed7e56a)

This will help you enhance the visual appeal and provide context to your content with titles and tile names on your carousel.

To change the carousel title's font, you need to add custom CSS:

```css
.tolstoy-carousel-title {
    font-family: /* font name here */;
}
```

For stories:

```css
.tolstoy-stories-title {
    font-family: /* font name here */;
    /* other CSS customization if needed */
}
```