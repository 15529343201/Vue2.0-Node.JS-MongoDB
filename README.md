### vue框架对比
Vue和React对比<br>
- Angular提供的更多是一整套解决方案,后者更像是一个生态
- Vue和React目前都使用了Virtual Dom
![image](https://github.com/15529343201/Vue2.0-Node.JS-MongoDB/blob/chapter1/image/1.PNG)

Vue<br>
- 模板和渲染函数的弹性选择
- 简单的语法及项目创建
- 更快的渲染速度和更小的体积

React<br>
- 更适用于大型应用和更好的可测试性
- 同时适用于Web端和原生App
- 更大的生态圈带来的更多支持和工具

Vue和React相同点<br>
- 利用虚拟DOM实现快速渲染
- 轻量级
- 响应式组件
- 服务器端渲染
- 易于集成路由工具,打包工具以及状态管理工具
- 优秀的支持和社区

### 前端JS框架回顾
![image](https://github.com/15529343201/Vue2.0-Node.JS-MongoDB/blob/chapter1/image/2.PNG)
![image](https://github.com/15529343201/Vue2.0-Node.JS-MongoDB/blob/chapter1/image/3.PNG)
![image](https://github.com/15529343201/Vue2.0-Node.JS-MongoDB/blob/chapter1/image/4.PNG)
![image](https://github.com/15529343201/Vue2.0-Node.JS-MongoDB/blob/chapter1/image/5.PNG)
![image](https://github.com/15529343201/Vue2.0-Node.JS-MongoDB/blob/chapter1/image/6.PNG)

### vue概况以及核心思想
- Vue本身并不是一个框架
- Vue结合周边生态系统构成一个灵活的、渐进式的框架

声明式渲染(Declaralive Rendering)-->组件系统(Component System)-->客户端路由(Client-Slide Routing)-->大规模状态管理(Large Scaie State Management)-->构建工具(Build System)<br>
核心思想:<br>
- 数据驱动
- 组件化

通过MVVM的数据绑定实现自动同步<br>
![image](https://github.com/15529343201/Vue2.0-Node.JS-MongoDB/blob/chapter1/image/7.PNG)

Vue组件化<br>
![image](https://github.com/15529343201/Vue2.0-Node.JS-MongoDB/blob/chapter1/image/8.PNG)

Vue组件树<br>
![image](https://github.com/15529343201/Vue2.0-Node.JS-MongoDB/blob/chapter1/image/9.PNG)

Vue如何实现双向数据绑定?<br>
- Object.defineProperty()函数
```HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
	<title>Title</title>
</head>
<body>
<input type="text" id="userName">
<br>
<span id="uName"></span>
<script>
    var obj={
	    pwd:"123456"
	};
	Object.defineProperty(obj,"userName",{
	    get: function(){
		    console.log("get init");
		},
		set: function(val){
		    console.log("set init");
			document.getElementById("uName").innerText=val;
			document.getElementById("userName").value=val;
		}
	});
	document.getElementById("userName").addEventListener("keyup",function(event){
	    obj.userName=event.target.value;
	})
</script>
</body>
</html>
```
![image](https://github.com/15529343201/Vue2.0-Node.JS-MongoDB/blob/chapter1/image/10.PNG)

前置知识<br>
- html/css/js
- Vue
- ES6
- Node
- Npm
- Webpack

### nodejs和npm的安装和环境搭建
- Webpack 代码模块化构建打包工具
- Gulp基于流的自动化构建工具
- Grunt JavaScript世界的构建工具
- Babel使用最新的规范来编写js
- Vue构建数据驱动的web界面的渐进式框架
- Express基于Node.js平台,快速、开放、极简的web开发框架

