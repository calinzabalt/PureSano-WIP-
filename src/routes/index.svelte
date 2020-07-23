<script>
let bgImage = "header.jpg";
let delivery ="delivery.png";
let social ="social-media.jpg";
let contact ="contact.jpg";
import Lazy from 'svelte-lazy';
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
	padding: 400px;
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
}

#Fifth_Section .item_content{
  position: absolute;
  z-index: 99;
  top: 50%;
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
  width: 64px;
  height: 64px;
  cursor: pointer;
  transform: rotate(270deg);
  opacity: 0.7;
  top: 20px;
}
button a{
  position: absolute;
  transform: translateX(50%);
  left: 49%;
}

.footer {
  text-align: center;
  height: 80px;
  padding-top: 80px;
  background: #171717;
}
.footer ul li{
  list-style: none;
  color: #fff;
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

</style>

<svelte:head>
	<title>PureSaneo</title>
</svelte:head>

<section id="header" style="background-image: url('{bgImage}')">
<h1 class="animated animatedFadeInUp fadeInUp">Wash your hands <br> and feel "safe"</h1>
</section>

<Lazy height={300} offset={150}>
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

<Lazy height={300} offset={150}>
<section id="Second_Section">
<div class="container">
	<div class="item"><img alt="dispenser" src="1.jpeg"/></div>
	<div class="item"><img alt="dispenser" src="3.jpeg"/></div>
</div>
</section>
</Lazy>

<section id="Third_Section">
<div class="container">
<form action="" method="POST">
    <label for="fname">Name</label>
    <input type="text" id="name" name="name" placeholder="Your name.." />

    <label for="lname">Email</label>
    <input
      type="text"
      id="email"
      name="_replyto"
      placeholder="Email address.." />

	<label for="fname">Phone number</label>
    <input type="text" id="name" name="name" placeholder="Phone number.." />

	<label for="fname">Company or Organization</label>
    <input type="text" id="name" name="name" placeholder="Company name .." />  

    <label for="subject">Message:</label>
    <textarea
      id="subject"
      name="subject"
      placeholder="Your message.."
      style="height:200px" />

    <input type="submit" value="Submit" />
  </form>
  </div>
</section>
<br/>
<section id="Four_Section" style="background-image: url('{delivery}')">
<h2>More Information / Delivery Methods / How is fabricated</h2>
</section>
<section id="Fifth_Section">
<div class="container">
	<div class="item"><img alt="dispenser" src="social-media.jpg"/>
    <div class="item_content">
      <h4>We are on Social Media:</h4>
      <span><p>Facebook</p></span>
      <span><p>Instagram</p></span>
      <span><p>Linkedin</p></span>
    </div>
  </div>

  <div class="item"><img alt="dispenser" src="contact.jpg"/>
    <div class="item_content">
      <h4>Call or chat with us live</h4>
      <span><p>04 0740 691 940</p></span>
      <span><p>Chat Icon</p></span>
    </div>
  </div>

</div>  
</section>
<button><a href="#header"><span></span></a></button>
<div class="footer">
<ul>
<li><a href="/">Terms & Condition</a></li>
<li><a href="/">Privacy Policy</a></li>
</ul>
</div>


