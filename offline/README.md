html5离线技术（offline ）
==============
## offline storage
用户操作引起的或指定的。
包含以下四种技术： Web Storage (also called "Local Storage" or "DOM Storage"), Web SQL Database (or simply "SQL Storage"), IndexedDB, and File Storage.
都受same-origin principle applies :　the store is tied to the origin of the site that creates it (typically this amounts to the site domain or subdomain)

*Web Storage
DOM Storage is useful for storing smaller amounts of data

* Web SQL Database
WebSQL Database is a relational database access system,  关系数据库

* IndexedDB
 IndexedDB is an indexed table system. store larger amounts of structured data.
** IndexedDB重要特征：
1. IndexedDB databases store key-value pairs.   键值对存储
2. IndexedDB is built on a transactional database model. 事务的完整性
3. The IndexedDB API is mostly asynchronous. 异步操作的
4. IndexedDB uses requests all over the place. 经常使用request对象，有have onsuccess and onerror properties等各种回调函数
5. IndexedDB uses DOM events to notify you when results are available.
6. IndexedDB is object-oriented:   也是面向对象
IndexedDB is not a relational database, which has tables with collections of rows and columns.
This important and fundamental difference affects the way you design and build your applications.
在indexedDB 需要您去创建一个某种类型的store对象。然后用来存储大量js object。
7. IndexedDB does not use Structured Query Language (SQL). 不会使用sql操作。 它属于NoSql的一种
8. IndexedDB adheres to a same-origin policy. 受同源策略的限制。
** IndexedDB重要概念：
1. database： 由多个 object store 组成， 必须有以下属性：name  和 version.
2. object store:  Indexed 数据库的存储机制。 可以永久的包含多条记录，每个记录就是一个key-value对。每个object store内的记录以key升序排列。 必须有以下属性：name，ptionally 属性:  key generator and a key path.
3. database connection：当打开数据库时被创建。 同时可以创建多个连接。
4. transaction:
5. request: Every request represents one read or write operation.
6. index:
7. Key and value
7.1 Key :
类型： string, date, float, and array.
7.2 key generator
7.3 key path
7.4 value
8. Range and scope
8.1 scope
The set of object stores and indexes to which a transaction applies
8.2 cursor
A mechanism for iterating over multiple records with a key range.
8.3 key range
A continuous interval over some data type used for keys.


Each record has a value, including: boolean, number, string, date, object, array, regexp, undefined, and null.




https://developer.mozilla.org/en-US/docs/IndexedDB/Basic_Concepts_Behind_IndexedDB


## application caching：
一般有服务器配置。
HTML5 Cache Manifest：
1. html例子：
<html manifest="demo.appcache">

2. demo.appcache 文件例子：
    CACHE MANIFEST
    # 2012-02-21 v1.0.0
    /theme.css
    /logo.gif
    /main.js

    NETWORK:
    login.asp

    FALLBACK:
    /html/ /offline.html

修改*.appcache文件才能使application更新cache， 所以最好使用如上例的注释来代表需要更新啦~

## demo 1:  database.html
展示web SQL Database 的操作。

## demo 2:  bootup.html
展示通过bootup.js组件，把静态资源localstorage化（内部读取js文件内容）

## demo3: collect_indexDB.html
展示使用indexDB来实现收藏夹功能

## demo3: todoList_indexDB.html
展示使用indexDB来实现todoList功能

## 参考文档
1. [(mdn)IndexedDB系列](https://developer.mozilla.org/en-US/docs/IndexedDB/Using_IndexedDB)
2. [(html5rock)教程系列](http://www.html5rocks.com/en/tutorials/offline/)





