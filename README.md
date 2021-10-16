<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ENGINEERING MATERIALS</title>

    <!-- font awesome cdn link  -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css">

    <!-- custom css file link  -->
    <link rel="stylesheet" href="style.css">
<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@100;200;300;400&display=swap');

:root{
    --purple:#814096;
    --pink:#F83292;
    --gradient:linear-gradient(90deg, var(--purple), var(--pink));
}

*{
    font-family: 'Poppins', sans-serif;
    margin:0; padding:0;
    box-sizing: border-box;
    text-decoration: none;
    outline: none; border:none;
    text-transform: capitalize;
}

*::selection{
    background:var(--pink);
    color:#fff;
}

html{
    font-size: 62.5%;
    overflow-x: hidden;
}

body{
    background:#f9f9f9;
}

section{
    min-height: 100vh;
    padding:0 9%;
    padding-top: 7.5rem;
    padding-bottom: 2rem;
}

.btn{
    display: inline-block;
    margin-top: 1rem;
    padding:.8rem 3rem;
    border-radius: 5rem;
    background:var(--gradient);
    font-size: 1.7rem;
    color:#fff;
    cursor: pointer;
    box-shadow: 0 .5rem 1rem rgba(0,0,0,.1);
    transition: all .3s linear;
}

.btn:hover{
    transform: scale(1.1);
}


.btn1{
    display: inline-block;
    margin-top: 5rem;
    padding:.8rem 3rem;
    border-radius: 8rem;
    background:var(--gradient);
    font-size: 2.2rem;
    color:#fff;
    cursor: pointer;
    box-shadow: 0 .5rem 1rem rgba(0,0,0,.1);
    transition: all .3s linear;
}

.btn1:hover{
    transform: scale(1.1);
}

.heading{
    text-align: center;
    background:var(--gradient);
    color:transparent;
    -webkit-background-clip: text;
    background-clip: text;
    font-size: 4.5rem;
    text-transform: uppercase;
    padding:1rem;
}

header{
    position: fixed;
    top:0; left:0;
    width:100%;
    background:#fff;
    box-shadow: 0 .5rem 1rem rgba(0,0,0,.1);
    padding:2rem 9%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    z-index: 1000;
}

header .logo{
    font-size: 2rem;
    color:var(--purple);
}

header .logo span{
    color:var(--pink);
}

header .navbar a{
    font-size: 1.7rem;
    margin-left: 2rem;
    color:var(--purple);
}

header .navbar a:hover{
    color:var(--pink);
}

header input{
    display: none;
}

header label{
    font-size: 3rem;
    color:var(--purple);
    cursor: pointer;
    visibility: hidden;
    opacity: 0;
}

.home{
    display: flex;
    align-items: center;
    justify-content: center;
    background:url(../images/home-bg-img.png) no-repeat;
    background-size: cover;
    background-position: center;
}

.home .image img{
    width:40vw;
    animation: float 3s linear infinite;
}

@keyframes float{
    0%, 100%{
        transform: translateY(0rem);
    }
    50%{
        transform: translateY(-3.5rem);
    }
}

.home .content h3{
    font-size: 5.5rem;
    color:#333;
    text-transform: uppercase;
}

.home .content h3 span{
    color:var(--pink);
    text-transform: uppercase;
}

.home .content p{
    font-size: 1.7rem;
    color:#666;
    padding:1rem 0;
}

.features .box-container{
    display: flex;
    align-items: center;
    justify-content: center;
    flex-wrap: wrap;
}
.center
{
	display: block;
  margin-left: auto;
  margin-right: auto;
  width: 50%;
}
.features .box-container .box{
    flex:1 1 30rem;
    background:#fff;
    border-radius: .5rem;
    border:.1rem solid rgba(0,0,0,.2);
    box-shadow: 0 .5rem 1rem rgba(0,0,0,.1);
    margin:1.5rem;
    padding:3rem 2rem;
    border-radius: .5rem;
    text-align: center;
    transition: .2s linear;
}

.features .box-container .box img{
    height: 20rem;
}

.features .box-container .box h3{
    font-size: 2rem;
    color:#333;
    padding-top: 1rem;
}

.features .box-container .box p{
    font-size: 1.3rem;
    color:#666;
    padding: 1rem 0;
}

.about{
    background:url(../images/about-bg.png) no-repeat;
    background-size: cover;
    background-position: center;
    padding-bottom: 3rem;
}

.about .column{
    display: flex;
    align-items: center;
    justify-content: center;
    flex-wrap: wrap;
}

.about .column .image{
    flex:1 1 40rem;
}

.about .column .image img{
    width:100%;
}

.about .column .content{
    flex:1 1 40rem;
}

.about .column .content h3{
    font-size: 3rem;
    color:#666;
}

