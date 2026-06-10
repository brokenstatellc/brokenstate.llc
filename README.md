<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Broken State</title>

<link href="https://fonts.googleapis.com/css2?family=Oswald:wght@400;500;700&family=Inter:wght@300;400;500;700&display=swap" rel="stylesheet">

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
scroll-behavior:smooth;
}

body{
background:#0a0a0a;
color:#fff;
font-family:'Inter',sans-serif;
overflow-x:hidden;
}

/* NAVBAR */

nav{
position:fixed;
top:0;
left:0;
width:100%;
padding:20px 8%;
display:flex;
justify-content:space-between;
align-items:center;
background:rgba(0,0,0,.95);
border-bottom:1px solid #1a1a1a;
z-index:1000;
}

.logo img{
height:55px;
}

nav ul{
display:flex;
gap:30px;
list-style:none;
}

nav a{
text-decoration:none;
color:white;
font-weight:500;
letter-spacing:1px;
}

nav a:hover{
opacity:.7;
}

/* HERO */

.hero{
height:100vh;
display:flex;
flex-direction:column;
justify-content:center;
align-items:center;
text-align:center;
padding:20px;
background:
linear-gradient(rgba(0,0,0,.55),rgba(0,0,0,.85)),
url("https://images.unsplash.com/photo-1523398002811-999ca8dec234?auto=format&fit=crop&w=1600&q=80");
background-size:cover;
background-position:center;
}

.hero-logo{
width:min(700px,90%);
margin-bottom:30px;
}

.hero h1{
font-family:'Oswald',sans-serif;
font-size:clamp(3rem,9vw,8rem);
text-transform:uppercase;
line-height:.9;
margin-bottom:20px;
}

.hero p{
font-size:1.1rem;
letter-spacing:2px;
color:#d1d1d1;
margin-bottom:40px;
}

.btn{
padding:15px 35px;
border:2px solid white;
color:white;
text-decoration:none;
font-weight:700;
transition:.3s;
}

.btn:hover{
background:white;
color:black;
}

/* SECTIONS */

section{
padding:100px 8%;
}

.section-title{
font-family:'Oswald',sans-serif;
font-size:4rem;
text-transform:uppercase;
margin-bottom:50px;
}

/* PRODUCT DROP */

.drop-grid{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(300px,1fr));
gap:25px;
}

.drop-item{
background:#111;
overflow:hidden;
}

.drop-item img{
width:100%;
height:500px;
object-fit:cover;
transition:.4s;
}

.drop-item:hover img{
transform:scale(1.05);
}

.drop-item h3{
padding:20px;
font-family:'Oswald',sans-serif;
font-size:1.5rem;
}

/* CATEGORIES */

.grid{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
gap:25px;
}

.card{
background:#111;
padding:40px;
border:1px solid #222;
transition:.3s;
}

.card:hover{
border-color:white;
transform:translateY(-5px);
}

.card h3{
font-family:'Oswald',sans-serif;
font-size:2rem;
margin-bottom:15px;
}

.card p{
line-height:1.8;
color:#bdbdbd;
}

/* ABOUT */

.about{
max-width:900px;
}

.about p{
font-size:1.05rem;
line-height:2;
color:#c7c7c7;
}

/* CONTACT */

.contact{
background:#111;
padding:40px;
border:1px solid #222;
}

.contact p{
margin-bottom:15px;
}

/* FOOTER */

footer{
padding:60px 20px;
text-align:center;
border-top:1px solid #222;
}

footer h2{
font-family:'Oswald',sans-serif;
font-size:3rem;
margin-bottom:10px;
}

footer p{
color:#888;
}

</style>
</head>
<body>

<nav>

<div class="logo">
<img src="broken-state-logo.png" alt="Broken State Logo">
</div>

<ul>
<li><a href="#home">HOME</a></li>
<li><a href="#drop">SHOP</a></li>
<li><a href="#categories">CATEGORIES</a></li>
<li><a href="#about">ABOUT</a></li>
<li><a href="#contact">CONTACT</a></li>
</ul>

</nav>

<section class="hero" id="home">

<img src="broken-state-logo.png"
alt="Broken State"
class="hero-logo">

<h1>BROKEN STATE</h1>

<p>
FOR THE ONES WHO NEVER FIT IN.
</p>

<a href="#drop" class="btn">
SHOP NOW
</a>

</section>

<section id="drop">

<h2 class="section-title">
LATEST DROP
</h2>

<div class="drop-grid">

<div class="drop-item">
<img src="hoodie.jpg" alt="Hoodie">
<h3>BROKEN STATE HOODIE</h3>
</div>

<div class="drop-item">
<img src="shirt.jpg" alt="Shirt">
<h3>BROKEN STATE TEE</h3>
</div>

<div class="drop-item">
<img src="pants.jpg" alt="Pants">
<h3>STATEMENT PANTS</h3>
</div>

</div>

</section>

<section id="categories">

<h2 class="section-title">
CATEGORIES
</h2>

<div class="grid">

<div class="card">
<h3>SHIRTS</h3>

<p>
Oversized graphic tees featuring bold artwork,
premium materials and designs inspired by the
Broken State mindset.
</p>

</div>

<div class="card">

<h3>HOODIES</h3>

<p>
Heavyweight hoodies built for comfort,
quality and statement-making streetwear fits.
</p>

</div>

<div class="card">

<h3>PANTS</h3>

<p>
Statement pieces built to lead the outfit.
Bold silhouettes, distressed details and designs
made to stand apart from everything else.
</p>

</div>

</div>

</section>

<section id="about">

<h2 class="section-title">
ABOUT
</h2>

<div class="about">

<p>
Broken State is built for people who move differently.
The overlooked. The underestimated.
The ones who refuse to become what the world expects.
Every collection represents resilience, individuality
and turning struggle into purpose.
</p>

</div>

</section>

<section id="contact">

<h2 class="section-title">
CONTACT
</h2>

<div class="contact">

<p><strong>Instagram:</strong> @brokenstate</p>

<p><strong>TikTok:</strong> @brokenstate</p>

<p><strong>Email:</strong> contact@brokenstate.com</p>

</div>

</section>

<footer>

<h2>BROKEN STATE</h2>

<p>
FOR THE ONES WHO NEVER FIT IN.
</p>

</footer>

</body>
</html>