## Slow Video Loading on Shop App

Your first and second video sizes may be a bit large. By default, we preload the current and next videos. The video starts playing when around 20%-25% is downloaded. Sometimes less, sometimes more. Unfortunately, we don't have control over these numbers in the Shop app.

Here's a tip from our dev team: either reduce the video sizes or reorder the videos from smallest to largest, putting the smaller files at the beginning.

To further improve our UX, we have already submitted a new player version where we use Shop app entry points to display the initial videos and download the rest in the background. Our tests show that it will only take 2-3 seconds for the first video to start playing. However, the go-live date of this new player version is tied to the Shop app updates. Hopefully, this will be rolled out soon!
