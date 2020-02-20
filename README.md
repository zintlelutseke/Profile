<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
body, html {
  height: 100%;
  margin: 0;
  font-family: Arial, Helvetica, sans-serif;}

.tablink {
  
background-size: -20%;

  color: black;
  float: left;
  border: none;
  outline: none;
  cursor: pointer;
  padding: 14px 16px; 
  width: 25%;
}

.tablink:hover {
  background-color:#C1CDCD;
}

/* Style the tab content */
.tabcontent {
  color: black;
  display: none;
  padding: 100px;
  text-align: center;
}

#Profile {background-image: url(coffee.jpg);}
#About  {background-image: url(coffee.jpg);}


.card {
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
  max-width: 300px;
  margin: auto;
  text-align: center;
  font-family: arial;
}

.occupation {
  color: grey;
  font-size: 22px;
}

.card button {
  border: none;
  outline: 0;
  padding: 12px;
  color: white;
  background-color: #000;
  text-align: center;
  cursor: pointer;
  width: 100%;
  font-size: 18px;
}

.card button:hover {
  opacity: 0.7;
}
.block {
  display: block;
  width: 100%;
  border: none;
  background-color: grey;
  color: white;
  padding: 14px 28px;
  font-size: 16px;
  cursor: pointer;
  text-align: center;
}

.block:hover {
  background-color: #ddd;
  color: black;
}

</style>

</head>
<body>


<div class="container">
<div id="Profile" class="tabcontent">
  <h1>Profile</h1>
  <p>This is a short summary of who I am</p>
</div>

<div id="About" class="tabcontent">
  <h1>About Me</h1>
 
</div>



<button class="tablink" onclick="openProduct('Profile', this, 'lightgrey')" id="defaultOpen">Profile</button>
<button class="tablink" onclick="openProduct('About', this, 'lightgrey')">About Me</button>

</div>
<script>
function openProduct(productName,elmnt,image) {
  var i, tabcontent, tablinks;
  tabcontent = document.getElementsByClassName("tabcontent");
  for (i = 0; i < tabcontent.length; i++) {
    tabcontent[i].style.display = "none";
  }
  tablinks = document.getElementsByClassName("tablink");
  for (i = 0; i < tablinks.length; i++) {
    tablinks[i].style.backgroundImage = "";
  }
  document.getElementById(productName).style.display = "block";
  elmnt.style.backgroundImage = image;

}
// Get the element with id="defaultOpen" and click on it
document.getElementById("defaultOpen").click();
</script>

 <div class="card">
  <img src="zee1.jpg" alt="Profile" style="width:100%">
  <h1>Zintle Lutseke</h1>
  <p class="Occupation">Graduate Trainee</p>
  <p>Zintle is a graduate trainee at Britehouse in Johannesburg. She studied Information Systems at the University of Cape Town.</p>
  <p><button>View profile</button></p>

  </div>

</body>


<style>
body, html {
  height: 100%;
  margin: 0;
  font-family: Arial, Helvetica, sans-serif;
}

.hero-image {
  background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url("high1.jpg");
  height: 100%;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;
}

.hero-text {
  text-align: center;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  color: white;
}

.block {
  display: block;
  width: 100%;
  border: none;
  background-color: white;
  color: lilac;
  padding: 14px 28px;
  font-size: 16px;
  cursor: pointer;
  text-align: center;
}

.block:hover {
  background-color: #ddd;
  color: black;
}

</style>
</head>
<body>

<div class="hero-image">
  <div class="hero-text">
    <h1 style="font-size:50px">ABOUT ME</h1>
    <h3 style="text-align:left;">Achievements:</h3>
	<p> I have a range of achievements in my life ranging from academic to social<br>

           <br> Represented the Eastern Cape Province in netbal</br>
           <br> Awarded Academic colours and Cum Laude in High school for my senior years</br>
           <br> Was part of the book room and stationery shop committees in high school</br>
           <br> A part of the Xhosa society choir in high school</br>
           <br> A residence senior mentor in University </br>
           <br> An O-week committee member in University </br>
           <br> A class representative for the final year class in University </br>
           

        </p>
	
  </div>
</div>


<style>
* {box-sizing: border-box}
body {font-family: Verdana, sans-serif; margin:0}
.mySlides {display: none}
img {vertical-align: middle;}

