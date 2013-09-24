* Mobile Tech  ( @ocean 同学分享的链接)
  <https://github.com/jtyjty99999/mobileTech>

* 操作绝对定位的dom,只会reflow对应节点及子节点

* audio不能播放离线缓存里的音频文件  
  解决方案: 基于base64 兜几个圈子  <http://www.appcelerator.com/>

* -webkit-animation-play-state 控制css动画的播放暂停

* 位移动画的target_el的top或left必须赋值(属于一个隐式bug)
  box-shadow等样式对性能影响较为严重

* do not add "minimum-scale=0.5", it will mess up the android  
  Android下这个viewport参数会触发系统的"双击缩放"功能, 影响游戏体验

* viewport屏幕适配相关问题备忘:     
<http://developer.android.com/reference/android/webkit/WebView.html>    
<http://menacingcloud.com/?c=highPixelDensityDisplays>

* CSS3 background-size 规则存在"优先级问题"(仅在新版本浏览器下存在 - -!)   
  
  解决方案: 
    1. background-size 定义在 background 之后
    2. background-size 属性添加 !important
    
  相关链接:   
  <http://blog.csdn.net/spring21st/article/details/7843341>
  
* iOS 下iFrame高度随内容变化而自适应(设置height无效)
  <http://www.cnblogs.com/weinan/archive/2013/01/05/2832800.html>

* App Splash Screen Sizes
  <https://github.com/phonegap/phonegap/wiki/App-Splash-Screen-Sizes>

* mobile safari上无法对 input 元素 focus 的问题
  <http://twilight.btlogs.com/how-to-focus-html-input-element-with-javascript-on-ios-and-android-mobile-safari/>

* 如果同时声明top和bottom的值，那么top值的优先级更高。如果同时声明left和right的值，那么优先级取决于网页的语言（例如，英语法语德语西班牙语）。比如，在英语的网页中，left的优先级更高；在阿拉伯语的网页中，right的优先级更高。

* 大家以后操作localStorage时记得加上 try { } catch，今天遇到ios safari隐私模式下报错进不了游戏。
