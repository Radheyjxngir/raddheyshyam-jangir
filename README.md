<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Trending Shoes — Luxury Dark Brand</title>

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800;900&display=swap" rel="stylesheet">

<style>
:root{
  --bg:#0a0a0d;
  --bg-soft:#0e0e12;
  --text:#f5f5f5;
  --muted:#9a9a9a;
}

*{margin:0;padding:0;box-sizing:border-box;font-family:'Inter',sans-serif}

body{
  background:linear-gradient(180deg,var(--bg),var(--bg-soft));
  color:var(--text);
  overflow-x:hidden;
}

/* ================= NAVBAR ================= */
nav{
  position:fixed;
  top:0;left:0;
  width:100%;
  z-index:100;
  display:flex;
  align-items:center;
  justify-content:space-between;
  padding:22px 8%;
  background:rgba(10,10,13,.65);
  backdrop-filter:blur(18px);
  border-bottom:1px solid rgba(255,255,255,.05);
  position: fixed;
}

.logo{
  font-weight:900;
  letter-spacing:2px;
}

nav ul{
  display:flex;
  gap:36px;
  list-style:none;
}

nav a{
  color:var(--text);
  text-decoration:none;
  opacity:.85;
}

.menu-btn{
  display:none;
  font-size:1.7rem;
  cursor:pointer;
}

/* ================= HERO ================= */
.hero{
  min-height:100vh;
  display:flex;
  align-items:center;
  justify-content:center;
  text-align:center;
  padding:140px 8% 80px;
}

