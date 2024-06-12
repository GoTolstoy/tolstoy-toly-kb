## How can I add a Carousel to my Shopify store?

1. Go to Onsite -> Create Tolstoy. 

![image](https://github.com/GoTolstoy/tolstoy-toly-kb/assets/159800692/a1f4832f-188d-4384-a5d3-05e1c1ab6191)


2. Create from scratch

![image](https://github.com/GoTolstoy/tolstoy-toly-kb/assets/159800692/c33ddf41-c2b3-415f-b21f-651721560bd5)


3. Choose Carousel.

![image](https://github.com/GoTolstoy/tolstoy-toly-kb/assets/159800692/5a3097da-661f-40d2-81f8-f3c224c2cd52)



4. Decide where you want to put Tolstoy: Homepages, Product pages, Collection pages, or Other pages.

![image](https://github.com/GoTolstoy/tolstoy-toly-kb/assets/159800692/56ad813e-585a-49d0-8411-c184a2197940)



5. Go to your Shopify theme and click Customize.

![image](https://github.com/GoTolstoy/tolstoy-toly-kb/assets/159800692/21bc813e-1b48-4bf4-822c-8cc3ddfeb6a9)



6. Before you can set this Tolstoy live, please enable the Tolstoy app on your theme -> App embeds (once per store), if you haven't done this already.

![image](https://github.com/GoTolstoy/tolstoy-toly-kb/assets/159800692/9830b92a-511f-47ea-b2f9-5bb964abe128)



7. Search and click on the Home page if you want your carousel to only appear on your home page.

![image](https://github.com/GoTolstoy/tolstoy-toly-kb/assets/159800692/d42d211c-2a76-4689-9280-f96e34b96740)



8. Search and click on Products if you want your carousel to appear only on your selected product page/(s).

![image](https://github.com/GoTolstoy/tolstoy-toly-kb/assets/159800692/af53de73-063e-4c9e-a494-585b66294d2b)



9. Click on Default product. Your carousel will automatically appear on the PDP/(s) using "Product tagged" playlist.

![image](https://github.com/GoTolstoy/tolstoy-toly-kb/assets/159800692/b0d197f2-d922-4f18-8f19-9145c76d401f)



10. Click on + Add block or + Add section.

![image](https://github.com/GoTolstoy/tolstoy-toly-kb/assets/159800692/6f00e340-907a-4714-8ec9-826a1bd10091)



11. Type "Tolstoy carousel" and click on it.

![image](https://github.com/GoTolstoy/tolstoy-toly-kb/assets/159800692/c02e2402-bd8a-488c-8c8f-66aa72006c90)



12. Paste the Publish ID then, click on Save.

![image](https://github.com/GoTolstoy/tolstoy-toly-kb/assets/159800692/14d87092-a7bd-4366-84cd-36f7e334073a)



If you can't find the 'Tolstoy carousel' on your Shopify product page, copy the code by clicking on the "Published" button in the Tolstoy app.

![image](https://github.com/GoTolstoy/tolstoy-toly-kb/assets/159800692/3266c8d5-ca2f-42a4-8125-09e3a3822875)


Go to your Shopify theme, click on the three dots, and choose Edit code.

![image](https://github.com/GoTolstoy/tolstoy-toly-kb/assets/159800692/ce571b6c-e246-484b-9659-bfc045630b26)


​Type product in the search field. Under Sections or Snippets, whichever is applicable, click on product-template.liquid and paste the code into your product page's template liquid in your desired position. 


### Carousel's Title Font


This is how to make the title go with the site's font.


Add this code to the carousel's code in the custom liquid. Change the **<your own font>** to the font's code.

.tolstoy-carousel-title 
{ 
font-family:<your own font> !important; 
}
