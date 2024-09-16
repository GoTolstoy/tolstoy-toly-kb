## Technical Issues

### Problem Description
The client reported an issue with the 'add to cart' functionality where items added from Tolstoy were not immediately visible in the cart. Additionally, these items appeared as duplicates when added again.

### Resolution
The issue was resolved by creating a function to refresh the cart page whenever an item is added from Tolstoy PDP. This ensured that the cart displayed the newly added items correctly and prevented duplicate entries.