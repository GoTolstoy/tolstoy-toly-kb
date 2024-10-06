## Extracting Custom Fields from Tolstoy with Zapier

If you are using the Tolstoy X Zapier integration, there are certain fields that you may want to extract that are not available using the regular Zap settings. Follow this guide to learn how to extract custom fields using advanced configuration. *Requires a Premium Zapier account.*

1. **Integrate Tolstoy with Zapier.**
2. **Begin setting up the Zap Trigger from Tolstoy.**  
   ![Screenshot](https://downloads.intercomcdn.com/i/o/430361111/6f8fb10c5472031f192375fc/image.png)
3. **Add a new Action and select Format.**  
   ![Screenshot](https://downloads.intercomcdn.com/i/o/430381548/976e75886e6153183d6b4717/image.png)
4. **Choose Utilities.**  
   ![Screenshot](https://downloads.intercomcdn.com/i/o/430382143/9f0721e85870670e2082a7a3/image.png)
5. **Under Set up action, select Line-item to Text.**  
   ![Screenshot](https://downloads.intercomcdn.com/i/o/430384222/90aebc45472c9ea32f58898f/image.png)

Make sure you give names to all your Tolstoy parts!

6. **In the Input, open the drop-down menu.** First select "Events Question", then "-", then "Events Event Name", then "***", and then add the "Events Text".

   In the Separator field, write "|||", and click Test and Continue, like this:  
   ![Screenshot](https://downloads.intercomcdn.com/i/o/430385061/ddba156b798042d3ba366ca4/image.png)

7. **Close the section and add a new action.** Search for the Code by Zapier app.  
   ![Screenshot](https://downloads.intercomcdn.com/i/o/430386009/1f1d394c9513e6ff78f90c12/image.png)
8. **In the Input Data, type text, and then select the Output Text from the Utilities.**  
   ![Screenshot](https://downloads.intercomcdn.com/i/o/430388320/8cdf4ea16dcae7bb707575e3/image.png)
9. **In the code section, type the following code:**

   ```javascript
   const text = inputData.text.split('|||');
   let obj = {};
   text.forEach((element) => {
     const [name, value] = element.split('***');
     obj[name] = value;
   });
   output = [obj];
   ```

10. **Click Continue and Test and Continue.** Now you will have the part name, the event name, and the text value that was entered.  
    ![Screenshot](https://downloads.intercomcdn.com/i/o/430389079/f6f377e6de8cd2d34f318eff/image.png)

You can easily choose the desired value and match it to the wanted field in Zapier!

*Based on this [article](https://community.zapier.com/featured-articles-65/how-to-parse-keys-and-values-from-line-item-arrays-into-zapier-mappable-values-7493) by Zapier.*