/* Slideshow container */
.slideshow-container {
  max-width: 1000px;
  position: relative;
  margin: auto;
}

/* Next & previous buttons */
.prev, .next {
  cursor: pointer;
  position: absolute;
  top: 50%;
  width: auto;
  padding: 16px;
  margin-top: -22px;
  color: black;
  font-weight: bold;
  font-size: 18px;
  transition: 0.6s ease;
  border-radius: 0 3px 3px 0;
  user-select: none;
}

/* Position the "next button" to the right */
.next {
  right: 0;
  border-radius: 3px 0 0 3px;
}

/* On hover, add a black background color with a little bit see-through */
.prev:hover, .next:hover {
  background-color: rgba(0,0,0,0.8);
}

/* Caption text */
.text {
  color:white;
  font-size: 15px;
  padding: 8px 12px;
  position: absolute;
  bottom: 8px;
  width: 100%;
  text-align: center;
}

/* Number text (1/3 etc) */
.numbertext {
  color: white;
  font-size: 12px;
  padding: 8px 12px;
  position: absolute;
  top: 0;
}

/* The dots/bullets/indicators */
.dot {
  cursor: pointer;
  height: 15px;
  width: 15px;
  margin: 0 2px;
  background-color: #bbb;
  border-radius: 50%;
  display: inline-block;
  transition: background-color 0.6s ease;
}

.active, .dot:hover {
  background-color: #717171;
}

/* Fading animation */
.fade {
  -webkit-animation-name: fade;
  -webkit-animation-duration: 1.5s;
  animation-name: fade;
  animation-duration: 1.5s;
}

@-webkit-keyframes fade {
  from {opacity: .4} 
  to {opacity: 1}
}

@keyframes fade {
  from {opacity: .4} 
  to {opacity: 1}
}

/* On smaller screens, decrease text size */
@media only screen and (max-width: 300px) {
  .prev, .next,.text {font-size: 11px}
}

.block {
  display: block;
  width: 100%;
  border: none;
  background-color: grey;
  color: white;
  padding: 14px 28px;
  font-size: 16px;
  cursor: pointer;
  text-align: center;
}

.block:hover {
  background-color: #ddd;
  color: black;
}
</style>
</head>
<body>

<h1><div style="text-align:center";> My Educational Background</div></h2>
<div class="slideshow-container">

<div class="mySlides fade">
  <div class="numbertext">1 / 3</div>
  <img src="primary.jpg" style="width:100%">
  <div class="text"><div style="text-align:center-top;">Primary school: I attended Balmoral Girls' Primary School from grade 1-7.</div></div>
</div>

<div class="mySlides fade">
  <div class="numbertext">2 / 3</div>
  <img src="high2.jpg" style="width:100%">
  <div class="text"><div style="text-align:center;">High school: I attended Queenstown Girls' High School from grade 8-12.</div></div>
</div>

<div class="mySlides fade">
  <div class="numbertext">3 / 3</div>
  <img src="varsity.jpg" style="width:100%">
  <div class="text"><div style="text-align:center;">University: I went to The University of Cape Town where I graduated with a Bachelor of Commerce Degree in Information Systems.</div></div>
</div>

<a class="prev" onclick="plusSlides(-1)">&#10094;</a>
<a class="next" onclick="plusSlides(1)">&#10095;</a>

</div>
<br>

<div style="text-align:center">
  <span class="dot" onclick="currentSlide(1)"></span> 
  <span class="dot" onclick="currentSlide(2)"></span> 
  <span class="dot" onclick="currentSlide(3)"></span> 
</div>


<script>
var slideIndex = 1;
showSlides(slideIndex);

function plusSlides(n) {
  showSlides(slideIndex += n);
}

function currentSlide(n) {
  showSlides(slideIndex = n);
}

function showSlides(n) {
  var i;
  var slides = document.getElementsByClassName("mySlides");
  var dots = document.getElementsByClassName("dot");
  if (n > slides.length) {slideIndex = 1}    
  if (n < 1) {slideIndex = slides.length}
  for (i = 0; i < slides.length; i++) {
      slides[i].style.display = "none";  
  }
  for (i = 0; i < dots.length; i++) {
      dots[i].className = dots[i].className.replace(" active", "");
  }
  slides[slideIndex-1].style.display = "block";  
  dots[slideIndex-1].className += " active";
}
</script>

</body>
</html> 

