# 更好的方式实现

### 实现思路：

`nginx`配置请求所有url返回同一个页面，如xx.com/aaa.html, xx.com/bbb.html返回同一个页面 。

- javaScript获取URI转换成对应的md文档AJAX请求然后渲染


# 另一种思路

### 后台语言根据URL找到应该的MD，嵌入到页面中直接返回完整的HTML