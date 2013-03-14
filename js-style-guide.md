JavaScript 语法检查可使用 [JSHint](http://www.jshint.com/), `Sublime Text` 的用户可以通过安装 [SublimeLinter](https://github.com/SublimeLinter/SublimeLinter) 这个插件自动监测。

------------------------------------

## 不要注释无用代码

一是增加了搜索时无用的结果，二是给维护增加了很多困难  
保存旧代码是版本管理工具的工作

## 总是用var声明变量

不使用var会导致变量作用域混乱


## 总是使用分号

浏览器自动补完的分号有时会出问题，产生莫名奇妙的bug，尤其是合并压缩的时候。

```JavaScript
(function(){
    // some code
})()

(function(){
    // some more code
})();
```

## function declarations should not be placed in blocks

```JavaScript
// Wrong
if(x){
    function foo(){}
}
```


