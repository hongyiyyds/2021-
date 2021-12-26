# 2021-
周鸿毅-201966345147
1.系统设计：
该系统设计了10个网页，分别为：
①小周商城主页面：商城主页面，可以看到商品等信息，也可以在个网页进入其他网页。

②商品详情页面：可以获得商品的信息以及加入购物车和购买等操作。

③购物车页面：
可以看到加入购物车的商品以及支付等操作。

④客户服务页面：
可以获得客服信息等进行处理。

⑤用户反馈页面：
用户可以在此页面提出反馈信息对网站问题进行提交。

⑥支付页面：
购物付款

⑦登陆页面：
用户登陆

⑧注册页面：
用户注册

⑨搜索页面：
搜索商品

⑩支付成功页面
支付成功提示


2.代码实现
（1）调用css和js文件
<head>
	<meta charset="UTF-8">
	<title>小周商城</title>
	<link rel="stylesheet" type="text/css" href="css文件/bootstrap.min.css">
	<link rel="stylesheet" href="css文件/font-awesome.min.css">
	<script src="js文件/jquery.js"></script>
	<script src="js文件/bootstrap.min.js"></script>
	<link rel="stylesheet" href="css文件/mall.css">
</head>
（2）设置顶部导航条等
<!-- 顶部导航条 -->
	<div class="nav">
		<ul>
			<li class="nav-pull-down location"><img src="img/小周地点标识符号乖巧小老妹.jpg"> 全国送达</li>
			<li><a href="小周商城.html">商城</a></li>
			<li><a href="小周商城.html">网站导航</a></li>
			<li><a href="客户服务.html">商城会员服务</a></li>
			<li><a href="购物车.html">购物车</a></li>
			<li><a href="用户反馈.html">反馈</a></li>
			<li><a href="客户服务.html">客户服务</a></li>
			<li class="nav-pull-down my-shop"><a href="小周商城.html">我的商城</a> <span class="glyphicon glyphicon-menu-down"></span></li>
			<li class="login-signup">你好，请<a href="登陆页面.html">登录 </a><span class="text-color-red"><a href="注册页面.html">免费注册</a></span></li>
		</ul>
	</div>


（3）幻灯片显示主页图片

<div class="nav-content">
				<!-- 幻灯片 -->
				<div class="slide">
					<img class="carousel_img" src="img/小周商城页面图片/主页辣条图1.jpg" name="1">
					<img class="carousel_img" src="img/小周商城页面图片/主页辣条图2.jpg" name="2">
					<img class="carousel_img" src="img/小周商城页面图片/主页辣条图3.jpg" name="3">
					<img class="carousel_img" src="img/小周商城页面图片/主页辣条图4.jpg" name="4">
					<img class="carousel_img" src="img/小周商城页面图片/主页辣条图5.jpg" name="5">
					<div class="icon">
						<i name="1" class="fa fa-circle"></i>
						<i name="2" class="fa fa-circle"></i>
						<i name="3" class="fa fa-circle"></i>
						<i name="4" class="fa fa-circle"></i>
						<i name="5" class="fa fa-circle"></i>
					</div>
					<div class="prev prevNext" onclick="PrevNextClick(1)"> <span class="glyphicon glyphicon-menu-left"></span> </div>
					<div class="next prevNext" onclick="PrevNextClick(2)"> <span class="glyphicon glyphicon-menu-right"></span> </div>
				</div>
				<div class="nav-show">
					<div class="nav-show-img"><img src="img/小周商城页面图片/主页下方辣条图1.jpg"></div>
					<div class="nav-show-img"><img src="img/小周商城页面图片/主页下方辣条图2.jpg"></div>
				</div>
			</div>



（4）登陆页面判断用户身份
<body>
	<div id="container">
		<div class="header">
			<p>登陆</p>
		</div>
		<div class="form-body">
			<form action="#">
				<div class="form-group">
					<label for="">用户名：</label>
					<input type="text" class="form-input">
				</div>
			</form>
			<form action="#">
				<div class="form-group">
					<label for="">密&nbsp;&nbsp;码：</label>
					<input type="password" class="form-input">
				</div>
			</form>
			<div class="btn">
				<input type="button" value="登陆" class="form-btn form-btn-primary">
				<input type="button" value="注册" class="form-btn form-btn-warning">
			</div>
		</div>
		<div class="footer">
			<p>by 2021 华工201966345147周鸿毅</p>
		</div>
	</div>
</body>



（5）注册页面用户身份注册
<body>
	<div class="container">
		<div class="info">
			<span>用户注册</span>
		</div>
		<form action="#">
			<div class="form-group">
				<p>
					<label for="">用户名：</label>
					<input type="text" class="form-input" name="username">
				</p>
			</div>
			<div class="form-group">
				<label for="">密&nbsp;&nbsp;码：</label>
				<input type="password" class="form-input" name="password">
			</div>
			<div class="form-group">
				<label for="">邮&nbsp;&nbsp;箱：</label>
				<input type="password" class="form-input" name="password">
			</div>
			<div class="radio">
				<span>性&nbsp;&nbsp;别：</span>
				<label><input type="radio" name="sex" value="male">&nbsp;&nbsp;男</label>
				<label><input type="radio" name="sex" value="female">&nbsp;&nbsp;女</label>
			</div>
			<div class="form-group">
				<label>城&nbsp;&nbsp;市：</label>
				<select class="form-input">
					<option>广州</option>
					<option>深圳</option>
					<option>佛山</option>
					<option>成都</option>
					<option>北京</option>
				</select>
			</div>
			<div class="btn">
				<input type="submit" value="注册" class="form-btn">
			</div>
		</form>
	</div>
</body>
