---
title: "Pure CSS cloud effect "
subtitle: by using only HTML and CSS
category:
  - HTML & CSS design
author: Harshit Kumar
date: 2020-06-26T23:06:54.616Z
featureImage: /uploads/clouds-using-css.png
---
Hi guys !!!

Welcome back to my blog again.

This time I have made an awesome looking cloud animation just by using HTML and CSS only. 

And that also with only few lines of code.

If you new around here, don't forget to subscribe to my channel Catalyst Coder on YouTube (link on the bottom of the page)

because I will be posting awesome new content every week or twice a week.



Please support us all in this though time of Covid-19.

![Pure CSS cloud effect [by using only HTML and CSS] - CSS animation  (2020)](/uploads/clouds-using-css.png "Pure CSS cloud effect [by using only HTML and CSS] - CSS animation  (2020)")

# YouTube 

If you guys haven't seen my video on this topic, then please give it a look : https://youtu.be/V5TzSm-INrY



# Source Code

Here are the codes which I used in the video. 

And seriously, Subscribe to the channel, you might be missing a lot.

**HTML**

```html
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title>Clouds using css</title>
    <link rel="stylesheet" href="style.css">
  </head>
  <body>
    <div id="background-wrap">
      <div class="x1">
        <div class="cloud"></div>
      </div>
      <div class="x2">
        <div class="cloud"></div>
      </div>
      <div class="x3">
        <div class="cloud"></div>
      </div>
      <div class="x4">
        <div class="cloud"></div>
      </div>
      <div class="x5">
        <div class="cloud"></div>
      </div>
    </div>
  </body>
</html>

```



**CSS**

```css
body{
	background: #00b4ff;
	color:#333;
	height:100vh;
	margin:0;
	padding:0;
	overflow-x: hidden;
}
#background-wrap{
	padding-top:50px;
	width:100%;
	position:fixed;
	z-index:-1;
}
@-webkit-keyframes animateCloud{
	0% {margin-left:-1000px;}
	100%{margin-left:100%;}
}
.x1{
	-webkit-animation: animateCloud 40s linear infinite;
	-webkit-transform:scale(0.65);
}
.x2{
	-webkit-animation: animateCloud 20s linear infinite;
	-webkit-transform:scale(0.3);
}
.x3{
	-webkit-animation: animateCloud 30s linear infinite;
	-webkit-transform:scale(0.5);
}
.x4{
	-webkit-animation: animateCloud 15s linear infinite;
	-webkit-transform:scale(0.4);
}
.x5{
	-webkit-animation: animateCloud 25s linear infinite;
	-webkit-transform:scale(0.55);
}

.cloud{
	background: #fff;
	border-radius:100px;
	box-shadow :0 8px 5px rgba(0,0,0,0.1);
	height:120px;
	position: relative;
	width:350px;
}
.cloud:after, .cloud:before{
	background:#fff;
	content:"";
	position: absolute;
	z-index: -1;

}
.cloud:after{
	border-radius:100px;
	height:100px;
	left:50px;
	top:-50px;
	width:100px;
}
.cloud:before{
	border-radius:200px;
	width:180px;
	height:180px;
	right:50px;
	top:-90px;
}

```





Hope you are all well and Happy in these tough times of 2020. 

Happy Coding :)