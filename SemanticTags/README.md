html5 标签相关
==============
##新增tag：  <section>,  <article>,  <aside>, <footer>,  <header>, and <nav> ...
## HTML的大纲算法(HTML5 outlining algorithm):  producing outline summaries of Web pages。
大纲算法允许用户代理(user agent)从一个web页面生成一个信息结构目录，让用户对页面有一个快速的概览。类似书籍、PDF、帮助文档等，都有一个清晰的目录结构，用户能方便的定位所需内容。一个良好结构的大纲，不仅是对于搜索引擎的优化，更是为借助于屏幕阅读器浏览网页的盲人（或弱视力）用户提供了巨大的帮助。
1. 显性定义section含义的标签都有 <body>, <section>,  <article>,  <aside>, and <nav>，且每个section最好都有一个heading标签（h1-h6）。
2. 隐性定义section含义的标签：heading标签（h1-h6）。
 2.1 每个标题都会生成一个隐性节点(implicit section)，紧随其后的相对层级低的标题会成为它的子节点，层级相同或者更高的标题则会关闭这个节点并生成新的节点。

## 参考文档
1. [(smashingmagazine)大纲算法详解](http://coding.smashingmagazine.com/2011/08/16/html5-and-the-document-outlining-algorithm/)
1. [(MDN)Sections and Outlines of an HTML5 Document](https://developer.mozilla.org/en-US/docs/Sections_and_Outlines_of_an_HTML5_document)
2. [(cued翻译)HTML大纲算法对结构的影响](http://cued.xunlei.com/log047)




