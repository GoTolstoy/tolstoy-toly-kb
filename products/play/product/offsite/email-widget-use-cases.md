## Email widget use cases

### Create

There are two types of carousel widgets, one that's suitable for email flows triggered by a product related event and the other is suitable for email campaigns showing the same content in all emails sent.
![screenshot](https://downloads.intercomcdn.com/i/o/1031051204/dcbc59231ee2b1cd5062457d/image.png)

### Email campaigns - Trending videos

The 'Trending videos' use case is great to add to a newsletter, product launch and even to a welcome flow. Even though it's designed for campaigns, it can be used in a flow, only it would show the same videos no matter what the trigger is.

### Selecting the videos source and GIF action

By default, a new 'Trending videos' project's videos are shown from a new set of playlists selected. In this case, since the feed is not yet added to your site, the GIF will redirect to a new TV page automatically added to your store. 

If you want to source the videos from an existing onsite project use the following steps:

1. Go to the projects settings, from the ⚙️ icon on the top right of the screen.

2. Under 'Video source', select from your active onsite projects. Notice that product page projects won't appear in this list for the 'Trending videos' use case.

3. Under 'GIF action', either type a URL of the page where the selected source is live on, or select a '+ New TV page'. Notice that if selecting a page where the source project is not live on the GIF will redirect to a new TV page. 
![screenshot](https://downloads.intercomcdn.com/i/o/1031102738/9f9ddb62ae68d06f07e2434c/image.png)

Notice that if you change the video source to any of your existing projects some of the video, design and settings won't be available since they're pulled from the selected source project.

### Email flows - Abandonment and Post-purchase

The 'Abandonment revival' and 'Post-purchase guides' use cases are the same type of widget, creating multiple feeds based on the product from event trigger from the email provider. Make sure the email you're adding the widget to is part of a flow triggered by a product related event. 

### Selecting the videos source and GIF action

By default, the videos are set to show from the latest active onsite product page project. The videos will be grouped by product to represent the different GIF variations that would be generated. Notice that some settings won't be available since they're pulled from the selected source project. In this case, the GIF will redirect to the video on the product page.

If you want to change the source of the videos use the following steps:

1. Go to the projects settings, from the ⚙️ icon on the top right of the screen.

2. Under 'Video source', select from your active onsite product page projects or create a new feed. Notice that only product page projects appear in this list for Abandonment and Post-purchase use cases.
![screenshot](https://downloads.intercomcdn.com/i/o/1031136618/091f6af096b1405666ac8203/image.png)

3. Under 'GIF action', either select Product page, this will dynamically redirect to the product page based on the product in the event that triggered the flow. Or select a '+ New TV page'.
![screenshot](https://downloads.intercomcdn.com/i/o/1031138255/5e9072ecbef18840de2ad4b7/image.png)

### Publish

Select the email provider so we can properly track the email attribute and provide user journeys, if your email provider is not in the list please contact support. Publishing the email widget is done using HTML, the code can be added via an HTML editor or via source code in a text block in a drag and drop editor. 
![screenshot](https://downloads.intercomcdn.com/i/o/1031159408/5d73d706842f16d978fe35df/image.png)

Simply add the code to an email template, the GIF automatically updates with new videos from the feed set up in the project editor on the Tolstoy app. Notice that the GIF won't show if there are less than three videos eligible.
![screenshot](https://downloads.intercomcdn.com/i/o/1031171244/6e797ce8defed340459a687b/image.png)

### Klaviyo flows

To preview the GIF for the email flows use cases, edit the template from the flow, it will show broken images instead of the videos in the GIF, it's OK. To preview properly, click 'Preview & test' and swipe through events. The GIF will show different videos per event based on the products connected to it. If you can't see the GIF it means there were no three videos found for the GIF. 
![screenshot](https://downloads.intercomcdn.com/i/o/1031220777/626f2f7194b911390a61c857/image.png)
