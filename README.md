<!DOCTYPE html>
<html lang="en">
	<head>
		<meta charset="utf-8">
		<meta http-equiv="X-UA-Compatible" content="IE=edge">
		<meta name="viewport" content="width=device-width, initial-scale=1">
		 <!-- The above 3 meta tags *must* come first in the head; any other head content must come *after* these tags -->

		<title>College Management System - ASD A33</title>

		<!-- Google font -->
		<link href="https://fonts.googleapis.com/css?family=Lato:700%7CMontserrat:400,600" rel="stylesheet">

		<!-- Bootstrap -->
			<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u" crossorigin="anonymous">
		<!-- Font Awesome Icon -->
		<link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.8.1/css/all.css" integrity="sha384-50oBUHEmvpQ+1lW4y57PTFmhCaXp0ML5d60M1M7uH2+nqUivzIebhndOJK28anvf" crossorigin="anonymous">

		<!-- Custom stlylesheet -->
		<style media="screen">
		body {
	font-family: 'Montserrat', sans-serif;
font-size: 15px;
	font-weight: 400;
	color: #798696;
overflow-x:hidden;
}

h1,h2,h3,h4,h5,h6 {
margin-top: 12px;
margin-bottom: 15px;
font-weight: 600;
color: #374050;
}

h1 {
font-size:38px;
}

h2 {
font-size:30px;
}

h3 {
font-size:24px;
}

h4 {
font-size:18px;
}

a {
font-family: 'Lato', sans-serif;
color: #374050;
font-weight: 700;
}

a:hover,
a:focus{
	text-decoration: none;
	outline: none;
color: #374050;
opacity: 0.9;
}

ul,ol{
	margin: 0;
	padding: 0;
	list-style: none
}

.white-text {
color: #FFF;
}

.section {
	position:relative;
	padding-top:80px;
	padding-bottom:80px;
}

.section-hr {
	margin-top:80px;
	margin-bottom:80px;
	border-color: #EBEBEB;
}

.section-header {
	margin-bottom:40px;
}

/* --- Background Image --- */
.bg-image {
	position:absolute;
	left:0;
	right:0;
	top:0;
	bottom:0;
	background-position:center;
	background-size:cover;
}

.bg-image.bg-parallax {
	background-attachment:fixed;
}

.bg-image.overlay:after {
	content:"";
	position:absolute;
	left:0;
	right:0;
	top:0;
	bottom:0;
	background-image: -webkit-gradient(linear, left top, left bottom, from(#374050), to(#798696));
	background-image: linear-gradient(to bottom, #374050 0%, #798696 100%);
	opacity: 0.7;
}

/* --- Buttons --- */
.main-button {
	position:relative;
	display:inline-block;
	padding:10px 30px;
	background-color: #FF6700;
	border: 2px solid transparent;
	border-radius: 40px;
	color: #FFF;
	-webkit-transition:0.2s all;
	transition:0.2s all;
}

.main-button:hover , .main-button:focus {
	background-color:#fff;
	border: 2px solid #FF6700;
	color:#FF6700;
}

.main-button.icon-button:hover , .main-button.icon-button:focus {
	padding-right: 45px;
}

.main-button.icon-button:after {
	content:"\f178";
	font-family:FontAwesome;
	position:absolute;
	width: 30px;
	right: 15px;
	text-align:center;
	opacity:0;
	-webkit-transition:0.2s all;
	transition:0.2s all;
}

.main-button.icon-button:hover:after , .main-button.icon-button:focus:after {
	opacity:1;
}

textarea {
    padding: 10px 15px;
}


.navbar-brand {
    padding: 0;
}

.navbar-brand .logo {
	margin-top: 10px;
	display: inline-block;
}

.navbar-brand .logo > img {
	max-height:30px;
}

@media only screen and (max-width: 767px) {
	.navbar-brand {
		margin-left:15px;
	}
}

/*------------------------------------*\
	Navigation
\*------------------------------------*/
#header {
	position:relative;
	left:0;
	right:0;
	top:0;
	z-index:99;
	border-bottom:1px solid rgba(235, 235, 235, 0.25);
	background-color:#FFF;
	-webkit-transition:0.2s all;
	transition:0.2s all;
}

#header.transparent-nav {
	position:absolute;
	background-color: transparent;
}

#header.transparent-nav .main-menu li a {
	color:#FFF;
}

.main-menu li a {
	text-transform:uppercase;
	-webkit-transition:0.2s all;
	transition:0.2s all;
}

.main-menu li a:hover , .main-menu li a:focus {
	background-color:transparent;
}

.main-menu li a:after {
	content:"";
	display:block;
	height:2px;
	background-color:#FF6700;
	width:100%;
	-webkit-transform: translateY(5px);
	    -ms-transform: translateY(5px);
	        transform: translateY(5px);
	opacity:0;
	-webkit-transition:0.2s all;
	transition:0.2s all;
}