.hero h1{
  font-size:clamp(4rem,10vw,9rem);
  font-weight:900;
  background:linear-gradient(120deg,#f7f7f7,#d9d9d9,#bcbcbc,#9e9e9e);
  -webkit-background-clip:text;
  -webkit-text-fill-color:transparent;
}

.hero p{
  margin-top:30px;
  max-width:760px;
  margin-inline:auto;
  color:var(--muted);
}

/* ================= SECTIONS ================= */
section{
  padding:140px 8%;
}

section h2{
  font-size:3rem;
  font-weight:800;
  margin-bottom:40px;
  background:linear-gradient(90deg,#f5f5f5,#cfcfcf,#a8a8a8,#f5f5f5);
  -webkit-background-clip:text;
  -webkit-text-fill-color:transparent;
}

section p{
  color:var(--muted);
  max-width:720px;
  line-height:1.8;
}

/* ================= FEATURES ================= */
.features{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(260px,1fr));
  gap:60px;
  margin-top:80px;
}

.feature{
  padding:40px;
  border-radius:28px;
  background:rgba(255,255,255,.05);
  backdrop-filter:blur(18px);
  border:1px solid rgba(255,255,255,.2);
  box-shadow:0 30px 60px rgba(0,0,0,.6);
  transition:.6s;
}

.feature:hover{
  transform:translateY(-12px);
}

/* ================= DIVIDER ================= */
.divider{
  height:1px;
  background:linear-gradient(90deg,transparent,#fff,transparent);
  opacity:.15;
  margin:140px 0;
}

/* ================= STORE ================= */
.store{
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:80px;
}

iframe{
  width:100%;
  height:380px;
  border:none;
  border-radius:28px;
}

/* ================= CTA ================= */
.cta{
  text-align:center;
}

.cta-buttons{
  display:flex;
  justify-content:center;
  gap:30px;
  margin:40px 0;
}

.cta-btn{
  padding:16px 36px;
  border-radius:40px;
  text-decoration:none;
  color:#fff;
  background:rgba(255,255,255,.06);
  border:1px solid rgba(255,255,255,.25);
  backdrop-filter:blur(12px);
  box-shadow:0 20px 40px rgba(0,0,0,.6);
  transition:.4s;
}

.cta-btn:hover{
  transform:translateY(-6px);
}

.social{
  color:var(--muted);
  font-size:.9rem;
}

.social a{
  color:var(--text);
  text-decoration:none;
  margin-left:8px;
}

/* ================= FOOTER ================= */
footer{
  padding:80px 8%;
  text-align:center;
  border-top:1px solid rgba(255,255,255,.06);
  color:var(--muted);
}

/* ================= CURSOR LIGHT ================= */
.cursor-light{
  position:fixed;
  width:420px;
  height:420px;
  border-radius:50%;
  background:radial-gradient(circle,rgba(255,255,255,.12),transparent 65%);
  pointer-events:none;
  transform:translate(-50%,-50%);
  z-index:2;
}

/* ================= FILM CUT ================= */


/* ================= RESPONSIVE ================= */
@media(max-width:900px){
  nav ul{
    position:absolute;
    top:100%;
    left:0;
    width:100%;
    background:rgba(10,10,13,.95);
    flex-direction:column;
    gap:24px;
    padding:30px 0;
    display:none;
  }
  nav ul.show{display:flex}
  .menu-btn{display:block}
  .store{grid-template-columns:1fr}
}
</style>
</head>

<body>

<div class="film-cut" id="filmCut"></div>
<div class="cursor-light" id="cursor"></div>

<nav>
  <div class="logo">TRENDING SHOES</div>

  <ul>
    <li><a href="#">Home</a></li>
    <li><a href="#">Brand</a></li>
    <li><a href="#">Visit</a></li>
  </ul>

  <div class="menu-btn" id="menuBtn">☰</div>
</nav>

<div class="hero">
  <div>
    <h1>Trending Shoes</h1>
    <p>Luxury footwear experience near Railway Station, Hanumangarh. Minimal. Premium. Purposeful.</p>
  </div>
</div>

<div class="divider"></div>

<section>
  <h2>The Brand</h2>
  <p>Trending Shoes is about presence. Calm, dark, refined footwear curation for people who value quality over noise.</p>

  <div class="features">
    <div class="feature"><h3>Curated Selection</h3><p>Only trending & timeless shoes.</p></div>
    <div class="feature"><h3>Premium Feel</h3><p>Material & comfort first.</p></div>
    <div class="feature"><h3>Local Trust</h3><p>Proudly Hanumangarh.</p></div>
  </div>
</section>

<div class="divider"></div>

<section>
  <h2>Visit the Store</h2>
  <div class="store">
    <p>Near Railway Station, Hanumangarh. Walk in and experience footwear with purpose.</p>
    <iframe src="https://www.google.com/maps?q=Trending+Shoes+Hanumangarh&output=embed"></iframe>
  </div>
</section>

<section class="cta">
  <h2>Connect With Us</h2>
  <div class="cta-buttons">
    <a href="https://wa.me/7727871322" class="cta-btn">WhatsApp For Order</a>
    <a href="tel:+917727871322" class="cta-btn">Call Now</a>
  </div>
  <div class="social">
    Follow on Instagram
    <a href="https://www.instagram.com/trending_shoes_hanumangarh_/" target="_blank">
      @trending_shoes_hanumangarh_
    </a>
  </div>
</section>

<footer>
  © 2025 Trending Shoes — Luxury Footwear Brand
</footer>

<script>
/* Cursor light */
const cursor=document.getElementById('cursor');
window.addEventListener('mousemove',e=>{
  cursor.style.left=e.clientX+'px';
  cursor.style.top=e.clientY+'px';
});

/* Film cut */
const film=document.getElementById('filmCut');
let last=0;
const secs=[...document.querySelectorAll('.hero,section')];

window.addEventListener('scroll',()=>{
  let cur=0;
  secs.forEach((s,i)=>{
    if(s.getBoundingClientRect().top<innerHeight*0.4) cur=i;
  });
  if(cur!==last){
    film.classList.add('active');
    setTimeout(()=>film.classList.remove('active'),1000);
    last=cur;
  }
});

/* Mobile menu */
const menuBtn=document.getElementById('menuBtn');
const navList=document.querySelector('nav ul');
menuBtn.addEventListener('click',()=>navList.classList.toggle('show'));

/* Manifesto */
const manifesto=document.createElement('div');
manifesto.textContent='Yoesh Suthar';
Object.assign(manifesto.style,{
  position:'fixed',
  bottom:'40px',
  left:'50%',
  transform:'translateX(-50%)',
  letterSpacing:'4px',
  fontSize:'0.8rem',
  color:'rgba(255,255,255,.5)'
});
document.body.appendChild(manifesto);
</script>

</body>
</html>
// subtle navbar shadow on scroll
window.addEventListener('scroll',()=>{
  document.querySelector('.navbar').classList.toggle('scrolled',window.scrollY>50)
})
// Navbar shadow
window.addEventListener('scroll',()=>{
  document.querySelector('.navbar').classList.toggle('scrolled',window.scrollY>60)
})

// Scroll reveal
const reveals=document.querySelectorAll('.reveal')
const revealOnScroll=()=>{
  reveals.forEach(el=>{
    const top=el.getBoundingClientRect().top
    if(top<window.innerHeight-80)el.classList.add('active')
  })
}
window.addEventListener('scroll',revealOnScroll)
revealOnScroll()
/* ================= FINAL MUSEUM FINISH ================= */

/* Museum Loader */
.museum-loader{
  position:fixed;
  inset:0;
  background:#0a0a0d;
  z-index:10000;
  display:flex;
  align-items:center;
  justify-content:center;
}
.museum-loader h1{
  font-size:clamp(2rem,6vw,4rem);
  letter-spacing:6px;
  font-weight:900;
  opacity:0;
  animation:loaderText 2.6s ease forwards;
}
@keyframes loaderText{
  from{opacity:0;letter-spacing:24px}
  to{opacity:1;letter-spacing:6px}
}

/* Fade main like gallery lights on */
main{opacity:0;transition:opacity 1.4s ease}
body.loaded main{opacity:1}

/* Grain toggle label */
.grain-control{
  position:fixed;
  right:30px;
  bottom:30px;
  font-size:.65rem;
  letter-spacing:2px;
  color:rgba(255,255,255,.45);
  z-index:9;
  cursor:pointer;
}
