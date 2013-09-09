JavaScript 语法检查可使用 [JSHint](http://www.jshint.com/), `Sublime Text` 的用户可以通过安装 [SublimeLinter](https://github.com/SublimeLinter/SublimeLinter) 这个插件自动监测。

------------------------------------

## 总是用var声明变量

不使用var会导致变量作用域混乱

## 变量命名
* 声明变量、函数等使用 [小驼峰式命名法(lower camel case)](http://en.wikipedia.org/wiki/CamelCase)
* 声明类使用 [大驼峰式命名法(upper camel case)](http://en.wikipedia.org/wiki/CamelCase)

```JavaScript
var Book = Backbone.Model.extend({

    defaults: {
        title: '',
        author: ''
    },

    initialize: function(){

    }
});

var mathBook = new Book({
    title: 'Advanced Mathematics'
});
```

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

## 访问 object 的属性使用`.`

```JavaScript
person['name'] = 'sdf';  // bad

person.name = 'aer';     // good
```

## function declarations should not be placed in blocks

```JavaScript
// Wrong
if(x){
    function foo(){}
}
```

## 避免使用位运算符
按位与`&`、按位或`|`、按位异或`^`、按位非`~`、左移`<<`、带符号的右移`>>`和用0补足的右移`>>>`。
这套运算符针对的是整数，所以对Javascript完全无用，因为Javascript内部，所有数字都保存为双精度浮点数。
如果使用它们的话，Javascript不得不将运算数先转为整数，然后再进行运算，这样就降低了速度。
而且“按位与运算符”`&`同“逻辑与运算符”`&&`，很容易混淆。

```Javascript
    // 有些喜欢这样取整
    var a = b|0 ;  // bad
    var a = Math.floor(b); // good
```

