---
title: Awesome Social media icon design
subtitle: " using HTML & CSS only and with Hover effect"
category:
  - HTML & CSS design
author: Harshit Kumar
date: 2020-06-14T16:56:07.530Z
featureImage: /uploads/social-media-icon-original.png
---
Hi everyone ,

In this tutorial, I made **Social Media Icon design** just by using **HTML** and **CSS** and with **Hover effect**.

The icons used in this video are  **fontawesome icons**.

![Awesome Social media icon design  using HTML & CSS only and with Hover effect](/uploads/social-media-icon-original.png "Awesome Social media icon design  using HTML & CSS only and with Hover effect")

<div class="embed-responsive embed-responsive-16by9 z-depth-1">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/Y5TR-Jkdzj0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> 
</div>





## Steps to use Fontawesome Icons

 For using any free **Fontawesome icons** follow the steps below :-

1. Create your accont in <https://fontawesome.com/> . If  you already have accont you  can skip this step.
2. After making the account, Go to your kits and config your kit.
3. Then you just need to copy the kit to your Head tag and thats it you are all done .

   Now you can start using the Fontawesome Icons for free.

I made this design using HTML and CSS only. So it won't be any difficult for any people to use this design in thier website.The icon also have nice hover animation too. if you want to change the color of the icon or the effect to match your website design. You can easily change that too. Just change the color in the CSS.

# Source Code

Following are the full HTML and CSS codes which I used in the Video.

**HTML**

```html
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <link rel="stylesheet" href="style.css">
    <script src="https://kit.fontawesome.com/c19c30a707.js" crossorigin="anonymous"></script>
    <title></title>
  </head>
  <body>
    <div class="social">
      <a class="button" href="#"><i class="fab fa-facebook-f"></i></a>
      <a class="button" href="#"><i class="fab fa-twitter"></i></a>
      <a class="button" href="#"><i class="fab fa-google"></i></a>
      <a class="button" href="#"><i class="fab fa-instagram"></i></a>
      <a class="button" href="#"><i class="fab fa-youtube"></i></a>

    </div>

  </body>
</html>
```

**CSS**

```css
body{
  padding: 0;
  margin: 0;
}
.social{
  position: absolute;
  top:50%;
  width:100%;
  text-align:center;
}
.button{
  display: inline-block;
  width: 90px;
  height: 90px;
  margin:10px;
  border-radius: 50px;
  color:#3498db;
  background: white;
  box-shadow: 20px 20px 60px #d9d9d9,
  -20px -20px 60px #ffffff;
  position: relative;
}

.button i{
  line-height: 90px;
  font-size:26px;
  transform: scale(1.5);
  transition: 0.25s;
}
.button:hover{
  transform:scale(1.1);
  color:#f1f1f1;
  background-color: #3498db;
  transition: 0.5s;
}
```

# Minified Source Code

This is minified CSS code which you can directly use in your website.

**Note**:- Make sure to copy and paste the minified HTML code in a div element.

**Minified HTML**

```
    <div class="social">
      <a class="button" href="#"><i class="fab fa-facebook-f"></i></a>
      <a class="button" href="#"><i class="fab fa-twitter"></i></a>
      <a class="button" href="#"><i class="fab fa-google"></i></a>
      <a class="button" href="#"><i class="fab fa-instagram"></i></a>
      <a class="button" href="#"><i class="fab fa-youtube"></i></a>
    </div>
```

**Minified CSS**

```
.social{
  position: absolute;
  text-align:center;
}
.button{
  display: inline-block;
  width: 90px;
  height: 90px;
  margin:10px;
  border-radius: 50px;
  color:#3498db;
  box-shadow: 20px 20px 60px #d9d9d9,
  -20px -20px 60px #ffffff;
}

.button i{
  line-height: 90px;
  font-size:26px;
  transform: scale(1.5);
  transition: 0.25s;
}
.button:hover{
  transform:scale(1.1);
  color:#f1f1f1;
  background-color: #3498db;
  transition: 0.5s;
}
```

**Note**:- If minified version doesn't work try and use the full version.

**Note:- This code is royalty/copyright free for personal as well as for non-profit use. Commercial use is not allowed.**