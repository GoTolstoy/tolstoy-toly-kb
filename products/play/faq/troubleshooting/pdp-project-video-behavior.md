# PDP Project Video Behavior

## Variables Influencing Video Display

1. **Project Type**: A PDP project will display videos based on product-specific filtering.
2. **Target Page**: When placed on a product page, only videos related to the specific product should appear.
3. **Allow Non-tagged Videos on PDPs Setting**:
   - Toggled Off (Default): Only product-specific videos will show.
   - Toggled On: All videos, whether tagged to products or not, will be shown on PDP pages.

## Expected Behavior

When a PDP Project is placed on a PDP:
- **Allow Non-tagged Videos Off (Default)**: Only videos tagged to the product are displayed.
- **Allow Non-tagged Videos On**: All videos will be displayed, even those not tagged to specific products.
- Pinning functionality from the app is properly reflected on the PDP.

## Common Bugs

- **Videos not showing correctly**: Check the "Allow non-tagged videos" setting. If non-product videos are showing, this toggle may be on when it should be off.
- **Pinning not working as expected**: Ensure pinning is correctly set in the app and that the PDP project is not mistakenly implemented on a Homepage.