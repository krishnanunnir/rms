# RMS 

I was building an app few days ago with the Reddit api with PRAW, I just realised how messed up the media management is, to list few of the inconveniences I faced
1. The audio and video is separated and avialable from different endpoints. The audio for newer uploads seem to be from another endpoint than the older one.
2. A gif/video hosted in gfycat etc, even though shown in Reddit directly, is treated as a embeds. 
3. Error messages are not very descriptive. Trying to access the audio endpoint for a video with audio seems to show forbidden. After having no clue what is happening and browsing on this subreddit froms ome time, I found for some videos the endpoint is different for some other videos.

I thought a framework would be nice for this.

The issues I want to solve with the framework are
1. Video management should be abstracted away, the user shouldn't have to worry about merging video and audio together.
2. Support for third party apps. Content from services like gfycat, imgur, streamable should be handled directly in the tool the user can directly use the image, gif or video.(A bit too ambitious maybe?)

Please add an issue if you think another feature needs to be added.