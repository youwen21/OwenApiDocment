<br/>  
# Owen接口文档系统

Owen接口文档系统，是一个把markdown文件转换成HTML并且高量代码模块的系统。  

Owen接口文档系统与其他的文档系统相比较优缺点：  
优点  
    - 无需搭建后台，不依赖数据库，下载既可用
    - 基于Markdown文件，输写方便

缺点  
    - 文档有大的参数调整时需要编辑每一个markdown文件

```
有数据库的API文档系统可以update数据批量更新文档接口，
而基于markdown文档的系统则需要使用sed,grep，awk等工具批量更新文档接口

```

Owen接口文档系统组成有
- [marked：Markdown转HTML](https://github.com/markedjs/marked)
- [markdown-css-themes：Markdown主题](https://github.com/jasonm23/markdown-css-themes)
- [highlight.js：高量代码块](https://github.com/isagalaev/highlight.js)
- [monokai_sublime：Sublime风格主题，找不到出处了](#)

### 项目结构
    - js
    - css
    - doc
        + 文档模块1
        + 文档模块2
    - index.html 首页
    - index.md 首页markdown文档

在index.md写入markdown 首页入口
doc目录是各个接口的markdown文档，index.md超链接到接口详情页


###  
## 效果预览
[http://owenapi.exwechat.com/](http://owenapi.exwechat.com/)

### 当前实现不好的地方：
给 pre>code 添加hljs类是用的字符串替换，有更好的实现方式的话可以提交