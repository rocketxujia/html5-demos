filereader
==============
根据 W3C 的定义，FileReader 接口 "提供一些读取文件的方法与一个包含读取结果的事件模型"。 目前一些主流的浏览器实现了 FileReader 接口（比如 Firefox 3.6+ 和 Chrome 6.0+）。
FileReader对象通过异步的方式读取本地机子上的文件（或data buffer）。
具体的api：可以查看
FileReader 对象 :　https://developer.mozilla.org/en-US/docs/DOM/FileReader
File 对象:  https://developer.mozilla.org/en-US/docs/DOM/File
## 案例一（filereader1.html）:
使用支持 FileReader 浏览器的用户将能够通过一个 file input 选择一个图像文件，并<b>不经过后台</b>将图像显示在页面中。

## 案例二（filereader2.html）: （demo需要在服务器下部署查看）
展示： 通过 FileReader 对象读取本地文件，然后使用FormData封装，最后使用xhr发送给后台。



