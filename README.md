<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Garki Supermarket</title>

<style>
:root{
--bg:#f4f4f4;
--text:#111;
--card:#ffffff;
--primary:#0a7d32;
}
.dark{
--bg:#121212;
--text:#f1f1f1;
--card:#1e1e1e;
}
body{
margin:0;
font-family:Arial,sans-serif;
background:var(--bg);
color:var(--text);
transition:.3s;
}

/* HEADER (unchanged) */
.header{
background:var(--primary);
color:#fff;
padding:22px;
text-align:center;
position:sticky;
top:0;
z-index:999;
box-shadow:0 4px 6px rgba(0,0,0,0.1);
}
.toggle{
position:absolute;
right:15px;
top:15px;
border:none;
background:#fff;
padding:6px 10px;
border-radius:6px;
cursor:pointer;
}

/* Layout */
.container{padding:18px;}
.card{
background:var(--card);
border-radius:14px;
padding:16px;
margin-bottom:20px;
box-shadow:0 4px 12px rgba(0,0,0,.12);
}

/* Carousel */
.carousel img{
width:100%;
border-radius:12px;
display:none;
}
.carousel img.active{display:block;}

/* Contact */
.contact-grid{
display:grid;
grid-template-columns:1fr 1fr;
gap:12px;
}
.contact-btn{
display:flex;
align-items:center;
justify-content:center;
gap:8px;
padding:12px;
border-radius:10px;
text-decoration:none;
font-weight:bold;
color:#fff;
}
.call{background:#0a7d32;}
.whatsapp{background:#25d366;}
.email{background:#3f51b5;}
.map{background:#ff9800;}

/* Product Slider */
.product-slider{
overflow:hidden;
margin-top:10px;
}
.product-track{
display:flex;
transition:transform .6s ease;
}
.product-group{
min-width:100%;
display:grid;
grid-template-columns:repeat(auto-fit,minmax(140px,1fr));
gap:14px;
}
.product{
background:var(--bg);
border-radius:12px;
padding:10px;
text-align:center;
}
.product img{
width:100%;
height:120px;
object-fit:cover;
border-radius:10px;
}
.product h4{
font-size:14px;
margin:8px 0 4px;
}
.product span{
font-size:12px;
color:#666;
}
.product button{
margin-top:6px;
padding:8px;
width:100%;
border:none;
border-radius:8px;
background:var(--primary);
color:#fff;
font-size:13px;
cursor:pointer;
}

/* Order */
input,textarea{
width:100%;
padding:10px;
margin:8px 0;
border-radius:8px;
border:1px solid #ccc;
}
button.send{
background:var(--primary);
color:#fff;
border:none;
padding:10px;
border-radius:8px;
width:100%;
cursor:pointer;
}

/* Reviews */
.reviews{
display:grid;
gap:16px;
}
.review-card{
background:var(--bg);
border-radius:14px;
padding:14px;
display:flex;
gap:14px;
align-items:flex-start;
}
.review-img{
width:50px;
height:50px;
border-radius:50%;
object-fit:cover;
}
.review-body{flex:1;}
.review-name{
font-weight:bold;
font-size:14px;
}
.stars{
color:#ffc107;
font-size:14px;
margin:3px 0;
}
.review-text{
font-size:14px;
line-height:1.4;
}

/* Map */
iframe{
width:100%;
height:280px;
border:none;
border-radius:12px;
}

/* Bottom buttons */
.bottom{
position:fixed;
bottom:0;
left:0;
width:100%;
display:flex;
z-index:1000;
}
.bottom a{
flex:1;
text-align:center;
padding:14px;
color:#fff;
font-weight:bold;
text-decoration:none;
}
.space{height:80px;}

/* Bottom slide-out navigation drawer */
.bottom-drawer{
position:fixed;
bottom:0;
left:0;
width:100%;
z-index:1001;
font-family:Arial, sans-serif;
}
.drawer-toggle{
background:var(--primary);
color:#fff;
text-align:center;
padding:12px;
cursor:pointer;
border-top-left-radius:12px;
border-top-right-radius:12px;
font-weight:bold;
font-size:16px;
}
.drawer-content{
background:var(--primary);
display:flex;
justify-content:space-around;
padding:12px 0;
transform:translateY(100%);
transition:transform .3s ease;
border-top-left-radius:12px;
border-top-right-radius:12px;
}
.drawer-content a{
color:#fff;
text-decoration:none;
font-weight:bold;
padding:6px 12px;
border-radius:6px;
transition:0.2s;
}
.drawer-content a:hover{
background:rgba(255,255,255,0.2);
}
.drawer-open .drawer-content{
transform:translateY(0);
}
</style>
</head>

<body>

<!-- HEADER (green box remains unchanged) -->
<div class="header">
<h2>Garki Supermarket</h2>
<p>Everyday Shopping – Garki, Abuja</p>
<button class="toggle" onclick="toggleMode()">🌙</button>
</div>

<div class="container">

<!-- Featured Carousel -->
<div id="home" class="card carousel">
<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQiel_mTLxW0KjAeE68J-ZX4s1mYgOSG0B4n4bKYpZ2Cw&s=10" class="active">
<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRo4K7v-TATHLzL-K9E3GVWGjTIKB6aFnsj8W_kOg3Bxg&s=10">
<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTR79gPnLPfSgN6iUYRR7da0cBymwdV-F4eMnmL5opgdQ&s=10">
<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRaYAEJN6CaZZ-esXbyaRoJfbcQbzbXpdn94lGupSFxRA&s=10">
</div>

<!-- About -->
<div class="card">
<h3>About Us</h3>
<p>
Garki Supermarket provides fresh groceries, household items,
drinks and daily essentials at affordable prices. Open daily to serve you.
</p>
</div>

<!-- Contact Section -->
<div id="contact" class="card">
<h3>Contact Details</h3>
<div class="contact-grid">
<a href="tel:+2340000000000" class="contact-btn call">📞 Call</a>
<a href="https://wa.me/2340000000000" class="contact-btn whatsapp">💬 WhatsApp</a>
<a href="mailto:info@garkisupermarket.com" class="contact-btn email">✉️ Email</a>
<a href="https://www.google.com/maps?q=Garki+Supermarket+Abuja" target="_blank" class="contact-btn map">📍 Map</a>
</div>
</div>

<!-- Product Slider -->
<div id="products" class="card">
<h3>Popular Products</h3>
<div class="product-slider">
<div class="product-track" id="track">

<!-- Group 1 -->
<div class="product-group">
<div class="product">
<img src="https://images.unsplash.com/photo-1580910051074-7c36a63c6b1c">
<h4>Rice (50kg)</h4>
<span>ID: P001</span>
<button onclick="addToCart('P001','Rice 50kg')">Add to Cart</button>
</div>
<div class="product">
<img src="https://images.unsplash.com/photo-1604719312566-8912e9227c6a">
<h4>Vegetable Oil</h4>
<span>ID: P002</span>
<button onclick="addToCart('P002','Vegetable Oil')">Add to Cart</button>
</div>
<div class="product">
<img src="https://images.unsplash.com/photo-1542838132-92c53300491e">
<h4>Sugar</h4>
<span>ID: P003</span>
<button onclick="addToCart('P003','Sugar')">Add to Cart</button>
</div>
<div class="product">
<img src="https://images.unsplash.com/photo-1615486364462-ef6363adbc18">
<h4>Milk</h4>
<span>ID: P004</span>
<button onclick="addToCart('P004','Milk')">Add to Cart</button>
</div>
</div>

<!-- Group 2 -->
<div class="product-group">
<div class="product">
<img src="https://images.unsplash.com/photo-1585238342028-4bbc1c8bfa5f">
<h4>Soft Drinks</h4>
<span>ID: P005</span>
<button onclick="addToCart('P005','Soft Drinks')">Add to Cart</button>
</div>
<div class="product">
<img src="https://images.unsplash.com/photo-1580910365203-8c68e85b4c2f">
<h4>Bread</h4>
<span>ID: P006</span>
<button onclick="addToCart('P006','Bread')">Add to Cart</button>
</div>
<div class="product">
<img src="https://images.unsplash.com/photo-1587049352851-8d93c0f03f23">
<h4>Detergent</h4>
<span>ID: P007</span>
<button onclick="addToCart('P007','Detergent')">Add to Cart</button>
</div>
<div class="product">
<img src="https://images.unsplash.com/photo-1612209924761-2c9db1f25c4c">
<h4>Toothpaste</h4>
<span>ID: P008</span>
<button onclick="addToCart('P008','Toothpaste')">Add to Cart</button>
</div>
</div>

</div>
</div>
</div>

<!-- Order Form -->
<div class="card">
<h3>Your Order</h3>
<form onsubmit="sendOrder(event)">
<input id="name" placeholder="Your Name" required>
<input id="phone" placeholder="Phone Number" required>
<textarea id="orderBox" placeholder="Selected products will appear here" readonly></textarea>
<button class="send">Send Order via WhatsApp</button>
</form>
</div>

<!-- Customer Reviews -->
<div id="reviews" class="card">
<h3>Customer Reviews</h3>
<div class="reviews">
<div class="review-card">
<img src="https://randomuser.me/api/portraits/women/44.jpg" class="review-img">
<div class="review-body">
<div class="review-name">Amina Yusuf</div>
<div class="stars">★★★★★</div>
<div class="review-text">Affordable prices and always fresh groceries. Highly recommended.</div>
</div>
</div>
<div class="review-card">
<img src="https://randomuser.me/api/portraits/men/32.jpg" class="review-img">
<div class="review-body">
<div class="review-name">Samuel Okoye</div>
<div class="stars">★★★★☆</div>
<div class="review-text">Good customer service and easy to locate. Parking could improve.</div>
</div>
</div>
<div class="review-card">
<img src="https://randomuser.me/api/portraits/women/68.jpg" class="review-img">
<div class="review-body">
<div class="review-name">Mary Johnson</div>
<div class="stars">★★★★★</div>
<div class="review-text">Best supermarket around Garki. Everything I need in one place.</div>
</div>
</div>
</div>
</div>

<!-- Map -->
<div class="card">
<h3>Find Us</h3>
<iframe src="https://www.google.com/maps?q=Garki+Supermarket+Abuja&output=embed"></iframe>
</div>

</div>

<div class="space"></div>

<!-- Bottom fixed buttons -->
<div class="bottom">
<a href="tel:+2340000000000" class="call">Call</a>
<a href="https://www.google.com/maps?q=Garki+Supermarket+Abuja" class="map">Directions</a>
<a href="https://wa.me/2340000000000" class="whatsapp">WhatsApp</a>
</div>

<!-- Bottom slide-out navigation drawer -->
<div id="bottomDrawer" class="bottom-drawer">
  <div class="drawer-toggle" onclick="toggleDrawer()">☰ Menu</div>
  <div class="drawer-content">
    <a href="#home">Home</a>
    <a href="#products">Products</a>
    <a href="#contact">Contact</a>
    <a href="#reviews">Reviews</a>
  </div>
</div>

<script>
let dark=false;
function toggleMode(){document.body.classList.toggle("dark");}

/* Featured carousel */
let carouselSlides=document.querySelectorAll(".carousel img");
let ci=0;
setInterval(()=>{
carouselSlides[ci].classList.remove("active");
ci=(ci+1)%carouselSlides.length;
carouselSlides[ci].classList.add("active");
},3000);

/* Product slider auto-slide */
let track=document.getElementById("track");
let groupIndex=0;
setInterval(()=>{
groupIndex=(groupIndex+1)%2;
track.style.transform=`translateX(-${groupIndex*100}%)`;
},4000);

/* Cart */
let cart=[];
function addToCart(id,name){
cart.push(`${id} - ${name}`);
document.getElementById("orderBox").value=cart.join("\n");
}

/* WhatsApp order */
function sendOrder(e){
e.preventDefault();
let msg=`Hello Garki Supermarket%0AName: ${name.value}%0APhone: ${phone.value}%0AOrder:%0A${cart.join("%0A")}`;
window.open(`https://wa.me/2340000000000?text=${msg}`);
}

/* Bottom drawer toggle */
function toggleDrawer(){
document.getElementById("bottomDrawer").classList.toggle("drawer-open");
}
</script>

</body>
</html>