.main-menu li a:hover:after , .main-menu li a:focus:after {
	-webkit-transform: translateY(0px);
	    -ms-transform: translateY(0px);
	        transform: translateY(0px);
	opacity:1;
}

@media only screen and (max-width: 767px) {
	#nav {
		position: fixed;
		top: 0;
		right: 0;
		width: 0%;
		max-width:250px;
		height: 100vh;
		background: #FFF;
		-webkit-box-shadow: 0px 5px 10px 0px rgba(0, 0, 0, 0.1);
		        box-shadow: 0px 5px 10px 0px rgba(0, 0, 0, 0.1);
		padding-top: 80px;
		padding-bottom: 40px;
		-webkit-transform: translateX(100%);
		    -ms-transform: translateX(100%);
		        transform: translateX(100%);
		-webkit-transition: 0.4s all cubic-bezier(.77,0,.18,1);
		transition: 0.4s all cubic-bezier(.77,0,.18,1);
		z-index:9;
	}

	#header.nav-collapse #nav{
		width:100%;
		-webkit-transform: translateX(0%);
		    -ms-transform: translateX(0%);
		        transform: translateX(0%);
	}

	.main-menu {
		margin:0;
	}

	.main-menu li a {
		color: #374050 !important;
		display: inline-block;
		margin-left: 40px;
	}
}

/* -- Mobile Toggle Btn -- */
.navbar-toggle {
	position:fixed;
	right:0;
	padding: 0;
	height: 40px;
	width: 40px;
	margin-top: 5px;
	z-index:99;
}

.navbar-toggle > span {
	position: absolute;
	top: 50%;
	left: 50%;
    -webkit-transform: translate(-50% , -50%);
        -ms-transform: translate(-50% , -50%);
            transform: translate(-50% , -50%);
	-webkit-transition: 0.2s background;
	transition: 0.2s background;
}

.navbar-toggle > span:before, .navbar-toggle > span:after {
	content: '';
	position:absolute;
	left:0;
	-webkit-transition: 0.2s -webkit-transform;
	transition: 0.2s -webkit-transform;
	transition: 0.2s transform;
	transition: 0.2s transform, 0.2s -webkit-transform;
}

.navbar-toggle > span , .navbar-toggle > span:before , .navbar-toggle > span:after {
	height: 2px;
	width: 25px;
	background-color:#374050;
}

.navbar-toggle > span:before {
	top: -10px;
}

.navbar-toggle > span:after {
	top: 10px;
}

#header.nav-collapse .navbar-toggle > span {
	background: transparent;
}

#header.nav-collapse .navbar-toggle > span:before {
    -webkit-transform: translateY(10px) rotate(45deg);
        -ms-transform: translateY(10px) rotate(45deg);
            transform: translateY(10px) rotate(45deg);
}

#header.nav-collapse .navbar-toggle > span:after {
    -webkit-transform: translateY(-10px) rotate(-45deg);
        -ms-transform: translateY(-10px) rotate(-45deg);
            transform: translateY(-10px) rotate(-45deg);
}

/*------------------------------------*\
	Hero Area
\*------------------------------------*/
.hero-area {
	position:relative;
	padding-top: 80px;
	padding-bottom: 80px;
}

#home.hero-area {
	height:calc(100vh - 80px);
	padding-top: 0px;
	padding-bottom: 0px;
}

.home-wrapper {
	position:absolute;
	top:50%;
	-webkit-transform:translateY(-50%);
	    -ms-transform:translateY(-50%);
	        transform:translateY(-50%);
	left:0;
	right:0;
}

/* -- Breadcrumb -- */
.hero-area-tree li {
	display:inline-block;
	font-family: 'Lato', sans-serif;
	font-weight:600;
	font-size:14px;
	color:rgba(255, 255, 255, 0.8);
}

.hero-area-tree li > a {
	color:rgba(255, 255, 255, 0.8);
}

.hero-area-tree li + li:before {
	content: "/";
	display: inline-block;
	margin: 0px 5px;
	color: rgba(235, 235, 235, 0.25);
}

/*------------------------------------*\
	About & Why Us (Feature)
\*------------------------------------*/
/* -- Feature -- */
.feature {
	position:relative;
}

.feature + .feature  {
	margin-top:40px;
}

.feature .feature-icon {
	position:absolute;
	left:0;
	top:0;
	width:80px;
	height:80px;
	line-height:80px;
	text-align:center;
	border-radius: 50%;
	font-size:30px;
	border:1px solid #EBEBEB;
	color:#FF6700;
}

.feature-content {
	padding-left:100px;
}

.about-img {
	margin-top:40px;
}

.about-img > img {
	width:100%;
}

.course {
	margin-top:20px;
	margin-bottom:20px;
}

.course .course-img {
	position: relative;
	display:block;
	margin-bottom:20px;
	border-radius:4px;
	overflow:hidden;
}

.course .course-img > img {
	width:100%;
}

