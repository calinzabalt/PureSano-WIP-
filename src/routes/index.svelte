<script>
let bgImage = "header.jpg";
let delivery ="delivery.jpg";
let social ="social-media.jpg";
let contact ="contact.jpg";
import Lazy from 'svelte-lazy';
const onload = (node) => {
    console.log('on load');
  }
</script>

<style>
@font-face {
    font-family: 'SansPro';
    src: url(/SourceSansPro-Regular.ttf);
    font-style: normal;
  }
@font-face {
    font-family: 'Fira';
    src: url(/FiraSans-Bold.ttf);
    font-style: normal;
  }

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    outline: 0 none;
}

#header {
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
}
#header h1{
  font-family: Fira;
	text-align:center;
	color: #ffffff;
	font-size: 68px;
	padding: 400px;
}
section{
  margin-bottom: 80px;
}
#First_Section p{
  font-family: SansPro;
	text-align: center;
	max-width: 900px;
	margin-left: auto;
	margin-right: auto;
  font-size: 20px;
  line-height: 1.8;
}
#Second_Section .container{
	max-width: 1300px;
	margin-left: auto;
	margin-right: auto;
	letter-spacing: -7px;
}

#Second_Section .container .item{
	width: 50%;
	display: inline-block;
	text-align: center;
	letter-spacing: normal;
}

#Second_Section .container .item img{
	height: 600px;
  max-width: 100%;
}

#Second_Section .container .item img:hover{
box-sizing: border-box;
box-shadow: 0px 7px 45px rgba(0, 0, 0, 0.12);
}

#Four_Section{
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
}
#Four_Section h2{
	text-align:center;
	color: #ffffff;
	font-size: 48px;
	padding: 250px;
}


input[type="text"],
  textarea {
    width: 100%;
    padding: 12px;
    border: 1px solid #ccc;
    border-radius: 4px;
    box-sizing: border-box;
    margin-top: 6px;
    margin-bottom: 16px;
    resize: vertical;
  }
  input[type="submit"] {
    background-color: #4caf50;
    color: white;
    padding: 12px 20px;
    border: none;
    border-radius: 4px;
    cursor: pointer;
  }
  input[type="submit"]:hover {
    background-color: #45a049;
  }
#Third_Section .container {
    border-radius: 5px;
    max-width: 800px;
    margin-left: auto;
    margin-right: auto;
    padding: 20px;
	margin-top: 100px;
  }
#Fifth_Section .container{
  max-width: 1200px;
  letter-spacing: -7px;
  text-align: center;
  margin-left: auto;
  margin-right: auto;
}
#Fifth_Section .container .item{
  width: 50%;
  display: inline-block;
  letter-spacing: normal;
  position: relative;
}

#Fifth_Section img{
    max-width: 500px;
    height: 400px;
    border-radius: 21px;
    filter: blur(4px);
    -webkit-filter: blur(4px);  
    transition: all 0.5s ease;
}
#Fifth_Section img:hover{
  filter: blur(0px);
    -webkit-filter: blur(0px);  
}
#Fifth_Section .item_content{
  position: absolute;
  z-index: 99;
  top: 35%;
  left: 50%;
  transform: translateX(-50%);
}

#Fifth_Section .item_content h4{
  color: #fff;
}

button a:before{
  content: "" !important;
  position: absolute;
  background-image: url(/top.png);
  width: 32px;
  height: 32px;
  cursor: pointer;
  transform: rotate(270deg);
  top: 30px;
}

button a{
  position: absolute;
  transform: translateX(-50%);
  left: 49%;
  opacity: 0.5;
  transition: all 0.5s ease;
}
button a:hover{
  opacity: 1;
}
.footer {
  text-align: center;
  height: 150px;
  padding-top: 80px;
  background: #2D2D2D;

}
.footer ul li{
  list-style: none;
  color: #fff;
  background: #2D2D2D;
}
.footer ul li a{
   font-family: SansPro;
   font-size: 18px;
}

@media only screen and (max-width: 765px){
	#header h1{
		padding: 100px 10px 100px 10px;
		font-size: 38px;
	}
  #Second_Section .container .item{
    width: 100%;
    padding: 20px 0 20px 0;
  }
  #Second_Section .container .item img{
  box-sizing: border-box;
  box-shadow: 0px 7px 45px rgba(0, 0, 0, 0.12);
  width: 100%;
  }
  #First_Section p{
	font-size: 16px;
  padding: 0 20px 0 20px;
}
}

@media only screen and (max-width: 493px){
	#header h1{
		font-size: 28px;
	}
}
@keyframes fadeInUp {
    from {
        transform: translate3d(0,40px,0)
    }

    to {
        transform: translate3d(0,0,0);
        opacity: 1
    }
}

@-webkit-keyframes fadeInUp {
    from {
        transform: translate3d(0,40px,0)
    }

    to {
        transform: translate3d(0,0,0);
        opacity: 1
    }
}

.animated {
    animation-duration: 1s;
    animation-fill-mode: both;
    -webkit-animation-duration: 1s;
    -webkit-animation-fill-mode: both
}

.animatedFadeInUp {
    opacity: 0
}

.fadeInUp {
    opacity: 0;
    animation-name: fadeInUp;
    -webkit-animation-name: fadeInUp;
}

#Third_Section .container{
  letter-spacing: -7px;
  max-width: 900px;
  margin-left: auto;
  margin-right: auto;
  box-sizing: border-box;
}
form .row .item{
  width: 50%;
  display: inline-block;
  padding: 0 15px;
}
input[type="text"]{
  border-radius: 71px;
  line-height: 21px;
}

