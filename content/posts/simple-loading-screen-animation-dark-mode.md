---
title: Simple Loading Screen animation (Dark Mode)
subtitle: using HTML & CSS only (responsive design)
category:
  - HTML & CSS design
author: Harshit Kumar
date: 2020-06-17T08:21:56.437Z
featureImage: /uploads/simple-loading-screen_.png
---


Hi Guys ,

Welcome back to my Blog. 

In this tutorial I made a  **simple Loading screen animation** using **HTML & CSS** only for our website.

Table of content

* Youtube Video link
* Features
* Source code

  * HTML
  * CSS

![Simple loading screen animation using HTML & CSS only ](/uploads/simple-loading-screen_.png "Simple loading screen animation using HTML & CSS only ")

#  Youtube Video

If you guys haven't seen my **youtube video** on this **design**, please give it a go

Link :- <https://youtu.be/UUwb-P_cH4k>



## Features of this design

1. Responsive Design :- The design will work on all kind of devices with different screen sizes always.
2.  Dark mode :- This design, as you see, is coded in black and white color so it can be used in Dark modes too.
3.  Fast loading and light weight:- Beacause of the minimal use of codes and no use of any kind of Javascript. This desgin is superfast to load and puts very less strain at the end user device.
4. Compatible :- Since the code use Webkit css. so it is cross compatible between all major browsers. 



# Source code

##### **HTML**

```html

<!DOCTYPE html>
<html lang="en" >
  <head>
    <meta charset="utf-8">
    <link rel="stylesheet" href="style.css">
    <title></title>
  </head>
  <body>
    <div class="loading-tile">
      <div class="tile"></div>
      <div class="tile"></div>
      <div class="tile"></div>
      <div class="tile"></div>
      <div class="tile"></div>
      <div class="tile"></div>
      <div class="tile"></div>
      <div class="tile"></div>
      <div class="tile"></div>
      <div class="tile"></div>
      <div class="tile"></div>
      <div class="tile"></div>
      <div class="tile"></div>
      <div class="tile"></div>
      <div class="tile"></div>
      <div class="tile"></div>
    </div>
  </body>
</html>
```

**CSS**

```
body{
  background: #000;
}
.loading-tile{
  position: absolute;
  width:80px;
  height:100px;
  left:50%;
  margin-left: -5px;
  top:50%;
  margin-top: -5px;
}
.tile{
  position: relative;
  float: left;
  width: 10px;
  height: 10px;
  margin: 0px 10px 10px 0px;
  border-radius: 5px;
  background: #fff;
}
.tile:nth-child(4n+1){
  -webkit-animation:wave 2.5s ease-in-out .0s infinite;
  animation: wave 2.5s ease-in-out .0s infinite;
}
.tile:nth-child(4n+2){
  -webkit-animation:wave 2.5s ease-in-out .2s infinite;
  animation: wave 2.5s ease-in-out .2s infinite;
}
.tile:nth-child(4n+3){
  -webkit-animation:wave 2.5s ease-in-out .4s infinite;
  animation: wave 2.5s ease-in-out .4s infinite;
}
.tile:nth-child(4n+4){
  -webkit-animation:wave 2.5s ease-in-out .6s infinite;
  animation: wave 2.5s ease-in-out .6s infinite;
  margin-right: 0;
}
@keyframes wave{
  0% {top:0; opacity:1;}
  50% {top:30px; opacity:.2;}
  100% {top:0; opacity:1;}

}
@-webkit-keyframes wave{
  0% {top:0; opacity:1;}
  50% {top:30px; opacity:.2;}
  100% {top:0; opacity:1;}
}
```





If you haven't **subscribe** to our **youtube channel**, then click here to subscribe 

https://www.youtube.com/channel/UCOyYK29kVXQvknRwdW_3-YQ