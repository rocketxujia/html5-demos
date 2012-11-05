audio and video
==============
## audio or video 属性
* controls : Displays the standard HTML5 controls for the audio on the web page.
* autoplay : Makes the audio play automatically.
* loop : Make the audio repeat (loop) automatically.
* preload: "none" does not buffer the file; "auto" buffers the media file; "metadata" buffers only the metadata for the file
## 支持media format:
https://developer.mozilla.org/en-US/docs/Media_formats_supported_by_the_audio_and_video_elements
## HTMLMediaElement对象的api：
* Properties: seekable、played、currentTime ...
## Fallback options: 渐进增强原理
the opening and closing tags of media elements is processed by browsers that don't support HTML5 media. You can take advantage of this fact to provide alternative fallback media for those browsers.
* 使用简单文案提示。
* 或内嵌falsh解决方案。
## Error handling
可通过source元素节点捕获异常

## 参考文档
1. [(MDN)HTMLMediaElement]：(https://developer.mozilla.org/en-US/docs/DOM/HTMLMediaElement)
2. [(w3.org)mediaevents](http://www.w3.org/TR/html5/media-elements.html#mediaevents)
3. [ovideoconverter](http://www.mirovideoconverter.com/)