form .item_text{
  padding: 0 15px;
}

form textarea{
  border-radius: 21px;
}

#Third_Section h2{
  letter-spacing: normal;
  text-align: center;
  padding-bottom: 40px;
}

#Third_Section input[type="submit"]{
    background-color: #2D2D2D;
    background: #2D2D2D;
    padding: 15px 45px;
    color: #fff;
    font-family: SansPro;
    font-size: 16px;
    border-radius: 25px;
    display: inline-block;
    margin-left: 15px;
    transition: all 0.5s ease;
    border: 1px solid #2D2D2D;
}
#Third_Section input[type="submit"]:hover{
    background: #ffffff;
    color: #2D2D2D;
    border: 1px solid #2D2D2D;
}
#Third_Section input[type="text"]{
    padding-left: 20px;
    font-size: 16px;
    font-family: SansPro;
}
#Third_Section textarea{
  padding-left: 20px;
  font-size: 16px;
  font-family: SansPro;
}
#Fifth_Section h4{
  font-size: 28px;
  font-family: SansPro;
}
#Fifth_Section .item a span{
  content: "" !important;
  position: absolute;
  background-image: url(/facebook.png);
  width: 32px;
  height: 32px;
  cursor: pointer;
  top: 20px;
  display: inline-block;
}
#Fifth_Section .item a:nth-child(3) span{
  content: "" !important;
  position: absolute;
  background-image: url(/facebook.png);
  width: 44px;
  height: 44px;
  background-size: cover;
  cursor: pointer;
  top: 40px;
  left: 0px;
  display: inline-block;
}
#Fifth_Section .item a:nth-child(2) span{
  content: "" !important;
  position: absolute;
  background-image: url(/twitter.png);
  width: 44px;
  height: 44px;
  background-size: cover;
  cursor: pointer;
  top: 40px;
  left: 60px;
  display: inline-block;
}
#Fifth_Section .item a span{
  content: "" !important;
  position: absolute;
  background-image: url(/instagram.png);
  width: 44px;
  height: 44px;
  background-size: cover;
  cursor: pointer;
  top: 40px;
  left: 120px;
  display: inline-block;
}
#Four_Section h2{
    font-family: Fira;
    text-align: center;
    color: #ffffff;
    font-size: 48px;
}

</style>

<svelte:head>
	<title>PureSaneo</title>
</svelte:head>

<section id="header" style="background-image: url('{bgImage}')">
<h1 class="animated animatedFadeInUp fadeInUp">Wash your hands <br> and feel "safe"</h1>
</section>

<Lazy height={800} offset={150} onload={onload} fadeOption={{delay: 500, duration: 1000}}>
<section id="First_Section" class="animated animatedFadeInUp fadeInUp">
<p>Developed and manufactured by ARSAT,
a trusted and certified quality European aerospace factory
where safety and high quality are fundamentally
required by global brands as our clients, the Astreea®
pedal hand sanitizer is proudly following these standards.
Entirely made from medical stainless steel,
durable, weather resistant and fully mechanical,
Astreea® is the solution for heavy duty intense use.

Quality and value for money rarely meet.
The Astreea® hand sanitizer is one
of these exceptions.</p>
</section>
</Lazy>

<Lazy height={800} offset={150} onload={onload} fadeOption={{delay: 500, duration: 1000}}>
<section id="Second_Section">
<div class="container">
	<div class="item"><img alt="dispenser" src="1.jpeg"/></div>
	<div class="item"><img alt="dispenser" src="3.jpeg"/></div>
</div>
</section>
</Lazy>

<Lazy height={800} offset={150} onload={onload} fadeOption={{delay: 500, duration: 1000}}>
<section id="Third_Section">
<div class="container">
<form action="" method="POST">
  <h2>Contact Us:</h2>
  <div class="row">
    <div class="item">
      <input type="text" id="name" name="name" placeholder="Your name.." />
    </div>
    <div class="item">
      <input
        type="text"
        id="email"
        name="_replyto"
        placeholder="Email address.." />
    </div>  
  </div>
  <div class="row">
      <div class="item">
      <input type="text" id="name" name="name" placeholder="Phone number.." />
      </div>
      <div class="item">
      <input type="text" id="name" name="name" placeholder="Company name .." />  
      </div>
  </div>
  <div class="item_text">
    <textarea
      id="subject"
      name="subject"
      placeholder="Your message.."
      style="height:200px" />
  </div>
    <input type="submit" value="Submit" />
  </form>
  </div>
</section>
</Lazy>

<Lazy height={800} offset={150} onload={onload} fadeOption={{delay: 500, duration: 1000}}>
<section id="Four_Section" style="background-image: url('{delivery}')">
<h2>More Information / Delivery Methods / How is fabricated</h2>
</section>
<section id="Fifth_Section">
<div class="container">
	<div class="item"><img alt="dispenser" src="social-media.jpg"/>
    <div class="item_content">
      <h4>We are on Social Media:</h4>
      <a href="https://www.facebook.com/" target="blank"><span></span></a>
      <a href="https://www.facebook.com/" target="blank"><span></span></a>
      <a href="https://www.facebook.com/" target="blank"><span></span></a>
    </div>
  </div>

  <div class="item"><img alt="dispenser" src="contact.jpg"/>
    <div class="item_content">
      <h4>Call or chat with us live</h4>
        <h4>+40 0740 691 940</h4>
    </div>
  </div>

</div>  
</section>
</Lazy>
<button><a href="#header"><span></span></a></button>
<div class="footer">
<ul>
<li><a href="/">Terms & Condition</a></li>
<li><a href="/">Privacy Policy</a></li>
</ul>
</div>


