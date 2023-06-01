# How to Create Navbar that Responds to different Screen sizes
![The image isn't showing because you are offline](https://www.ixtlan.si/wp-content/uploads/2019/09/quattro_krka_1_shutterstock_421766797-2.jpg)
95% of websites are built with a navbar attached at the top which, looks good on different screen sizes. Navbar helps users to access information fast and easily. To make your website user-friendly and interactive; attach a navbar to the top of your website.

In this tutorial, you'll learn the following:
* What is a Navbar?
* How to create a navbar that responds to different screen sizes using:
  - Html
  - CSS
  - Media query
  - JavaScript

Learn [HTML](https://www.w3schools.com/html/), [CSS](https://www.w3schools.com/Css/), [Mediaqueries](https://www.w3schools.com/css/css3_mediaqueries.asp), and [JavaScript](https://www.w3schools.com/js/DEFAULT.asp); if you don't have the basic knowledge to continue this tutorial.
## What is a Navbar?
Before we dive deeper into this tutorial, what is a navbar?

![The image isn't showing because you are offline](2023-05-31-22-44-11.png)

A **Navbar** is the section of a web page interface that helps users to access information on a website easily. Navbars are implemented in the following user interfaces:
* operating system
* websites
* file browsers
* apps

### Steps to Create Navbar that Responds to Different Screen Sizes

Take the following steps to create a navbar that responds to different screen sizes:
1. Write your HTML code.
2. Add CSS to style your navbar.
3. Make your navbar responsive using media queries.
4. Make your navbar toggleable using JavaScript.

**Write Your HTML Code**

***Code***
```ruby
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>navbar</title>
    <!--external css file linked here-->
    <link rel="stylesheet" href="style.css">
    <!--font awesome url linked here to enable display font-icon-->
    <script src="https://kit.fontawesome.com/58b7424050.js" crossorigin="anonymous"></script>
</head>
<body>
    <div class="navbar">
        <label class="logo"><h1>Logo</h1></label>
        <nav>
            <ul id="menulist">
                <li><a href="#">Home</a></li>
                <li><a href="#">About</a></li>
                <li><a href="#">News</a></li>
                <li><a href="#">Contact</a></li>
            </ul>
        </nav>
        <label class="icon"><i class="fa fa-bars" onclick="togglemenu()"></i></label>
    </div>
</body>
</html>
```
***Result***

![image](2023-06-01-00-10-18.png)

**Add CSS to style your navbar**

***Code***
```ruby
*{
    margin: 0;
    padding: 0;
    font-family: Arial, Helvetica, sans-serif;
}
.navbar{
    width:100%;
    display: flex;
    align-items: center;
    background-color: #008000;
    z-index: 2;
}
.logo{
    font-size: 15px;
    font-weight: bolder;
    margin: 10px;
    color: #fff;
    cursor: pointer;
}
.icon{
    font-size: 20px;
    margin: 10px;
    color: #fff;
    cursor: pointer;
    display: none;
}
nav{
    text-align: right;
}
nav ul li{
    list-style-type: none;
    display: inline-block;
    margin: 10px 30px;
}
nav ul li a{
    text-decoration: none;
    color: #fff;
    font-size: 20px;
}
nav ul li a:hover{
    text-decoration: underline;
}
```
