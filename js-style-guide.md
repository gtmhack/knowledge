## 总是用var声明变量

不使用var会导致变量作用域混乱


## 总是使用分号

浏览器自动补完的分号有时回出问题，产生莫名奇妙的bug，尤其是合并压缩的时候。

```JavaScript
(function(){
    // some code
})()

(function(){
    // some more code
})();
```