.course-img:after {
	content:"";
	position:absolute;
	left:0;
	right:0;
	bottom:0;
	top:0;
	background-color:#FF6700;
	opacity:0;
	-webkit-transition:0.2s opacity;
	transition:0.2s opacity;
}

.course .course-img:hover:after {
	opacity:0.7;
}

.course .course-img .course-link-icon {
	position:absolute;
	left:50%;
	top:50%;
	-webkit-transform: translate(-50% , calc(-50% - 15px));
	    -ms-transform: translate(-50% , calc(-50% - 15px));
	        transform: translate(-50% , calc(-50% - 15px));
	width:40px;
	height:40px;
	line-height:40px;
	text-align:center;
	border:2px solid #fff;
	color:#fff;
	border-radius:50%;
	opacity:0;
	z-index:10;
	-webkit-transition:0.2s all;
	transition:0.2s all;
}

.course .course-img:hover .course-link-icon {
	-webkit-transform: translate(-50% , -50%);
	    -ms-transform: translate(-50% , -50%);
	        transform: translate(-50% , -50%);
	opacity:1;
}

.course .course-title {
	display:block;
	height:42px;
}

.course .course-details {
	margin-top: 20px;
	padding-top: 10px;
	border-top: 1px solid #EBEBEB;
}

.course .course-details .course-price {
	float: right;
}

.course .course-details .course-price.course-free {
	color: green;
}

.course .course-details .course-price.course-premium {
	color: #FF6700;
}

#courses .center-btn {
	text-align:center;
	margin-top:40px;
}


		</style>

    </head>
	<body>

		<!-- Header -->
		<header id="header" class="transparent-nav">
			<div class="container">

				<div class="navbar-header">
					<div class="navbar-brand">
					</div>

					<!-- Mobile toggle -->
					<button class="navbar-toggle">
						<span></span>
					</button>
					<!-- /Mobile toggle -->
				</div>

				<!-- Navigation -->
				<nav id="nav" class="navbar-fixed-top">
					<ul class="main-menu nav navbar-nav navbar-right">
						<li><a href="">Home</a></li>
						<li><a href="">Instructors</a></li>
						<li><a href="">Departments</a></li>
						<li><a href="">Students</a></li>
						<li><a href="">Sections</a></li>
						<!-- <li> <a href="#">Teaches</a> </li> -->
					</ul>
				</nav>
				<!-- /Navigation -->

			</div>
		</header>
		<!-- /Header -->

		<!-- Home -->
		<div id="home" class="hero-area">

			<!-- Backgound Image -->
			<div class="bg-image bg-parallax overlay" style="background-image:url(https://i.imgur.com/YDwNPZg.jpg)"></div>
			<!-- /Backgound Image -->

			<div class="home-wrapper">
				<div class="container">
					<div class="row">
						<div class="col-md-8">
							<h1 class="white-text">College Management System</h1>
							<p class="lead white-text">Agile Software Development A40 </p>
						</div>
					</div>
				</div>
			</div>

		</div>

		<!-- About -->
		<div id="about" class="section">

			<!-- container -->
			<div class="container">

				<!-- row -->
				<div class="row">

					<div class="col-md-6">
						<div class="section-header">
							<h2>Welcome to CMS of Sanjay Ghodawat University</h2>
							<p class="lead">College management system consisting of  Students, Instructors, Departments and Sections.</p>
						</div>

						<!-- feature -->
						<div class="feature">
							<i class="feature-icon fa fa-flask"></i>
							<div class="feature-content">
								<a href=""><h4>Departments </h4></a>
								<p>Click to view the list of departments in the college.</p>
							</div>
						</div>
						<!-- /feature -->

						<!-- feature -->
						<div class="feature">
							<i class="feature-icon fa fa-users"></i>
							<div class="feature-content">
								<a href=""><h4>Instructors</h4></a>
								<p>Click to view the info about instructors of the college.</p>
							</div>
						</div>
						<!-- /feature -->

						<!-- feature -->
						<div class="feature">
							<i class="feature-icon fab fa-simplybuilt"></i>
							<div class="feature-content">
								<a href=""><h4>Sections</h4></a>
								<p>Click to view the details about sections in the college.</p>
							</div>
						</div>
						<!-- /feature -->

					</div>

					<div class="col-md-6">
						<div class="about-img">
							<img src="https://i.imgur.com/qw0AWhu.png" alt="">
						</div>
					</div>

				</div>
				<!-- row -->

			</div>
			<!-- container -->
		</div>
		<!-- /About -->

		<!-- Courses -->
		<div id="courses" class="section">

			<!-- container -->
			<div class="container">

				<!-- row -->

		<!-- /Footer -->

		<!-- preloader -->
		<div id='preloader'><div class='preloader'></div></div>
		<!-- /preloader -->


		<!-- jQuery Plugins -->
		<script type="text/javascript" src="js/jquery.min.js"></script>
		<script type="text/javascript" src="js/bootstrap.min.js"></script>
		<script type="text/javascript" src="js/main.js"></script>

	</body>
</html>
