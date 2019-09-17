一，Node中的js和浏览器中的js区别
1，区别：

浏览器中的js：

（1）添加了DOM，用于处理document object model；
（2）添加了BOM，用于处理brower object model；
（3）主要用于前端HTMl元素的操作；
（4）JavaScript = ECMAScript+DOM+BOM；

Node中的js:

（1）在服务端来实现操作<script>，没有DOM
（2）主要用于后台服务的操作。
（3）ECMAScript+后台操作的API（OS:操作系统，file文件系统，net网络系统，database数据库）

2，相同点
（1）语言基础都是ECMAScript；

3，性能

浏览器中的js：

（1）根据浏览器内核解析js；

Node中的js：

（1）nodejs是基于Chrome's JavaScript runtime，也就是说，实际上它是对GoogleV8引擎（应用于Google Chrome浏览器)进行了封装
