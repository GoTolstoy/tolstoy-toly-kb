## Content Integration Sources

### Goal

The goal of this class of integrations is for users to easily access existing sources of fresh content. These integrations allow users to connect sources where their content already exists and automatically access and import that content on an ongoing basis.

### List of Content Integrations

#### Cloud

- **Dropbox**

  The integration leverages a Dropbox component to import the specific video files the user selects. Every time the user wants to import new files, they have to re-enter the Tolstoy app and choose the additional files. There is no need to connect Dropbox’s account to Tolstoy; the authentication happens in the Dropbox component.

- **Google Drive**

  The integration allows users to connect their Google Drive and select specific folders to auto-display video files from the selected folders in the Tolstoy app. Even though the files are automatically displayed under the Google Drive source in the Library, the files are not auto-imported. A file is only imported after tagging it with a product or a playlist. There can only be one Google Drive account connected per Tolstoy account.

#### Social

- **Instagram**

  The integration allows users to connect their Business Instagram account and auto-import video, image, and image carousel files from it. You can connect multiple Instagram accounts to one Tolstoy account. The videos will be added and refreshed under the Instagram source automatically once connected.

  In addition, users can find UGC Search content by hashtags and their Instagram mention, ask for content rights, and use the content after approval. Requesting rights is manual via a direct message on Instagram. Once the content is approved by the publisher, it is automatically moved to the approved folder and is ready to use.

  There is also an option to auto-tag assets from Instagram with products based on exact matching of the name of the tagged product on Instagram to the name of a product in the Shopify catalog.

- **TikTok**

  The integration allows users to connect their TikTok account and auto-import videos from it. You can connect multiple TikTok accounts to one Tolstoy account. The videos will be added and refreshed under the TikTok source automatically once connected.

  In addition, users can manually import videos via a URL to the video on TikTok. Users have to check the checkbox that they have rights to the video.

- **YouTube**

  The integration allows users to connect their YouTube account and select specific folders to auto-display video files from the selected folders in the Tolstoy app. Even though the files are automatically displayed under the YouTube source in the Library, the files are not auto-imported. A file is only imported after tagging it with a product or a playlist. There can only be one YouTube account connected per Tolstoy account.

#### AI

- **D-ID**
- **Synthesia**

#### Creators

- **Billo**

### UX / UI

These integrations can be found in two areas inside the app:

#### Library Page

- The content source integrations (such as Instagram, TikTok, YouTube, and Google Drive) are available from the **Library page** in the app.
- The library page presents a content management area where users can connect various content sources for their assets (videos and images) in addition to organizing and tagging their assets.
- This page has a second navigation panel grouping the assets by type, source, or playlist. The content source integrations are available under the ‘Sources’ menu item.
- **Sources Menu Item:**
  This is a collapsible menu item within the second panel of the user interface. It appears to be an organizing header for various content source integrations available to the user. The arrow next to ""Sources"" suggests it can be expanded to show or hide the list of content sources.
- **Content Source Integration Section:**
  This is a designated area within the library interface for integrating external content platforms. Each platform has a distinct section similar to the one displayed for YouTube.
- **Empty State Placeholder:**
  - The placeholder showcases the logo of the respective platform, clearly indicating which service it pertains to.
  - A ""Connect"" button is prominently displayed, suggesting a single-step action to link the platform to the app.
  - When a source is not yet connected, this uniform empty state serves a dual purpose. It visually indicates that the integration is available but not yet activated, and it acts as a call to action, prompting the user to establish the connection. Once connected, this section would transition to display content from the integrated platform's media library, maintaining a consistent user experience across all sources.
  - **Screenshot** of the library page when YouTube is not connected and selected: [YouTube Integration Screenshot](https://app.gotolstoy.com/videos/youtube)

#### Integrations Page