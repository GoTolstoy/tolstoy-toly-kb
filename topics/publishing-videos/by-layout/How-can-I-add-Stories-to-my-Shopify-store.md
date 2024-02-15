## How can I add Stories to my Shopify store?

Displaying stories is a great way to engage your customers and add more content to your Shopify store. You can easily display stories in your store in a few simple steps.
1. Create Tolstoy stories.
2. Click on Publish. (screenshot image of this step: https://downloads.intercomcdn.com/i/o/887797007/1ed691b0669479e5e10fecba/image.png)
3. Copy ID and click "Done". (screenshot image of this step: https://downloads.intercomcdn.com/i/o/887798503/ad2ff6da846c8a50d2714d99/image.png)
4. Go to your Shopify theme and click Customize. (screenshot image of this step: https://downloads.intercomcdn.com/i/o/686518798/4f2913b8b5c88aa190370be4/image.png)
5. Go to the App embeds panel and make sure that Tolstoy is toggled ON. (screenshot image of this step: https://downloads.intercomcdn.com/i/o/887799255/335746afa54580b2e7adb349/image.png)
6. Go to Sections. (screenshot image of this step: https://downloads.intercomcdn.com/i/o/840859757/3b597b0bdd9893f11a9a9629/9c80cd78-e34a-455e-86b3-efc0a74457b4)
7. Search and click on "Home page" if you want your stories to only appear on your home page. (screenshot image of this step: https://tolstoy-2c549356d0c0.intercom-attachments-1.com/i/o/686531724/7a757332907d005d0e2d6377/35cb81f8-55dd-40b2-8c1c-bcf82926a984.png)
8. Search and click on Products if you want your stories to appear only on your selected product pages. (screenshot image of this step: https://tolstoy-2c549356d0c0.intercom-attachments-1.com/i/o/686531733/fbdbf515325bc69be1dea0cd/d9ce0a5f-6702-4e33-a412-96b88495456c.png)
9. Click on Default product. Your stories will automatically appear on your PDPs. (screenshot image of this step: https://tolstoy-2c549356d0c0.intercom-attachments-1.com/i/o/686531740/0b520f542fa89d4b06d576e5/77ea5b88-9406-4d01-9a53-f95269eda6a9.png)
10. Click on + Add section or + Add block. (screenshot image of this step: https://tolstoy-2c549356d0c0.intercom-attachments-1.com/i/o/686531747/186e2bd7ea564f84e22a2715/45f4ff53-dff4-4891-8886-4aab8446d6b6.png)
11. Type "tolstoy stories" and click on it. (screenshot image of this step: https://tolstoy-2c549356d0c0.intercom-attachments-1.com/i/o/686531755/3681a57dfd212559a383bef7/987afdf1-d221-44e4-858c-7b0a43419575.png)
12. Paste the Publish ID, and click "Save". (screenshot image of this step: https://tolstoy-2c549356d0c0.intercom-attachments-1.com/i/o/686531761/1f3504c82cabcc4e3fd5a6da/147918f2-0366-4be9-a3b2-ddd8ff3eec8b.png)


If you can’t find “Tolstoy Story” in your Shopify sections, copy the following code and paste it into your page, in the position you desire.


    <tolstoy-stories
      data-tags="{% for tag in product.tags -%}{{ tag }},{%- endfor %}"
      class="tolstoy-stories"
      data-publish-id="PASTE ID HERE" 
      data-product-id="{{ product.id }}">
    </tolstoy-stories>


You can find the code by clicking the drop-down alongside the Publish/Pause button, then </> Use code instead. (screenshot image: https://downloads.intercomcdn.com/i/o/887802984/95f28485cdd2db7062687551/image.png)
​
Go to your Shopify theme, click on the three dots, and choose Edit code. (screenshot image: https://downloads.intercomcdn.com/i/o/686865258/fa415b4c597ae70d6d16b115/image.png)
Type product in the search field. It's usually under Sections or Snippets, click on product-template.liquid and paste the code into your product page's template liquid in your desired position.
