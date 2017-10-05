sketch.js
========================================
功能：实现SVG素描动画<br>
![test.gif](./test.gif)

使用方法如下：
----------------------------------------
引入文件
```
<script src="[path]/jquery-3.2.1.min.js"></script>
<script src="[path]/jQuery.sketch.js"></script>
```
选中父容器，并为它设置宽、高
```
<div id="content" style="width:800px;height:800px;"></div>
```
调用sketch()方法
```
$("#content").sketch({

	//SVG图案的路径
	d: "",
	
	//填充颜色
	fill: "none",
	
	//图案的轮廓颜色
	stroke: "#000",
	
	//图案的轮廓宽度
	strokeWidth: "1px",
	
	//是否同时改变透明度
	opacity: "false",
	
	//动画持续时间
	time: 4500
	
});
```
d的值是SVG图案的路径，画出来是什么样就是由这个参数来决定的。你可以自己写，也可以用记事本方式打开你已拥有的.SVG文件，找到“path”标签，将其中“d”属性中的内容复制过来<br>
