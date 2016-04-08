HTML5中的download属性
---

`download` 是 HTML5 中 `<a>` 标签的新增属性。

当用户点击超链接时，`download` 属性指定 `href` 目标进行下载，而不是跳转。

语法：
```
<a href="xx.png" download="filename">
```

> `filename` 参数可选，它指定下载文件的文件名。

检测浏览器是否支持 `download` 属性：
```
var isSupportDownload = 'download' in document.createElement('a');
```

示例：
```
<a href="images/fe/fe1.jpg" download>download</a>
```

除了图片资源，我们还可以是PDF资源，或者txt资源等等。尤其Chrome等浏览器可以直接打开PDF文件，使得此文件格式需要download处理的场景越来越普遍。