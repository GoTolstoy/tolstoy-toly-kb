# Products Wishlist

## Feature Overview

The **Products Wishlist** feature allows customers to add their favorite products to a wishlist as they swipe through video feeds on-site. The wishlist is found in a second tab within the video feed. The customer’s products will be saved for them across sessions after they sign in. The main goal of the feature is to enable customers to aggregate their favorite products as they browse video feeds so they can return and convert.

![Lana](https://downloads.intercomcdn.com/i/o/1021645760/71f40d9673ad5859e3b33fa1/Lana.png)
![Wishlist](https://downloads.intercomcdn.com/i/o/1021646264/71fdf2848fb4c5d13cb72f6a/Wishlish.png)

## Configuration Options

The wishlist is enabled by default for all video feeds, but users can disable the wishlist feature in their player settings under “Design” → “Video Feed” → “Behavior” and select the "Hide wishlist" option.

![Hide wishlist](https://downloads.intercomcdn.com/i/o/1021647739/040830e0cc08ecac18f8dc8f/Hide+wishlist.png)

Shopify Plus stores can provide their **Multipass Secret**, which will allow customers with any email provider to save their wishlist under any email address after providing a verification code. The Multipass Secret should be inputted in **Settings** → **My Workspace** → **Account information**.

Stores not on Shopify Plus (or Shopify Plus stores that have not provided their Multipass Secret in Tolstoy) will allow customers to save their wishlist through Google accounts.

## User Experience

When adding a product to the wishlist for the first time:

- When watching a video feed, customers can select the heart button on a product to add it to their wishlist. The wishlist tab will then open, and the user will be prompted to log in to add the product to their wishlist.

  ![Multipass login](https://downloads.intercomcdn.com/i/o/1021648622/37933f6faf21120a3c697950/multipass+login.png)
  
  - Customers on a Shopify Plus store will be prompted to provide their email. They will then receive a confirmation email with a code. They will return to the wishlist window and provide the code to access their wishlist.
  - Customers not on a Shopify Plus store will be prompted to log in via Google Auth0.

  ![Google Auth0 login](https://downloads.intercomcdn.com/i/o/1021649021/3a92d7db7d99cb40aafa1f48/Google+Auth0+login.png)

After authentication, the player is reopened, and the product will be added to the wishlist.

As users continue to scroll through video feeds across a store, they can add products to their wishlist. They can navigate to their wishlist by selecting the wishlist tab. Customers can also remove products from their wishlist.

## Data Management

Each shop maintains its separate customer profiles. Wishlist and customer data are not shared across different shops.

When a customer likes a product, their profile is saved in the shop's database along with their liked products. In the future, stores will be able to see which products have been added to a customer’s wishlist through the Audience tab.