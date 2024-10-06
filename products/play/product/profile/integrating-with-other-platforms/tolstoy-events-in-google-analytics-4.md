# Tolstoy Events in Google Analytics 4

## Main Event Names (Actions)

1. **tolstoyPageView** - Event of Tolstoy loaded on a page. For widgets, this also means view as it is always visible on the page.
2. **tolstoyEmbedView** - Event of Tolstoy element (carousel, stories) viewed on the page, fired when the user scrolls to the element on the screen.
3. **tolstoyStarted** - Click to play Tolstoy (click on the widget/carousel/stories).
4. **click** with label of **button text** - Click on an interactive button for branching video.
5. **tolstoyFeedScroll** - Scroll to the next video in the feed.
6. **tolstoyModalClose** - Close Tolstoy modal event, with label of seconds opened.
7. **tolstoyVideoLoaded-products** - Current video playing with label of tagged products.
8. **tolstoyVideoLoaded-videoName** - Current video playing with label of video name.

## Additional Events

- **tolstoyReachedEnd** - Reached end.
- **tolstoyLeadFormSubmit** - Submit of lead form.
- **Input with label of text** - Submit text response.
- **tolstoyVideoSubmit** - Submit video response.
- **tolstoyAudioSubmit** - Submit audio response.
- **tolstoyImageSubmit** - Submit image response.
- **tolstoyFeedPause** - Click on pause in the feed.
- **tolstoyFeedPlay** - Click on play in the feed.
- **tolstoyFeedNavigationArrowClick** - Click on arrow in the feed.
- **tolstoyFeedProductModalOpen** - Click on product info in feed.
- **tolstoyFeedProductModalClose** - Click on close product info in feed.
- **tolstoyOpenShareLink** - Click on a share platform.
- **tolstoyClickViewProduct** - Click on view product (URL product default).
- **tolstoyAddToCart** - Click on add to cart button.
- **tolstoyCartItemQuantityChange** - Click on quantity change button (- or +).
- **tolstoyClickCart** - Click the view cart button.
- **tolstoyClickViewProduct** - Click a specific product from multiple tagged products on video.
- **tolstoyDescriptionActionButtonClick** - Expand the product description accordion.
- **tolstoyFeedMenuModalClose** - Close modal after clicking […] menu.
- **tolstoyFeedNavigationArrowClick** - Click on arrow in the feed.
- **tolstoyFeedPause** - Click on pause in the feed.
- **tolstoyFeedPlay** - Click on play in the feed.
- **tolstoyFeedProductModalClose** - Click on close product info in feed.
- **tolstoyFeedProductModalOpen** - Click on product info in feed.
- **tolstoyVideoLoaded-products** - Current video playing with label of tagged products.
- **tolstoyVideoMuted** - Click mute button.
- **tolstoyVideoSeeked** - Move the timebar within the video.
- **tolstoyVideoUnmuted** - Click unmute button.
- **tolstoyVideoWatched** - When someone completed watching a video.