.about .column .content p{
    font-size: 1.5rem;
    color:#666;
    padding:1rem 0;
}

.about .column .content .buttons a:last-child{
    margin-left: 2rem;
}

.newsletter{
    text-align: center;
    padding:5rem 1rem;
    background:url(../images/subscribe-bg.png) no-repeat;
    background-size: cover;
    background-position: center;
}

.newsletter h3{
    color:#fff;
    font-size: 3rem;
    text-transform: uppercase;
}

.newsletter p{
    color:#fff;
    font-size: 1.6rem;
    margin:2rem auto;
    width:70rem;
}

.newsletter form{
    display: flex;
    max-width: 70rem;
    border:.2rem solid #fff;
    padding:.5rem;
    border-radius: 5rem;
    margin:2rem auto;
    height:5.5rem;
}

.newsletter form input[type="email"]{
    padding:0 2rem;
    font-size: 1.7rem;
    background:none;
    width:100%;
    color:#fff;
    text-transform: none;
    background:none;
}

.newsletter form input[type="email"]::placeholder{
    color:#eee;
    text-transform: capitalize;
}

.newsletter form input[type="submit"]{
    background:#fff;
    width:20rem;
    font-size: 1.7rem;
    border-radius: 5rem;
    cursor: pointer;
}

.newsletter form input[type="submit"]:hover{
    color:var(--pink);
}

.review .box-container{
    display: flex;
    align-items: center;
    justify-content: center;
    flex-wrap: wrap;
}

.review .box-container .box{
    background:#fff;
    margin:1rem;
    padding:1rem;
    text-align: center;
    position: relative;
    border:.1rem solid rgba(0,0,0,.2);
    box-shadow: 0 .5rem 1rem rgba(0,0,0,.1);
    flex:1 1 30rem;
    border-radius: .5rem;
}

.review .box-container .box .fa-quote-right{
    position: absolute;
    top:1rem; right:2rem;
    font-size: 8rem;
    color:var(--pink);
    opacity: .3;
}

.review .box-container .box .user img{
    border-radius: 50%;
    object-fit: cover;
    height: 7rem;
    width:7rem;
    margin-top: 2rem;
}

.review .box-container .box .user h3{
    color:var(--pink);
    font-size: 2rem;
}

.review .box-container .box .user .stars i{
    color:var(--purple);
    font-size: 1.5rem;
    padding:1rem 0;
}

.review .box-container .box .comment{
    color:#666;
    font-size: 1.4rem;
    padding:1rem;
}

.pricing .box-container{
    display: flex;
    align-items: center;
    justify-content: center;
    flex-wrap: wrap;
}

.pricing .box-container .box{
    flex:1 1 27rem;
    margin:1rem;
    padding:1rem;
    background:#fff;
    border:.1rem solid rgba(0,0,0,.2);
    box-shadow: 0 .5rem 1rem rgba(0,0,0,.1);
    border-radius: .5rem;
    text-align: center;
    padding-bottom: 3rem;
}

.pricing .box-container .box:nth-child(2),
.pricing .box-container .box:hover{
    border:.2rem solid var(--pink);
}

.pricing .box-container .box .title{
    color:var(--purple);
    font-size: 2.5rem;
    padding-top: 1rem;
}

.pricing .box-container .box .price{
    font-size: 4rem;
    color:var(--pink);
    padding:1rem 0;
}

.pricing .box-container .box .price span{
    font-size: 2rem;
}

.pricing .box-container .box ul{
    padding:1rem 0;
    list-style: none;
}

.pricing .box-container .box ul li{
    font-size: 1.7rem;
    color:#666;
    padding:.5rem 0;
}

.pricing .box-container .box ul li .fa-check{
    color:lightgreen;
}

.pricing .box-container .box ul li .fa-times{
    color:tomato;
}

.contact{
    display: flex;
    align-items: center;
    justify-content: center;
    flex-wrap: wrap;
    padding-bottom: 4rem;
}

.contact .image{
    flex:1 1 40rem;
}

.contact .image img{
    width:100%;
    padding:2rem;
}

.contact form{
    flex:1 1 40rem;
    padding:2rem 3rem;
    border:.1rem solid rgba(0,0,0,.2);
    box-shadow: 0 .5rem 1rem rgba(0,0,0,.1);
    border-radius: .5rem;
    background:#fff;
}

.contact form .heading{
    text-align: left;
    padding:0;
    padding-bottom: 2rem;
}

.contact form .inputBox{
    position: relative;
}

.contact form .inputBox input, .contact form .inputBox textarea{
    width:100%;
    background:none;
    color:#666;
    margin:1.5rem 0;
    padding:.5rem 0;
    font-size: 1.7rem;
    border-bottom: .1rem solid rgba(0,0,0,.1);
    text-transform: none;
}

