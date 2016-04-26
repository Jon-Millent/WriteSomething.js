# WriteSomething.js
**这是一个用js模拟打字的小程序，很炫酷**<br />

**JavaScript**
```javascript
//如何使用

//引入js文件
<script type="text/javascript" src="js/WriteSomething.js"></script>

//配置参数

var try=new WriteSomething();

try.doit('main',{//main为id名字
	data:['hello world','how are you?'],//要显示的每句话
	frequency:500,//光标闪烁时间间隔,默认为500
	textChange:600,//打字的速度,默认为100
	replay:true,//当文字显示完后是否重新播放，默认为true
	stop:4000,//当每句话显示完后的时间间隔,默认为4000
});
```
**HTML**
```html
//引入这段html
<div class="showtext" id="main">
	<div><h1></h1></div><span></span>
</div>
```
**css**
```css
//引入WriteSomethingStyle.css
<link type="text/css" rel="stylesheet" href="css/WriteSomethingStyle.css" >
//或者
.showtext div{
	display: inline-block;
}
.showtext div h1{
	color: #E8E8FF;
}
.showtext span{
	display: inline-block;
	width: 8px;
	height: 30px;
	background-color: #fff;
	margin-left: 6px;
	margin-bottom: -4px;
}

```
