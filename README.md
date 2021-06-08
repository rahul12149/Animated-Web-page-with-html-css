# Animated-Web-page-with-html-css
This is My Animated web page with html/css
<!doctype html>
<html>
<head>
<title>Running car Animation-Easy Tutorials</title> 
       <link rel="stylesheet" type="text/css" href="css/style.css">
    
    
</head>
    <body>
    <div class="hero">
        <div class="highway"></div>
        <div class="city"></div>
        <div class="car">
            <img src="car.png">
    
        </div>
    
    </body>



</html>

  
  
  
  
  
  
  
  .....................................
  
  
  
  *{
    margin: 0;
    padding: 0;
    
}
.hero
{
    height: 100vh;
    width: 100%;
    background-image: url('../image/sky.jpg');
    background-size: cover;
    background-position: center;
    position: relative;
    overflow-x: hidden;
    
}
.highway
{
    height: 200px;
    width: 500%;
    display: block;
    background-image: url('../image/road.jpg');
    position: absolute;
    bottom: 0;
    left: 0;
    right: 0;
    z-index: 1;
    background-repeat: repeat-x;
    animation: highway 5s linear infinite;
    
    
}
@keyframes highway
{
    100%{
        transform: translateX(-3400px);
    }
}
.city
{
height: 250px;
width: 500%;
background-image: url('../image/city.png');
    position: absolute;
    bottom: 200px;
    left: 0;
    right: 0;
    display: block;
    z-index: 1;
    background-repeat: repeat-x;
    animation: city 20s linear infinite;
}
@keyframes city
{
    100%{
        transform: translateX(-1400px)
    }
}
.car
{
    width: 400px;
    left: 50%;
    bottom: 100px;
    transform: translateX(-50%);
    position: absolute;
    z-index: 2;
}
.car img
{
    width: 100%;
  
}
    
