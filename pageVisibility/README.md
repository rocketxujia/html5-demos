pageVisibility
==============
The Page Visibility API lets you know when a webpage is visible or in focus. 也就是说我们能通过Page Visibility API监听到页面被最小化操作，或tab切换掉了。
## 浏览器端的页面预加载功能
页面有三种状态： visible、hidden、prerender。所谓的prerender状态就是页面在预加载状态。
<link rel="prerender" href="http://example.org/index.html">

## demo 1: visibility.html
展示了通过页面是否visible的监听来控制视频的播放或停止

## 参考文档
1. [(mdn)visibility](https://developer.mozilla.org/en-US/docs/DOM/Using_the_Page_Visibility_API)
2. [(google developer)Using the Page Visibility API](https://developers.google.com/chrome/whitepapers/prerender)
3. [(github)visibility组件]：(https://github.com/ai/visibility.js)




