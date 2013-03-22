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


