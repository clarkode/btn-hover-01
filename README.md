# btn-hover-01
button hover effect css html

# Powered by: Clarkode
Website: clarkode.com

# CODE 

HTML
-------------------------------------------------------------------------
<!DOCTYPE html>
<html lang="es">
<head>
	<meta charset="utf-8">
	<title>Button Hover CSS3</title>
	<link rel="stylesheet" type="text/css" href="main.css">
</head>
<body>
	<a href="#" class="btn">
		<span class="btn__line"></span>
		<span class="btn__line"></span>
		<span class="btn__line"></span>
		<span class="btn__line"></span>
		BTN HOVER CSS
	</a>
</body>
</html>
-------------------------------------------------------------------------

CSS
-------------------------------------------------------------------------
*{
	margin: 0;
	padding: 0;
	box-sizing: border-box;
}
body{
	display: flex;
	align-items: center;
	justify-content: center;
	text-align: center;
	min-height: 100vh;
	background: #000;
	font-family: sans-serif;
}

.btn{
	position: relative;
	padding: 15px 30px;
	color: green;
	font-size: 25px;
	letter-spacing: 1px;
	background: none;
	text-decoration: none;
	transition: 0.5s linear;
	transition-delay: 0s;
	overflow: hidden;
}
.btn:hover{
	background: green;
	color: #fff;
	transition: 0.5s linear;
	transition-delay: 1s;
}

.btn__line{
	position: absolute;
	display: block;
}
.btn__line:nth-child(1){
	top: 0;
	left: -100%;
	width: 100%;
	height: 2px;
	background: linear-gradient(90deg, transparent, green);
	transition: 0.5s;
	transition-delay: 1s;
}
.btn:hover .btn__line:nth-child(1){
	left: 100%;
	transition: 1s;
}

.btn__line:nth-child(2){
	top: -100%;
	right: 0;
	width: 2px;
	height: 100%;
	background: linear-gradient(180deg, transparent, green);
	transition: 0.5s;
	transition-delay: 0.75s;
}
.btn:hover .btn__line:nth-child(2){
	top: 100%;
	transition: 1s;
	transition-delay: 0.25s;
}

.btn__line:nth-child(3){
	bottom: 0;
	right: -100%;
	width: 100%;
	height: 2px;
	background: linear-gradient(270deg, transparent, green);
	transition: 0.7s;
	transition-delay: 0.25s;
}
.btn:hover .btn__line:nth-child(3){
	right: 100%;
	transition: 1s;
	transition-delay: 0.5s;
}

.btn__line:nth-child(4){
	top: 100%;
	left: 0;
	width: 2px;
	height: 100%;
	background: linear-gradient(360deg, transparent, green);
	transition: 0.5s;
	transition-delay: 0s;
}
.btn:hover .btn__line:nth-child(4){
	top: -100%;
	transition: 1s;
	transition-delay: 0.75s;
}

