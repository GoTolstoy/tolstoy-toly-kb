## How to Upload Your Product Catalog via CSV

This guide will walk you through how to upload your product catalog to Tolstoy using a CSV file. If you need to display product data (such as images, prices, and descriptions) in Tolstoy experiences, you'll need to set up a daily export of your product catalog, host it at a public URL, and connect it in the Tolstoy settings.

**Step 1: Prepare Your CSV File**

 

Before linking your CSV file, ensure it follows the correct column naming conventions. Your CSV file must contain specific mandatory columns as shown below.

 

**Mandatory Fields:**

- id: A unique identifier for the product (e.g., SKU or product ID).

- title: The name of the product.

- url: The URL link to the product page.

- imageUrl: The primary image URL of the product.

- price: The current price of the product.

![image](https://github.com/user-attachments/assets/7e0abd20-cc53-47a7-8ac2-039e498f5a4e)

**Optional Fields:**

- descriptionHtml: A description of the product, which may include HTML formatting.

- images: Additional image URLs for the product (comma-separated).

- compareAtPrice: The original price before any discounts (for comparison).

- currencyCode: The code of the currency (e.g., USD, EUR).

- currencySymbol: The symbol of the currency (e.g., $, €).

- inventory: The number of units available.

Ensure your CSV file matches these column names exactly, as Tolstoy will not accept files with incorrect headers.

**Step 2: Set Up a Daily Export**


**​1. Export Your Product Catalog:**

- Set up a system to export your product catalog data daily into a CSV file. Many eCommerce platforms (such as Shopify, WooCommerce, etc.) allow automated product data exports.

**2. Host the CSV File:**

- Place the exported CSV file in a shared location with a public URL. The CSV file must be accessible via a public link so Tolstoy can access it regularly. For example, you can host it in a public cloud storage service like Google Drive, Dropbox, or AWS S3 with public read permissions. 

**Step 3: Add CSV URL to Tolstoy Settings**

 

**1. Navigate to Tolstoy Settings:**

- Log into your Tolstoy account and go to the Installation section.

  ![image](https://github.com/user-attachments/assets/d5876beb-2cc3-49dd-aa77-68812644813b)

- You can get there by clicking your profile letter on the lower left, then selecting Settings.

  ![image](https://github.com/user-attachments/assets/ad95a6f5-d18d-4958-b7e4-dc08bd5ef12c)

**2. Upload Your CSV:**

- In the "Upload from CSV" section, click Import CSV file.

- Paste the public URL of your CSV file into the provided input field.

  ![image](https://github.com/user-attachments/assets/8e24d7db-d97f-45f7-ab34-073add2a2044)

**3. Connect the CSV:**

- Once the URL is added, Tolstoy will automatically import the product data from the CSV file.

- Ensure that your CSV file is updated daily to reflect accurate and up-to-date product information in Tolstoy experiences.

**Frequently Asked Questions:**
​

**What happens if my CSV file has an error?**

- Ensure the CSV file follows the correct column names and formats. Any discrepancies in the required fields may result in errors during upload.

**How often should I update the CSV file?**

- We recommend updating the file daily to ensure your product information in Tolstoy is always current and reflects changes in inventory or pricing.

**Can I manually upload the CSV file instead of using a URL?**

- Currently, Tolstoy requires a public URL to access your CSV file. This helps automate the process by pulling in updated product data daily without manual uploads.

**What file formats are supported?**

- Only .csv file formats are supported at this time. Ensure that the file uses commas as delimiters between values.


