# Tapcart Conversion Troubleshooting

Troubleshoot list for missing conversion data on Tapcart:

- Is the Cart API correctly enabled for the customer account? (Check with their Tapcart AM)
- Is the customer's Tapcart app updated to the latest version? (Check with their Tapcart AM)
- Is the custom block SDK on version 1.7 or higher?
- Is the block code set up with the correct appKey and projectId?
- Do they have the new code implementation? (The initial code we created for custom blocks didn't support conversion, so they will have to update the block code if that's the case.)
