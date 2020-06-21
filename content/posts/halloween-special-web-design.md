---
title: Halloween special web design
subtitle: "Cat animation using html and css only "
category:
  - HTML & CSS design
author: Harshit Kumar
date: 2020-06-21T23:12:52.729Z
featureImage: /uploads/halloween-cat-animation.png
---
![Halloween cat animation using html and css only](/uploads/halloween-cat-animation_final.png "Halloween cat animation using html and css only")

Hi guys, Since Halloween is in few months. So I made this a Halloween special web design, so everyone can use this thier Halloween special themed website. In this web design , I am generating a Cat and moon and some clouds just by using html and css. Since it is purely generated in HTML and CSS it doesn't decrease the load time of the website. Comment below and tell me your thoughts on this video.



# **Youtube Video link**

If you guys haven't **watch my video** or the **live demo of this desgin**, Simply click on this link and **watch the video** :- <https://youtu.be/YEN1mrZrrV8>

![Halloween cat animation using html and css only](/uploads/halloween-cat-animation.png "Halloween cat animation using html and css only")







# **Source Code**

The coding is done in HTML5 and CSS3 which is widely used this days in all the websites , so this code won't cause any problem in the website. If it still does, then comment below or head over to Contact page and contact us by filling the form.

**HTML**

```html
<!DOCTYPE html>
<html lang="en" >
<head>
  <meta charset="UTF-8">
  <title>Halloween Cat Animation</title>
  <link rel="stylesheet" href="./style.css">

</head>
<body>
<div class="box">
  <div class="cat">
    <span class="eyes left"></span>
    <span class="eyes right"></span>
    <span class="mouth"></span>
  </div>
  <div class="moon">
    <div class="sphere"></div>
  </div>
  <div class="cloud-container">
    <div class="cloud"></div>
    <div class="cloud"></div>
    <div class="cloud"></div>
    <div class="cloud"></div>
  </div>
</div>
</body>
</html>

```

**CSS**

```css
body{background:#02112d;}
div{
  display: block;
  position: absolute;
  margin: auto;
  top:0;
  bottom:0;
  left:0;
  right:0;
}
.box{
  height: 500px;
  width:500px;
  margin:auto;
}
.cloud{
  background: #464145;
  width:100px;
  height:50px;
  -webkit-animation: clouds 25s infinite;
  margin-left:0;
}
.cloud:before{
  border-radius: 60%;
  box-shadow: 20px -20px 0 0 #464145,
          90px 0 0 0 #464145,
          60px -27px 0 8px #464145;
  content: "";
  position: absolute;
  width:60px;
  height:60px;
  left:-22px;
  bottom:0;
  background: #464145;
}

.cloud:nth-child(1){top:auto; bottom:250px; opacity: 0.85}
.cloud:nth-child(2){right:auto; left:300px; opacity: 0.5}
.cloud:nth-child(3){bottom:auto; top:350px; right:auto; left:150px; opacity: 0.75}
.cloud:nth-child(4){bottom:auto; top:100px; right:auto; left:220px; opacity: 0.65}

.moon{
  height:120px;
  width:120px;
  background: #949494;
  border-radius: 50%;
  box-shadow: 1px 1px 20px 9px #444444;
}
.moon:before{
  border-radius:60%;
  box-shadow:20px -50px 0 0 #444,
           50px 0 0 0 #444,
           50px -37px 0 10px #444;
  content: "";
  position: absolute;
  width: 20px;
  height: 20px;
  left:30px;
  bottom:10px;
  background: #444;
}
.cat{
  background:#EEEEEE;
  height:60px;
  top: auto;
  bottom: 200px;
  width:60px;
  z-index: 0;
  -webkit-transition: all linear 1s;
}
.cat:before, .cat:after{
  width:0;
  height: 0;
  top: -10px;
  position: absolute;
  content:"";
}

.cat:before{
  border-left: 0px solid transparent;
  border-right: 15px solid transparent;
  border-bottom: 15px solid #EEE;
  left:0;
}
.cat:after{
  border-right: 0px solid transparent;
  border-left: 15px solid transparent;
  border-bottom: 15px solid #EEE;
  right:0;
}

.cat .eyes{
  position: absolute;
  height: 8px;
  width:8px;
  background: #333;
  border-radius:100%;
  top: 15px;
}

.cat .eyes.left{left:12px;}
.cat .eyes.right{right:12px;}
.cat .mouth{
  position: absolute;
  height: 4px; width:60%;
  background: #333;
  border-radius: 0 0 30% 30%;
  top:28px;
  margin:auto;
  left:0; right:0;
}

.box:hover .cat{
  bottom: 300px;

}
@-webkit-keyframes clouds{
  0 {margin-left:0;}
  50% {margin-left:100px;}
  100% {margin-left:0;}
}

```





**Thank you for reading.** 

If you have any design idea or want to contact me for anything. Feel free to contact me via the contact form present in the contact page. Also don't forget to subscribe to my channel on Youtube.