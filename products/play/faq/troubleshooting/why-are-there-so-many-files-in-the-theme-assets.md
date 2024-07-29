## Why are there so many files in the theme assets? Can the video files in the theme assets be deleted?

We used to store the video files there, so that they would load faster via Shopify CDN and also at the top of the waterfall on page load so that it wouldn't hurt core web vitals.

However, we've since realized this wasn't the best location for the files, and we've updated our process. Today we store videos in 'files' so these are actually old assets that can be deleted. We just prefer not to delete anything from this area on customers' behalf.
