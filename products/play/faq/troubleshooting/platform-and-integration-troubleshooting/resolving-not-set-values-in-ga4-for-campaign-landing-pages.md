## Resolving 'Not Set' Values in GA4 for Campaign Landing Pages

The 'not set' values in Google Analytics 4 (GA4) for campaign landing pages are likely caused by Tolstoy events being fired on pages with the Tolstoy snippet embedded, even if no videos are present on those pages. This can lead to inaccurate data reporting and confusion when analyzing campaign performance.

### Filtering Tolstoy Events in GA4

To address this issue, Tolstoy events can be filtered using Google Tag Manager (GTM) or any event management platform. By doing so, you can ensure that only relevant events, such as `TolstoyStarted` and `TolstoySessionStarted`, are recorded. This filtering helps maintain accurate and meaningful data in your GA4 reports.