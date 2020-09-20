Audio ,vedio ,...
HTML5 comes with elements for embedding rich media in documents — <video> and <audio> — which in turn come with their own APIs for controlling playback, seeking, etc. This article shows you how to do common tasks such as creating custom playback controls.
  
  The HTML Video element (<video>) embeds a media player which supports video playback into the document. You can use <video> for audio content as well, but the <audio> element may provide a more appropriate user experience.


``<video controls width="250">``

    ``<source src="/media/cc0-videos/flower.webm" type="video/webm">``

    ``<source src="/media/cc0-videos/flower.mp4" type="video/mp4">``

  ``  Sorry, your browser doesn't support embedded videos.``
``</video>``


**Attributes**
Like all other HTML elements, this element supports the global attributes.

+ autoplay
A Boolean attribute; if specified, the video automatically begins to play back as soon as it can do so without stopping to finish loading the data.

+ controls
If this attribute is present, the browser will offer controls to allow the user to control video playback, including volume, seeking, and pause/resume playback.

+ loop
A Boolean attribute; if specified, the browser will automatically seek back to the start upon reaching the end of the video.
+ muted
A Boolean attribute that indicates the default setting of the audio contained in the video. If set, the audio will be initially silenced. Its default value is false, meaning that the audio will be played when the video is played.

+ preload
This enumerated attribute is intended to provide a hint to the browser about what the author thinks will lead to the best user experience with regards to what content is loaded before the video is played.

+ poster
A URL for an image to be shown while the video is downloading. If this attribute isn't specified, nothing is displayed until the first frame is available, then the first frame is shown as the poster frame.

+ src
The URL of the video to embed. This is optional; you may instead use the <source> element within the video block to specify the video to embed.
+ width

The width of the video's display area, in CSS pixels (absolute values only; no percentages).

[vedio  ](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/video)


The HTML <audio> element is used to embed sound content in documents. It may contain one or more audio sources, represented using the src attribute or the <source> element: the browser will choose the most suitable one.
  
  `` <audio  controls  src="/media/cc0-audio/t-rex-roar.mp3">``
           `` Your browser does not support the
            <code>audio</code> element.``
``</audio>``


**Attributes**

This element's attributes include the global attributes.

+ autoplay
A Boolean attribute: if specified, the audio will automatically begin playback as soon as it can do so, without waiting for the entire audio file to finish downloading.

+ controls
If this attribute is present, the browser will offer controls to allow the user to control audio playback, including volume, seeking, and pause/resume playback.

+ loop
A Boolean attribute: if specified, the audio player will automatically seek back to the start upon reaching the end of the audio.
+ muted
A Boolean attribute that indicates whether the audio will be initially silenced. Its default value is false.
+ preload
This enumerated attribute is intended to provide a hint to the browser about what the author thinks will lead to the best user experience.

+ src
The URL of the audio to embed. This is subject to HTTP access controls. This is optional; you may instead use the <source> element within the audio block to specify the audio to embed.
[audio](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/audio)
