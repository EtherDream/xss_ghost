XSS Ghost

将 XSS 注入到父窗口和子窗口，延长攻击时间。

用法：

```
<script src="xss_ghost.js"></script>
<script>
    XssGhost.init({
      id: 'test-1',   // 相同 id 的 padyload 不会重复运行
      payload: function() {
      	console.log('xss run');
      }
	});
</script>
```

讲解：[http://www.cnblogs.com/index-html/p/xss_long_live.html](http://www.cnblogs.com/index-html/p/xss_long_live.html)

Demo：[http://www.etherdream.com/FunnyScript/XSSGhost/](http://www.etherdream.com/FunnyScript/XSSGhost/)

未实现：

* 子页面劫持

* document.domain 降域尝试

* 低版本 ie 不支持
