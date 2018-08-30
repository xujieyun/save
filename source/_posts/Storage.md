---
title: Storage 进行页面缓存
date: 2018-08-28 01:04:06
tags:
---
<iframe frameborder="no" border="0" marginwidth="0" marginheight="0" width=330 height=86 
	src="http://music.163.com/outchain/player?type=2&id=25706282&auto=0&height=66">
</iframe>
sessionStorage 属性允许你访问一个 session Storage 对象。它与 localStorage 相似，不同之处在于 localStorage 里面存储的数据没有过期时间设置，而存储在 sessionStorage 里面的数据在页面会话结束时会被清除。页面会话在浏览器打开期间一直保持，并且重新加载或恢复页面仍会保持原来的页面会话。在新标签或窗口打开一个页面会初始化一个新的会话，这点和 session cookies 的运行方式不同。
应该注意的是，无论是 localStorage 还是 sessionStorage 中保存的数据都仅限于该页面的协议。
``` bash
// 保存数据到sessionStorage
sessionStorage.setItem('key', 'value');

// 从sessionStorage获取数据
var data = sessionStorage.getItem('key');

// 从sessionStorage删除保存的数据
sessionStorage.removeItem('key');

// 从sessionStorage删除所有保存的数据
sessionStorage.clear();
```
{% asset_img 程序员择偶标准.JPG 程序员择偶标准 %}