.contact form .inputBox textarea{
    resize: none;
    height: 13rem;
}

.contact form .inputBox label{
    position: absolute;
    top:1.7rem; left:0;
    font-size: 1.7rem;
    color:#666;
    transition: .2s linear;
}

.contact form .inputBox input:focus ~ label,
.contact form .inputBox input:valid ~ label,
.contact form .inputBox textarea:focus ~ label,
.contact form .inputBox textarea:valid ~ label{
    top:-.5rem;
    font-size: 1.5rem;
    color:var(--pink);
}

.footer{
    padding-top: 3rem;
    background:url(../images/footer-bg.png) no-repeat;
    background-size: cover;
    background-position: center;
}

.footer .box-container{
    display: flex;
    flex-wrap: wrap;
}

.footer .box-container .box{
    flex:1 1 25rem;
    margin:2rem;
}

.footer .box-container .box h3{
    font-size: 2.5rem;
    padding:1rem 0;
    color:#fff;
    text-decoration: underline;
    text-underline-offset: 1rem;
}

.footer .box-container .box p{
    font-size: 1.5rem;
    padding:.5rem 0;
    color:#eee;
}

.footer .box-container .box a{
    display: block;
    font-size: 1.5rem;
    padding:.5rem 0;
    color:#eee;
}

.footer .box-container .box a:hover{
    text-decoration: underline;
}

.footer .box-container .box .info{
    display: flex;
    align-items: center;
}

.footer .box-container .box .info i{
    margin:.5rem 0;
    margin-right: 1rem;
    border-radius: 50%;
    background:#fff;
    color:var(--pink);
    font-size: 1.5rem;
    height:4.5rem;
    width:4.5rem;
    line-height: 4.5rem;
    text-align: center;
}

.footer .credit{
    font-size: 2rem;
    font-weight: normal;
    letter-spacing: .1rem;
    color:#fff;
    border-top: .1rem solid #fff5;
    padding:2.5rem 1rem;
    text-align: center;
}














/* media queries  */

@media (max-width:1200px){
    
    html{
        font-size: 55%;
    }

}

@media (max-width:991px){
    
    section{
        padding:0 3%;
        padding-top: 7.5rem;
        padding-bottom: 2rem;
    }

}

@media (max-width:768px){

    header label{
        visibility: visible;
        opacity: 1;
    }

    header .navbar{
        position: absolute;
        top:100%; left: 0;
        width:100%;
        background:#fff;
        padding:1rem 2rem;
        border-top: .1rem solid rgba(0,0,0,.2);
        box-shadow: 0 .5rem 1rem rgba(0,0,0,.1);
        transform-origin: top;
        transform: scaleY(0);
        opacity: 0;
        transition: .2s linear;
    }

    header .navbar a{
        display: block;
        margin:2rem 0;
        font-size: 2rem;
    }

    header input:checked ~ .navbar{
        transform: scaleY(1);
        opacity: 1;
    }

    header input:checked ~ label::before{
        content:'\f00d';
    }

    .home{
        flex-flow: column-reverse;
    }

    .home .image img{
        width:100%;
    }

    .home .content h3{
        font-size: 3.6rem;
    }

    .home .content p{
        font-size: 1.5rem;
    }

    .about{
        background-position: right;
    }

    .newsletter p{
        width:auto;
    }

}

@media (max-width:450px){
    
    html{
        font-size: 50%;
    }

    .about .column .content .buttons a{
        width:100%;
        text-align: center;
    }

    .about .column .content .buttons a:last-child{
        margin: 1rem 0;
    }

}
</style>
</head>
<body>
    
<!-- header section starts  -->

<header>

    <a href="#self" class="logo"><span>Engineering</span>Materials</a>

    <input type="checkbox" id="menu-bar">
    <label for="menu-bar" class="fas fa-bars"></label>

    <nav class="navbar">
        <a href="#home">home</a>
        <a href="#features">features</a>
        <a href="#about">about</a>
		 <a href="#supporters">Supporters</a>
        <a href="#team">Team</a>
        <a href="#contact">contact</a>
    </nav>

</header>

<!-- header section ends -->

<!-- home section starts  -->

<section class="home" id="home">

    <div class="content">
        <h3>WELCOME TO <span>ENGINEERING MATERIALS</span></h3>
        <p>Nice to Meet u Guys!!!!!</br>
Here You Can Download the All Study Materials of your Branches According to the JNTU Anantapur Syllabus</br>
<b>"DESIGNED AND DEVELOPED BY SVCK STUDENTS"</b></p>
        <a href="#features" class="btn">Scroll For More</a>
    </div>

    <div class="image">
        <img src="home-img.jpg">
    </div>

</section>

<!-- home section ends -->

<!-- features section starts  -->

