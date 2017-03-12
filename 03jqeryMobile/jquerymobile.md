WebApp - day01
========================================
- 01_认识移动Web应用开发
- 02_Android中创建加载简单的html界面
- 03_JQM创建具有移动风格的html5界面
- 04_用PhoneGap创建移动应用3种方式
- 05_创建一个标准的JQM界面
- 06_JQM_UI_界面跳转及对话框
- 07_JQM_UI_常见控件
- 08_JQM_界面初始化事件
- 09_JQM_常用的触摸事件_系统事件
- 10_PhoneGap_调用系统组件

-----------------------------------------



三个优点1. 上手迅速并支持快速迭代2. 避免麻烦的应用商店审批过程以及调试、构建带来的痛苦3. 支持跨平台和跨设备开发html5
三个缺点1. 比原生程序运行慢2. 界面在不同平台浏览器效果略微不同3. 功能不完善

常见移动开发框架(支持html5)
jQueryMobile (基于jQuery-JavaScript) html驱动
Sencha touch(基于ExtJs) js驱动
jQTouch (基于jQuery) 
Bootstrap (Twitter推出)
jQuery



1.jQuery

	jQuery是一个快速、简洁的JavaScript框架，是继Prototype之后又一个优秀的JavaScript代码库（或JavaScript框架）。jQuery设计的宗旨是“write Less，Do More”，即倡导写更少的代码，做更多的事情。它封装JavaScript常用的功能代码，提供一种简便的JavaScript设计模式，优化HTML文档操作、事件处理、动画设计和Ajax交互

	jQuery的核心特性可以总结为：具有独特的链式语法和短小清晰的多功能接口；具有高效灵活的css选择器，并且可对CSS选择器进行扩展；拥有便捷的插件扩展机制和丰富的插件。jQuery兼容各种主流浏览器，如IE 6.0+、FF 1.5+、Safari 2.0+、Opera 9.0+等
	


2.jQueryMobile
	
	用于创建移动 Web 应用的前端开发框架。
	jQuery Mobile是jQuery针对手机和平板设备的版本。包含jQuery核心库和专门针对主流移动平台设计的完整统一的jQuery移动UI框架。
	jQuery Mobile本身也是对JavaScript的封装，属于jQuery的一个插件
	jQuery Mobile 的功能是开发html5界面内容，这些界面效果和NativeApp（本地应用）很相似。可以使用PhoneGap将这些内容打包成不同平台的WebApp部署在移动设备上。
	官网地址：http://jquerymobile.com

3.AJAX

	AJAX 指异步JavaScript及XML（AsynchronousJavascript+XML）。
	Web应用的交互如Flickr,Backpack和Google在这方面已经有质的飞跃。这个术语源自描述从基于Web的应用到基于数据的应用的转换。在基于数据的应用中，用户需求的数据如联系人列表，可以从独立于实际网页的服务端取得并且可以被动态地写入网页中，给缓慢的Web应用体验着色使之像桌面应用一样。
	Ajax的核心是JavaScript对象XmlHttpRequest。该对象在Internet Explorer 5中首次引入，它是一种支持异步请求的技术。简而言之，XmlHttpRequest使您可以使用JavaScript向服务器提出请求并处理响应，而不阻塞用户。

4.PhoneGap--开发平台-->创建跨平台移动应用程序(可访问设备的api)

	PhoneGap是一个用基于HTML，CSS和JavaScript的，创建移动跨平台移动应用程序的---快速开发平台。它使开发者能够利用IOS，Android，Palm，Symbian,WP7,WP8,Bada和Blackberry智能手机的核心功能——包括地理定位，加速器，联系人，声音和振动等，此外PhoneGap拥有丰富的插件，可以调用。

	重点是访问本地设备的API




----------------------------------------------
1.开发

	1.jQueryMobile
		JQM创建具有移动风格的html5界面

		开发准备流程
		1. 文档声明设置为HTML5
		2. 在Header标签中添加 //适配手机屏幕
			<meta name="viewport" content="width=device-width, initial-scale=1">
		3. 新建html文件，引入一个css、两个js
			 <link rel="stylesheet" href="css/jquery.mobile-1.4.5.min.css" />
		 	<script src="js/jquery-1.4.5.min.js"></script>
		 	<script src="js/jquery.mobile-1.4.5.min.js"></script>
		4. 在body中添加
		<div data-role="page">
			<div data-role="header">标题</div>
			<div data-role="content">内容</div>
			<div data-role="footer">页脚</div>
		</div>

