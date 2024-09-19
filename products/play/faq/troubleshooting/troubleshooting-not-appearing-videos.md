# Troubleshooting Not Appearing Videos

## Steps to Troubleshoot

1. **Check the Project Type**
   - Ensure the correct project type is being used for your page:
     - **Homepage Project**: All videos should appear, regardless of tags.
     - **PDP Project**: Only product-specific videos will appear unless otherwise configured.

2. **Confirm the Target Page**
   - Verify that the project type matches the target page:
     - **Homepage Project on a Homepage**: All videos should appear.
     - **PDP Project on a PDP**: Only the videos associated with that specific product will appear.

3. **Review the ""Allow Non-tagged Videos on PDPs"" Setting**
   - For PDP Projects:
     - **Toggled Off (Default)**: Only product-specific videos will show.
     - **Toggled On**: All videos, tagged or not, will show on product pages.
   - For Homepage Projects, this setting is irrelevant as all videos should display regardless.

4. **Pinning Misconfiguration**
   - Check if pinning is set up correctly in the app. Pinning affects the display order, and incorrect pinning could cause videos to not appear.

5. **Check for Implementation Errors**
   - Ensure that the project widget is placed correctly on the intended target page.
   - For PDP projects, confirm that the correct product page is linked.

## Common Causes

- **Incorrect Project Type**: A PDP project implemented on a Homepage or vice versa.
- **Misconfigured Allow Non-tagged Videos Setting**: Videos not tagged to products may not appear if this setting is toggled off.
- **Pinning Setup Issues**: Videos might not be appearing if pinning is misconfigured.

If videos still do not appear after following these steps, try refreshing the widget and clearing any cached data on the site. If the issue persists, contact support.
