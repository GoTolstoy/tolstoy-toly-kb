## how to publish stories using code blocks
For Shopify V1 

1. Log into your Shopify admin. 
2. Go to the page where you want to add the block.  
3. Click on the page editor. 
4. Add a Custom Liquid section where you want the block to appear. 
5. Go to your Tolstoy dashboard, find the project you want to publish and copy the code provided inside the publish button under No app blocks? Use code instead.
   
![image](https://github.com/user-attachments/assets/52dc7f62-cf15-43c4-afe8-93f029143822)

​Stories code: 
​
<tolstoy-stories
data-tags="{% for tag in product.tags -%}{{ tag }},{%- endfor %}"
class="tolstoy-stories"
data-publish-id="PUBLISH ID" 
data-product-id="PRODUCT_ID">
</tolstoy-stories>

6. Paste this code into the Custom liquid section in Shopify.
7. Save your changes.


​For Native 

1. Go to your Tolstoy dashboard, find the project you want to publish and copy the code provided inside the publish button under No app blocks? Use code instead.
   
![image](https://github.com/user-attachments/assets/d7e6fb84-7f28-4b5b-bf20-90a128b79661)

 ​Stories code: 
​
<tolstoy-stories
data-tags="{% for tag in product.tags -%}{{ tag }},{%- endfor %}"
class="tolstoy-stories"
data-publish-id="PUBLISH ID" 
data-product-id="PRODUCT_ID">
</tolstoy-stories>
​

2. Paste the code anywhere into your HTML.
3. Save your changes. 



**How to find your publish ID**

For Shopify
Go to your Shopify Admin dashboard.

Click on Products to view your product list.

Click on the product you want to link.

In the URL of your browser while viewing the product, the number at the end after /products/ is the product ID.
​

For Other Platforms/ Native websites

 

The method is similar: look for the product in your platform's product management section and use the unique identifier given in the URL or product details section. Usually, this can be found on your website.
