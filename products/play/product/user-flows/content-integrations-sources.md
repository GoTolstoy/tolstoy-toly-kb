## Content Integrations Sources

- Goal
    - The goal of this class of integrations is for users to be able to easily access existing sources of fresh content. These integrations allow users to connect sources where their content already exists, and to automatically access and import that content on an ongoing basis.
- List of content integrations
    - cloud
        - dropbox
            
            The integration leverages a dropbox component to import the specific videos files the user selects. Every time the user wants to import new files they have to re-inter the Tolstoy app in and choose the additional files. There is no need to connect dropbox’s account Tolstoy, the auth happens in the dropbox component.
            
        - google drive
            
            The integration allows users to connect their google drive and select specific folders to auto display video files from the selected folders in the tolstoy app. Even though the files are automatically displayed under the Google Drive source in the Library, the files are not auto imported, a file is only imported after tagging it with a product or a playlist. There can only be one Google drive account connected per Tolstoy account.
            
    - social
        - instagram
            
            The integration allows users to connect their Business instagram account and auto import video, image and image carousel files from it. You can connect multiple Instagram accounts on one Tolstoy account. The videos will be added and refreshed under the instagram source automatically once connected.
            
            In addition, users can find UGC Search content by hashtags and their Instagram mention, ask for content rights and use the content after approved. Requesting rights is manual via a direct message in Instagram. Once the content is approved by the publisher it is automatically moved to approved folder and is ready to use.
            
            There is also an option auto tag assets from instagram with products based on exact matching the name of the tagged product in instagram to the name of a product in shopify catalog.
            
        - tiktok
            
            The integration allows users to connect their Tiktok account and auto import video from it. You can connect multiple TikTok accounts on one Tolstoy account. The videos will be added and refreshed under the TikTok source automatically one connected.
            
            In addition, users can manually import videos via a URL to the video in TikTok. Users have to check the checkbox that they have rights to the video.
            
        - youtube
            
            The integration allows users to connect their youtube and select specific folders to auto display video files from the selected folders in the tolstoy app. Even though the files are automatically displayed under the YouTube source in the Library, the files are not auto imported, a file is only imported after tagging it with a product or a playlist. There can only be one YouTube account connected per Tolstoy account.
            
    - ai
        - D-ID
        - synthesia
    - creators
        - billo
- UX / UI
    - these integrations can be found in 2 areas inside the app
        - library page
            - The content source integrations (such as Instagram, Tiktok, YouTube, and Google drive) are available from the **Library page** in the app.
            - The library page presents a content management area where users can connect various content sources for their assets (videos and images) in addition to organize and tag their assets.
            - This page has 2nd navigation panel grouping the assets by type, source or playlist. The content source integrations are available under the ‘Sources’ menu item.
            - **Sources Menu Item:**
            This is a collapsible menu item within the second panel of the user interface. It appears to be an organizing header for various content source integrations available to the user. The arrow next to "Sources" suggests it can be expanded to show or hide the list of content sources.
            - **Content Source Integration Section:**
            This is a designated area within the library interface for integrating external content platforms. Each platform has a distinct section similar to the one displayed for YouTube.
            - **Empty State Placeholder:**
                - The placeholder showcases the logo of the respective platform, clearly indicating which service it pertains to.
                - A "Connect" button is prominently displayed, suggesting a single-step action to link the platform to the app.
            - When a source is not yet connected, this uniform empty state serves a dual purpose. It visually indicates that the integration is available but not yet activated, and it acts as a call to action, prompting the user to establish the connection. Once connected, this section would transition to display content from the integrated platform's media library, maintaining a consistent user experience across all sources.
            - **Screenshot** of the [library page when youtube is not connected and selected](https://app.gotolstoy.com/videos/youtube)
                
                ![image](https://github.com/user-attachments/assets/75bbf033-471f-4107-9c51-7e589f9f2b9f)

                
        - integrations page
