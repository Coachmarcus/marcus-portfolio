<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Emmanuel Books | Trusted Bookstore</title>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
<script src="https://js.paystack.co/v1/inline.js"></script>
<style>
:root{
--blue:#143c6d;
--cream:#f9f7f2;
--accent:#d9a441;
--shadow:0 10px 25px rgba(0,0,0,.1);
}
*{margin:0;padding:0;box-sizing:border-box;font-family:Inter,sans-serif;scroll-behavior:smooth;}
body{background:var(--cream);color:#222}
.dark{--cream:#121212;--blue:#0a3a7a;background:#121212;color:#eee}
.dark header, .dark section, .dark .card, .dark .contact-card{background:#1e1e1e;color:#eee}
header{position:sticky;top:0;background:#fff;box-shadow:0 4px 12px rgba(0,0,0,.05);z-index:999}
.nav{max-width:1200px;margin:auto;padding:15px 20px;display:flex;justify-content:space-between;align-items:center}
.logo{font-size:22px;font-weight:700;color:var(--blue)}
.nav-buttons a{margin-left:8px;padding:10px 18px;border-radius:25px;background:#fff;color:var(--blue);font-weight:600;text-decoration:none;box-shadow:var(--shadow)}
.nav-buttons a.active,.nav-buttons a:hover{background:var(--blue);color:#fff}
#modeToggle{padding:8px 14px;border-radius:20px;border:none;background:#143c6d;color:#fff;cursor:pointer;margin-left:10px}

/* HERO */
.hero{min-height:60vh;display:flex;align-items:center;background:linear-gradient(rgba(20,60,109,.65),rgba(20,60,109,.65)),url("https://images.unsplash.com/photo-1524995997946-a1c2e315a42f") center/cover;color:#fff;padding:40px 20px}
.hero-content{max-width:1100px;margin:auto}
.hero h1{font-size:42px}
.hero p{margin:20px 0;font-size:18px;max-width:650px}
.hero a{padding:14px 28px;border-radius:30px;font-weight:600;text-decoration:none;margin-right:10px}
.primary{background:var(--accent);color:#000}
.secondary{background:#fff;color:var(--blue)}

section{padding:90px 20px}
.title{text-align:center;margin-bottom:50px}
.title h2{font-size:32px;color:var(--blue)}

/* SEARCH */
.search-box{max-width:600px;margin:0 auto 40px}
.search-box input{width:100%;padding:15px;border-radius:30px;border:none;box-shadow:var(--shadow);font-size:16px}

/* BOOKS */
.grid{max-width:1200px;margin:auto;display:grid;grid-template-columns:repeat(auto-fit,minmax(250px,1fr));gap:30px}
.card{background:#fff;border-radius:20px;overflow:hidden;box-shadow:var(--shadow);opacity:0;transform:translateY(20px);transition:.6s;cursor:pointer}
.card.show{opacity:1;transform:none}
.card img{width:100%;height:180px;object-fit:cover}
.card .content{padding:20px}
.badge{background:var(--accent);padding:5px 12px;border-radius:15px;font-size:12px;font-weight:600;display:inline-block;margin-bottom:10px}
.card h3{color:var(--blue)}
.card input{margin-bottom:6px;padding:6px;border-radius:8px;border:1px solid #ccc;width:60px}

/* SERVICES */
.services{background:#fff}
.services-grid{max-width:1100px;margin:auto;display:grid;grid-template-columns:repeat(auto-fit,minmax(250px,1fr));gap:30px}
.service{padding:30px;border-radius:20px;box-shadow:var(--shadow);background:var(--cream)}

/* TESTIMONIALS */
.testimonials{background:#143c6d;color:#fff;text-align:center;padding:70px 20px}
.testimonial{max-width:700px;margin:auto;font-size:18px;display:none}
.testimonial.active{display:block}

/* CONTACT */
.contact-wrap{max-width:1100px;margin:auto;display:grid;grid-template-columns:1fr 1fr;gap:40px}
.contact-card{background:#fff;padding:30px;border-radius:20px;box-shadow:var(--shadow)}
.contact-card input,.contact-card textarea{width:100%;padding:12px;margin-bottom:12px;border-radius:12px;border:1px solid #ccc}
.contact-card button{width:100%;padding:14px;border:none;border-radius:25px;background:var(--blue);color:#fff;font-weight:600}
#total{font-weight:600;margin-bottom:10px}

/* MAP */
.map{border-radius:20px;overflow:hidden;box-shadow:var(--shadow)}

/* WHATSAPP */
.whatsapp{position:fixed;bottom:20px;right:20px;width:55px;height:55px;background:#25D366;color:#fff;display:flex;align-items:center;justify-content:center;border-radius:50%;font-size:26px;box-shadow:0 8px 20px rgba(0,0,0,.25);z-index:2000}

/* BACK TO TOP */
#topBtn{position:fixed;bottom:90px;right:20px;width:45px;height:45px;border-radius:50%;border:none;background:#143c6d;color:#fff;font-size:18px;display:none;box-shadow:0 6px 16px rgba(0,0,0,.3);cursor:pointer;z-index:2000}

/* MOBILE */
@media(max-width:768px){
.hero h1{font-size:32px}
.contact-wrap{grid-template-columns:1fr}
}
</style>
</head>
<body>

<header>
  <div class="nav">
    <div class="logo">Emmanuel Books</div>
    <div>
      <a class="nav-buttons" href="#home">Home</a>
      <a class="nav-buttons" href="#books">Books</a>
      <a class="nav-buttons" href="#contact">Contact</a>
      <button id="modeToggle">🌙</button>
    </div>
  </div>
</header>

<section class="hero" id="home">
  <div class="hero-content">
    <h1>Your Trusted Bookstore for Learning & Inspiration</h1>
    <p>Educational, religious and general books for readers of all ages.</p>
    <a href="#books" class="primary">Browse Books</a>
    <a href="#contact" class="secondary">Visit Store</a>
  </div>
</section>

<section id="books">
  <div class="title"><h2>Our Books</h2></div>
  <div class="search-box"><input id="search" placeholder="Search books..."></div>
  <div class="grid" id="booksGrid">
    <div class="card" data-category="Educational"><img src="https://images.unsplash.com/photo-1512820790803-83ca734da794">
      <div class="content"><span class="badge">In-Store</span><h3>Educational Books</h3></div>
    </div>
    <div class="card" data-category="Religious"><img src="https://images.unsplash.com/photo-1509021436665-8f07dbf5bf1d">
      <div class="content"><span class="badge">In-Store</span><h3>Religious Books</h3></div>
    </div>
    <div class="card" data-category="Fiction"><img src="https://images.unsplash.com/photo-1524578271613-d550eacf6090">
      <div class="content"><span class="badge">In-Store</span><h3>Fiction & Novels</h3></div>
    </div>
    <div class="card" data-category="Stationery"><img src="https://images.unsplash.com/photo-1584697964192-39c5d4e78d9a">
      <div class="content"><span class="badge">In-Store</span><h3>Stationery</h3></div>
    </div>
  </div>
</section>

<section class="services">
  <div class="title"><h2>Why Choose Emmanuel Books</h2></div>
  <div class="services-grid">
    <div class="service">📚 Wide Book Collection</div>
    <div class="service">💬 Friendly Assistance</div>
    <div class="service">🏫 Student-Focused</div>
    <div class="service">📍 Easy Local Access</div>
  </div>
</section>

<section class="testimonials">
  <div class="testimonial active">“Best bookstore in town. Always helpful.”</div>
  <div class="testimonial">“I found all my school books here.”</div>
  <div class="testimonial">“Affordable and reliable.”</div>
</section>

<section id="contact">
  <div class="title"><h2>Contact Us</h2></div>
  <div class="contact-wrap">
    <div class="contact-card">
      <p>📞 +234 XXX XXX XXXX</p>
      <p>💬 WhatsApp Available</p>
      <input placeholder="Your Name" required>
      <input placeholder="Phone" required>
      <textarea placeholder="Book Request" required></textarea>
      <input type="number" id="qty" placeholder="Quantity" min="1" value="1">
      <input type="number" id="price" placeholder="Price per book (₦)" required>
      <p id="total">Total: ₦0</p>
      <button onclick="order(event)">Send Request</button>
    </div>
    <div class="map"><iframe src="https://www.google.com/maps?q=Nigeria&output=embed" width="100%" height="350" style="border:0"></iframe></div>
  </div>
</section>

<section id="admin" style="display:none;padding:50px;background:#f1f1f1;">
  <h2>Admin Panel</h2>
  <p>Add new books here:</p>
  <input id="bookName" placeholder="Book Name">
  <input id="bookPrice" placeholder="Price (₦)">
  <input id="bookID" placeholder="Book ID">
  <button onclick="addBook()">Add Book</button>

  <h3>Books List:</h3>
  <ul id="bookList"></ul>
</section>

<footer>© Emmanuel Books</footer>

<a class="whatsapp" href="https://wa.me/234XXXXXXXXXX" target="_blank">💬</a>
<button id="topBtn">↑</button>

<script>
// Dark mode
const toggle=document.getElementById("modeToggle");
if(localStorage.mode==="dark") document.body.classList.add("dark");
toggle.onclick=()=>{document.body.classList.toggle("dark");localStorage.mode=document.body.classList.contains("dark")?"dark":"light";}

// Active nav
const sections=document.querySelectorAll("section");
const links=document.querySelectorAll(".nav-buttons");
window.addEventListener("scroll",()=>{
let current="";
sections.forEach(s=>{if(scrollY>=s.offsetTop-120)current=s.id});
links.forEach(a=>{a.classList.remove("active");if(a.getAttribute("href")==="#"+current)a.classList.add("active")});
});

// Reveal
const cards=document.querySelectorAll(".card");
const io=new IntersectionObserver(e=>e.forEach(x=>x.isIntersecting&&x.target.classList.add("show")));
cards.forEach(c=>io.observe(c));

// Search
document.getElementById("search").onkeyup=e=>{
document.querySelectorAll(".card").forEach(c=>{c.style.display=c.innerText.toLowerCase().includes(e.target.value.toLowerCase())?"block":"none";});
};

// Testimonials
let i=0;setInterval(()=>{const t=document.querySelectorAll(".testimonial");t.forEach(x=>x.classList.remove("active"));t[i=(i+1)%t.length].classList.add("active");},4000);

// Order
function order(e){
const d=document.querySelectorAll(".contact-card input, .contact-card textarea");
const qty=document.getElementById("qty").value;
const price=document.getElementById("price").value;
const total=document.getElementById("total");
total.textContent="Total: ₦"+(qty*price||0);
const message=`Hello Emmanuel Books,%0AName:${d[0].value}%0APhone:${d[1].value}%0ABook:${d[2].value}%0AQuantity:${qty}%0APrice per Book:₦${price}%0ATotal:₦${qty*price}`;
window.open(`https://wa.me/234XXXXXXXXXX?text=${message}`,"_blank");
}

// Back to top
const topBtn=document.getElementById("topBtn");
window.onscroll=()=>topBtn.style.display=scrollY>500?"block":"none";
topBtn.onclick=()=>scrollTo({top:0,behavior:"smooth"});

// ----------------- BOOKS FUNCTIONALITY -------------------
const booksGrid=document.getElementById("booksGrid");
const originalCards=[...booksGrid.children];
let cart=[];

function showCategoryBooks(category){
    booksGrid.innerHTML="";
    for(let i=1;i<=8;i++){
        const card=document.createElement("div");
        card.className="card";
        card.innerHTML=`
            <img src="https://images.unsplash.com/photo-1524995997946-a1c2e315a42f">
            <div class="content">
                <h3>${category} Book ${i}</h3>
                <span class="badge">In-Store</span>
                <p>Price: ₦<input type="number" class="price" value="${1000+i*500}"></p>
                <p>Qty: <input type="number" class="qty" value="1" min="1"></p>
                <button class="add-cart" data-id="${category}${i}">Add to Cart</button>
            </div>
        `;
        booksGrid.appendChild(card);
    }

    const backBtn=document.createElement("button");
    backBtn.textContent="← Back to Categories";
    backBtn.style.cssText="margin:20px auto; display:block; padding:10px 20px; border:none; border-radius:25px; background:#143c6d; color:#fff; font-weight:600; cursor:pointer;";
    backBtn.onclick=()=>{restoreCategories()};
    booksGrid.appendChild(backBtn);

    attachCartButtons();
}

function restoreCategories(){
    booksGrid.innerHTML="";
    originalCards.forEach(c=>booksGrid.appendChild(c));
    attachCategoryClick();
}

function attachCategoryClick(){
    const cards=document.querySelectorAll("#booksGrid .card");
    cards.forEach(card=>{
        card.onclick=()=>{
            const category=card.getAttribute("data-category");
            showCategoryBooks(category);
        }
    });
}

function attachCartButtons(){
    const addBtns=document.querySelectorAll(".add-cart");
    addBtns.forEach(btn=>{
        btn.onclick=()=>{
            const card=btn.closest(".card");
            const id=btn.getAttribute("data-id");
            const name=card.querySelector("h3").innerText;
            const qty=parseInt(card.querySelector(".qty").value);
            const price=parseFloat(card.querySelector(".price").value);
            const total=qty*price;

            const existing=cart.find(b=>b.id===id);
            if(existing){
                existing.qty=qty;
                existing.price=price;
                existing.total=total;
            } else {
                cart.push({id,name,qty,price,total});
            }
            alert(`${name} added to cart.\nQty: ${qty}\nPrice: ₦${price}\nTotal: ₦${total}`);
        }
    });
}

attachCategoryClick();

// ----------------- ADMIN PANEL -------------------
const bookList=document.getElementById("bookList");
function addBook(){
  let name=document.getElementById("bookName").value;
  let price=document.getElementById("bookPrice").value;
  let id=document.getElementById("bookID").value;
  if(name && price && id){
    let li=document.createElement("li");
    li.textContent=`${name} - ₦${price} (ID: ${id})`;
    bookList.appendChild(li);
    
    let payBtn=document.createElement("button");
    payBtn.textContent=`Pay ₦${price}`;
    payBtn.className="pay-btn";
    payBtn.setAttribute("data-price",price);
    payBtn.setAttribute("data-id",id);
    li.appendChild(payBtn);

    payBtn.onclick=()=>{
      let priceKobo=price*100;
      let handler=PaystackPop.setup({
        key:'YOUR_PUBLIC_KEY',
        email:'customer@example.com',
        amount:priceKobo,
        currency:"NGN",
        ref:id+"_"+Math.floor(Math.random()*1000000),
        onClose:function(){alert('Payment cancelled');},
        callback:function(resp){alert('Payment successful. Ref: '+resp.reference);}
      });
      handler.openIframe();
    }

    document.getElementById("bookName").value="";
    document.getElementById("bookPrice").value="";
    document.getElementById("bookID").value="";
  }
}
</script>
</body>
</html>
