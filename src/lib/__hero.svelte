<div class="hero">
	<h1>Sense<span>- Welcome to Education -</span></h1>
</div>

<style>
    @import url(https://fonts.googleapis.com/css?family=Open+Sans:600,300);
* {
	margin: 0;
	padding: 0;
}
.hero {
	height: 75vh;
	background: linear-gradient(45deg, rgba(100,216,243,.7), rgba(245,146,176,.7), rgba(52,219,216,.7)) 0 0 / 1000% no-repeat, 0 0 / cover no-repeat;
	-webkit-animation: gradientAnimation 40s ease infinite;
	animation: gradientAnimation 40s ease infinite;
}
@-webkit-keyframes gradientAnimation {
	0%   { background-position: 0% 30%, 0 0;}
	50%  { background-position: 100% 70%, 0 0;}
	100% { background-position: 0% 30%, 0 0;}
}
@keyframes gradientAnimation {
	0%   { background-position: 0% 30%, 0 0;}
	50%  { background-position: 100% 70%, 0 0;}
	100% { background-position: 0% 30%, 0 0;}
}
h1 {
	position: absolute;
	top: 50%;
	left: 50%;
	-webkit-transform: translate(-50%, -50%);
	transform: translate(-50%, -50%);
	color: #fff;
	font : normal 600 72px/1 'Open Sans', sans-serif;
	text-align: center;
	white-space: nowrap;
}
h1 span {
	display: block;
	margin-top: 1em;
	font-size: 40px;
	font-weight: 300;
}
</style>
