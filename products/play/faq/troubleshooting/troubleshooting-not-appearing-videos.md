# Troubleshooting Not Appearing Videos

## Key Factors to Check

1. **Project Type & Target Page**
   - **Project Type:**
     - **Homepage Project:** Displays all videos.
     - **PDP Project:** Shows videos specific to each product.
   - **Target Page:**
     - **Homepage:** All videos should display.
     - **PDP:** Displays videos for the relevant product only.

2. **Allow Non-Tagged Videos Setting**
   - **PDP Projects:**
     - If off (default), only product-specific videos appear.
     - If on, all videos appear.
   - **Homepage Projects:** This setting doesn’t matter since all videos will display.

## Common Scenarios

1. **Standard Implementation**
   - **PDP Projects on PDPs:**
     - Product-specific videos are shown.
     - Pinning is correctly reflected.
   - **Homepage Projects on Homepages:**
     - All videos are shown without filtering.
     - Pinning works as expected.

2. **Abusive Implementation**
   - **Homepage Project on PDP:**
     - Shows all videos or only product-specific ones, but pinning might not work.
   - **PDP Project on Homepage:**
     - All videos appear, but pinning may not reflect correctly.

## Common Causes for Missing Videos

1. **Mismatched Project Type:** Ensure the correct project type is used for the page.
2. **Allow Non-Tagged Videos:** Check if the setting is off for PDPs.
3. **Abusive Implementation:** Avoid placing Homepage projects on PDPs and vice versa to prevent pinning and display issues.\
