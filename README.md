## 移动端mate标签

    <meta name = "viewport" content = "width = device-width, initial-scale = 1.0, maximum-scale = 1.0, user-scalable = 0" />
* width - 可视区域的宽度，值可为数字或关键词device-width
* height - viewport的高度
* initial-scale - 初始的缩放比例
* minimum-scale - 允许用户缩放到的最小比例
* maximum-scale - 允许用户缩放到的最大比例
* user-scalable - 用户是否可以手动缩放
* header 和 footer

## 一、天猫触屏版

    <title>天猫触屏版</title>
    <meta content="text/html; charset=utf-8" http-equiv="Content-Type"> 
    <meta charset="utf-8"> 
    <meta content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=0" name="viewport"> 
    <meta content="yes" name="apple-mobile-web-app-capable"> 
    <meta content="black" name="apple-mobile-web-app-status-bar-style"> 
    <meta content="telephone=no" name="format-detection">
## 二、淘宝
    <title>淘宝网触屏版</title>
    <meta charset="utf-8">
    <meta content="yes" name="apple-mobile-web-app-capable">
    <meta content="yes" name="apple-touch-fullscreen">
    <meta content="telephone=no" name="format-detection">
    <meta content="black" name="apple-mobile-web-app-status-bar-style">
    <meta property="wb:webmaster" content="c51923015ca19eb1">
    <meta name="author" content="m.taobao.com">
    <meta name="copyright" content="Copyright ©m.taobao.com 版权所有">
    <meta name="revisit-after" content="1 days">
    <meta name="keywords" content="">
    <meta name="description" content="">
## 三、京东
    <title> 京东 - 手机版 </title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=0;">
    <meta name="format-detection" content="telephone=no">
    <meta name="Keywords" content="手机购物,WAP商城,日用百货,3C家电,汽车用品">
    <meta name="description" 
    content="京东手机版提供了包括数码、家电、手机、电脑配件、网络产品、
    日用百货等数万种商品，手机快捷购物，就上京东手机版。">
## 四、网易
    <title>手机网易网</title>
    <meta charset="UTF-8">
    <meta content="width=device-width,user-scalable=no" name="viewport">
    <meta name="apple-itunes-app" content="app-id=425349261">
    <meta name="apple-mobile-web-app-capable" content="yes">
## 五、百度
    <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
    <meta name="viewport" content="width=device-width,minimum-scale=1.0,maximum-scale=1.0,user-scalable=no">
    <meta name="format-detection" content="telephone=no">
meta指元素可提供有关页面的元信息（meta-information），比如针对搜索引擎和更新频度的描述和关键词。 标签位于文档的头部，不包含任何内容。 标签的属性定义了与文档相关联的名称/值对。

## 六、手机端特有的有哪些？
    <meta content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=0" name="viewport"> 
    <meta content="yes" name="apple-mobile-web-app-capable"> 
    <meta content="black" name="apple-mobile-web-app-status-bar-style"> 
    <meta content="telephone=no" name="format-detection">
第一个meta标签表示：
强制让文档的宽度与设备的宽度保持 1:1，并且文档最大的宽度比例是 1.0，且不允许用户点击屏幕放大浏览；

* width - viewport 的宽度

* height - viewport的高度

* initial-scale - 初始的缩放比例

* minimum-scale - 允许用户缩放到的最小比例

* maximum-scale - 允许用户缩放到的最大比例

* user-scalable - 用户是否可以手动缩放

第二个 meta 标签是 iphone 设备中的 safari 私有 meta 标签，它表示：允许全屏模式浏览；

第三个 meta 标签也是 iphone 的 私有 标签，它指定的 iphone 中 safari 顶端的状态条的样式； 在 web app 应用下状态条（屏幕顶部条）的颜色； 默认值为default（白色），可以定为 black（黑色）和 black-translucent（灰色半透明）。 注意：若值为 “black-translucent” 将会占据页面px位置，浮在页面上方 （会覆盖页面 20px 高度–iphone 4 和 itouch 4 的 Retina 屏幕为 40px）。

第四个meta标签表示：告诉设备忽略将页面中的数字识别为电话号码。

    <meta name = "viewport" content = "width = device-width, initial-scale = 1.0, maximum-scale = 1.0, user-scalable = 0" />
* width - 可视区域的宽度，值可为数字或关键词 device-width

* height - viewport的高度

* initial-scale - 初始的缩放比例

* minimum-scale - 允许用户缩放到的最小比例

* maximum-scale - 允许用户缩放到的最大比例

* user-scalable - 用户是否可以手动缩放 header 和 footer


        $("body>*").on("touchstart",function(e){
            let _con = $(".baMaYD_head_choose_c");   // 设置目标区域
            if(!_con.is(e.target) && _con.has(e.target).length === 0){
                _con.parent().removeClass("active");
            }
        });
