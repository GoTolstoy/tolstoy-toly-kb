## Embedding a Stories or Carousel in a Blog Post

1. In the Tolstoy App, click the **Onsite** tab and choose the stories or carousel you want to embed.

2. Click the dropdown alongside the **Published** button on the upper right.  
![image](https://github.com/user-attachments/assets/9eaa0987-8f0a-4626-b382-275995cad1a7)

3. Click **Use code instead** and copy the code.  
![image](https://github.com/user-attachments/assets/17a0d3f7-0138-4be2-82b3-4ace48c290b3)
![image](https://github.com/user-attachments/assets/e87c6872-6cd2-40c1-9a8e-f4eef12cad6f)

```html
<tolstoy-carousel
  data-tags="{% for tag in product.tags -%}{{ tag }},{%- endfor %}"
  class="tolstoy-carousel"
  data-publish-id="YOUR_PUBLISH_ID_HERE" 
  data-product-id="{{ product.id }}">
</tolstoy-carousel>
```

4. Go to your Shopify Blog Posts section and choose the blog post where you want the Tolstoy carousel to appear.  
![image](https://github.com/user-attachments/assets/25132f5b-92db-4661-a82f-f72573c9539f)

5. Click on **Show HTML**.  
![image](https://github.com/user-attachments/assets/45d25752-66a5-4d34-88a9-bc2f1b1b525a)

6. Paste the copied code where you want the Tolstoy carousel to appear.  
![image](https://github.com/user-attachments/assets/6ce189ee-58b6-4fec-a019-c8380ed76c67)

7. Save.  
![Step 6](https://tolstoy-2c549356d0c0.intercom-attachments-1.com/i/o/665227355/d735ce6b8280f944ff16e869/b63175b8-2443-4e80-9762-a66e03a696f9.png)

8. Done! The carousel will appear only on the chosen blog post.  
![Step 7](https://tolstoy-2c549356d0c0.intercom-attachments-1.com/i/o/665227358/cc1bddc3f058118bdfc53eae/cba149cc-4e73-417a-9f47-b998418ce6d1.png)