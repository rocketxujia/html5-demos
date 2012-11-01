drag&drop 事件
==============
过去我们想实现网页中的拖拽效果，基本上都是使用DOM事件模型中的mousedown、mousemove、mouseup的事件监听来模拟拖拽效果，为了实现实时的拖拽移动效果，还要不停地获取鼠标的坐标，还要不停的修改元素的位置，代码要堆很多，而且性能上也很不好(不停地修改元素位置会导致页面reflow，除非绝对定位)。<br />
现在有了html5原生的Drag & Drop 拖拽事件，不仅性能而且使用上也方便了许多。
１.　包含的相关事件可查看页面： https://developer.mozilla.org/en-US/docs/DragDrop/Drag_and_Drop
２.　值得一提的是HTML5支持拖拽数据存储，使用dataTransfer接口，作用于元素的拖拽过程中，可通过事件句柄中的event对象上取得， 包含属性可查看页面：  https://developer.mozilla.org/en-US/docs/DragDrop/DataTransfer
## demo一（test1.html）:
简单拖放图片

## demo二（../filereader/filereader2.html）: （demo需要在服务器下部署查看）
展示： 包含展示了从本地文件中拖放到页面指定框内，从而得到文件信息，以及做其他操作。