<section class="features" id="features">

    <h1 class="heading"> SITE FEATURES </h1>

    <div class="box-container">

        <div class="box">
            <img src="images/f-icon1.png" alt="">
            <h2 class="btn">Materials For All Regulations</h2>
            <h3>Here Students Can Get All Regulations Materials For the Respective Branches</h3>
        </div>

        <div class="box">
            <img src="images/f-icon2.png" alt="">
            <h2 class="btn">Online Compilers</h2>
            <h3>Students Can Get the Online Compilers for Coding In the Mobile Also</h3>
        </div>

        <div class="box">
            <img src="images/f-icon3.png" alt="">
            <h2 class="btn">Programming Softwares</h2>
            <h3>Students Can Get the All Programming Softwares for Download and Coding in a Desktop</h3>
        </div>

    </div>

</section>

<!-- features section ends -->

<!-- about section starts  -->

<section class="about" id="about">

    <h1 class="heading"> SELECT YOUT BANCH HERE</h1>

    <div class="column">

        <div class="image">
            <img src="dept.jpg" alt="">
        </div>

        <div class="content">
            <h3>SELECT YOUR BRANCH BELOW</h3>
             <div class="buttons">
                <a href="https://websiteengineering.wixsite.com/mysite" class="btn1"> COMPUTER SCIENCE & ENGINEERING <br>[ CSE ]</a>
                <a href="https://editorengineeringm.wixsite.com/r19ece" class="btn1">  ELECTRONICS & COMMUNICATION ENGINEERING [ ECE ] </a>
				<a href="https://editoraiml.wixsite.com/aiml" class="btn1"> ARTIFICIAL INTELLEGENCE & MACHINE LEARNING [ AIML ] </a>
            </div>
        </div>

    </div>

</section>

<!-- about section ends -->

<section class="review" id="supporters">

    <h1 class="heading"> ABOUT SUPPORTERS</h1>

    <hr color="red">
                       <img src="unnamed (1).jpg"  class="center">
 <div class="box-container">

        <div class="box">
           <img src="hod_h&s.jpg">
        </div>

        <div class="box">
                       <img src="hod_cse.jpg">

        </div>

        <div class="box">
                       <img src="hod_ece.jpg">

        </div>
		<div class="box">
                       <img src="DILIP_SIR.jpg">

        </div>
</div>
        

</section>
<hr color="red">
<!-- review section starts  -->

<section class="review" id="team">

    <h1 class="heading"> ABOUT ENGINEERING MATERIALS TEAM </h1>

    <div class="box-container">

        <div class="box">
           <img src="1.jpg">
        </div>

        <div class="box">
                       <img src="2.jpg">

        </div>

        <div class="box">
                       <img src="3.jpg">

        </div>

    </div>

</section>

<!-- review section ends -->


<!-- contact section starts  -->

<section class="contact" id="contact">

    <div class="image">
        <img src="about-img.jpg" alt="">
    </div>

    <form action="">

        <h1 class="heading">contact us</h1>

        <div class="inputBox">
            <input type="text" required>
            <label>name</label>
        </div>

        <div class="inputBox">
            <input type="email" required>
            <label>email</label>
        </div>

        <div class="inputBox">
            <input type="number" required>
            <label>phone</label>
        </div>

        <div class="inputBox">
            <textarea required name="" id="" cols="30" rows="10"></textarea>
            <label>message</label>
        </div>

        <input type="submit" class="btn" value="send message">

    </form>

</section>

<!-- contact section edns -->

<!-- footer section starts  -->

<div class="footer">

    <div class="box-container">

        <div class="box">
            <h3>about us</h3>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Amet pariatur rerum consectetur architecto ad tempora blanditiis quo aliquid inventore a.</p>
        </div>

        <div class="box">
            <h3>quick links</h3>
            <a href="#">home</a>
            <a href="#">features</a>
            <a href="#">about</a>
            <a href="#">review</a>
            <a href="#">pricing</a>
            <a href="#">contact</a>
        </div>

        <div class="box">
            <h3>follow us</h3>
            <a href="#">facebook</a>
            <a href="#">instagram</a>
            <a href="#">pinterest</a>
            <a href="#">twitter</a>
        </div>

        <div class="box">
            <h3>contact info</h3>
            <div class="info">
                <i class="fas fa-phone"></i>
                <p> +123-456-7890 <br> +111-2222-333 </p>
            </div>
            <div class="info">
                <i class="fas fa-envelope"></i>
                <p> example@gmail.com <br> example@gmail.com </p>
            </div>
            <div class="info">
                <i class="fas fa-map-marker-alt"></i>
                <p> mumbai, india - 400104 </p>
            </div>
        </div>

    </div>

    <h1 class="credit"> &copy; copyright @ 2021 by mr. web designer </h1>

</div>

<!-- footer section ends -->




















</body>
</html>
