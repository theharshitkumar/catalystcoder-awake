---
title: Hamburger Menu V2
subtitle: "in HTML & CSS only "
category:
  - HTML & CSS design
author: Harshit Kumar
date: 2020-06-29T21:02:10.715Z
featureImage: /uploads/hamburger-menu-v2.png
---
Hi Guys!!

Welcome back to my Blog of **Catalyst Coder.**

Are you one of them who always wanted to create a **Hamburger Menu** or a **Nav/Navigation Bar** just by using **HTML and CSS only** and wanted to use it in your website just easily by just copy and pasting the HTML and CSS code. Well then this blog post is just for you. Comment down below and tell me how much u you liked this video on a scale of 1 to 10. Also if you want any specific design, do comment and tell me. I regularly read the comments and who knows, my next video will be on your idea :)

So, today we are gonna make a Hamburger menu just by using HTML & CSS.

If you are new and wanna watch my youtube video on this topic ( I always leave some explanation text in between the video, so make sure you watch the full video), Hit the link below or if you are comming form the Youtube to get the source code . Well in that case scroll below.

![Hamburger Menu V2 in HTML & CSS only ](/uploads/hamburger-menu-v2.png "Hamburger Menu V2 in HTML & CSS only ")

# **Youtube Link**

If you are new here, Please go to my channel on Youtube and hit that like and subscribe button and also watch the whole video (the **music is lit** though) - [](https://youtu.be/FDovd3izofo)<https://youtu.be/SL5tStHBREY>

# **Source Code**

**HTML**

```html
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title>Hamburger menu design</title>
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
  </head>
  <body>
<nav class="menu">
  <input type="checkbox" href="#" class="menu-open" name="menu-open" id="menu-open"/>
  <label class="menu-open-button" for="menu-open">
  <i class= "fa fa-bars"></i>
</label>
<a href="#" class="menu-item"><i class="fa fa-phone"></i></a>
<a href="#" class="menu-item"><i class="fa fa-info-circle"></i></a>
<a href="#" class="menu-item"><i class="fa fa-sign-in"></i></a>
<a href="#" class="menu-item"><i class="fa fa-envelope"></i></a>
<a href="#" class="menu-item"><i class="fa fa-users"></i></a>
<a href="#" class="menu-item"><i class="fa fa-home"></i></a>
</nav>
<svg xmlns="http://www.w3.org/2000/svg" version="1.1">
    <defs>
      <filter id="shadowed-goo">
          <feGaussianBlur in="SourceGraphic" result="blur" stdDeviation="10" />
          <feColorMatrix in="blur" mode="matrix" values="1 0 0 0 0  0 1 0 0 0  0 0 1 0 0  0 0 0 18 -7" result="goo" />
          <feGaussianBlur in="goo" stdDeviation="3" result="shadow" />
          <feColorMatrix in="shadow" mode="matrix" values="0 0 0 0 0  0 0 0 0 0  0 0 0 0 0  0 0 0 1 -0.2" result="shadow" />
          <feOffset in="shadow" dx="1" dy="1" result="shadow" />
          <feComposite in2="shadow" in="goo" result="goo" />
          <feComposite in2="goo" in="SourceGraphic" result="mix" />
      </filter>
      <filter id="goo">
          <feGaussianBlur in="SourceGraphic" result="blur" stdDeviation="10" />
          <feColorMatrix in="blur" mode="matrix" values="1 0 0 0 0  0 1 0 0 0  0 0 1 0 0  0 0 0 18 -7" result="goo" />
          <feComposite in2="goo" in="SourceGraphic" result="mix" />
      </filter>
    </defs>
</svg>
</body>
</html>

```

**CSS**

```css
body{  background:#005999; }
.menu{
  -webkit-filter:url("#goo");
  top:30%;
}
.menu-item, .menu-open-button{
  background: #06bd8a;
  border-radius: 100%;
  width:80px;
  height:80px;
  margin-left:-40px;
  position: absolute;
  top:50px;
  color:white;
  text-align: center;
  line-height:80px;
  -webkit-transform:translate3d(0,0,0);
  -webkit-transition:-webkit-transform ease-out 200ms;
}
.menu-open{ display: none; }
.menu{
  position: absolute;
  left:50%;
  margin-left:-190px;
  padding-top:20px;
  padding-left:190px;
  width:380px;
  height:250px;
  box-sizing:border-box;
  font-size: 20px;
  text-align: left;
}
.menu-item:hover{
  background:white;
  color: #e91e63;
}
.menu-item:nth-child(3){
  -webkit-transition-duration:180ms;
}
.menu-item:nth-child(4){
  -webkit-transition-duration:180ms;
}
.menu-item:nth-child(5){
  -webkit-transition-duration:180ms;
}
.menu-item:nth-child(6){
  -webkit-transition-duration:180ms;
}
.menu-item:nth-child(7){
  -webkit-transition-duration:180ms;
}
.menu-item:nth-child(8){
  -webkit-transition-duration:180ms;
}
.menu-item:nth-child(9){
  -webkit-transition-duration:180ms;
}
.menu-open-button{
  z-index:2;
  -webkit-transition-timing-function:cubic-bezier(0.1,0.8,0.3,1.2);
  -webkit-transition-duration:400ms;
  -webkit-transform:scale(1.1,1.1) translate3d(0,0,0);
  cursor:pointer;
}
.menu-open-button:hover{
  -webkit-transform:scale(1.2,1.2)translate3d(0,0,0);
}
.menu-open:checked+ .menu-open-button{
  -webkit-transition-timing-function:linear;
  -webkit-transition-duration:200ms;
  -webkit-transform:scale(0.8,0.8) translate3d(0,0,0);
}
.menu-open:checked~.menu-item{
  -webkit-transition-timing-function:cubic-bezier(0.9,0,0.3,1.3);
}
.menu-open:checked~.menu-item:nth-child(3){
  -webkit-transition-duration:380ms;
  -webkit-transform:translate3d(0.08px,-104.9px,0);
}
.menu-open:checked~.menu-item:nth-child(4){
  -webkit-transition-duration:480ms;
  -webkit-transform:translate3d(90.9px,-52.6px,0);
}
.menu-open:checked~.menu-item:nth-child(5){
  -webkit-transition-duration:580ms;
  -webkit-transform:translate3d(90.9px,52.6px,0);
}
.menu-open:checked~.menu-item:nth-child(6){
  -webkit-transition-duration:680ms;
  -webkit-transform:translate3d(0.08px,104.9px,0);
}
.menu-open:checked~.menu-item:nth-child(7){
  -webkit-transition-duration:780ms;
  -webkit-transform:translate3d(-90.8px,52.6px,0);
}
.menu-open:checked~.menu-item:nth-child(8){
  -webkit-transition-duration:880ms;
  -webkit-transform:translate3d(-91.03px,-52.3px,0);
}
.menu-open:checked~.menu-item:nth-child(9){
  -webkit-transition-duration:980ms;
  -webkit-transform:translate3d(-0.25px,-104.9px,0);
}

```



Note this awsome design **doesn’t require any Javascript files**. So you can easily copy and paste the code in your website.