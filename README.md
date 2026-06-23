<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="referrer" content="strict-origin-when-cross-origin">

<meta http-equiv="X-Content-Type-Options" content="nosniff">
<meta http-equiv="X-Frame-Options" content="DENY">
<meta name="xss-protection" content="1; mode=block">

<title>𝑪𝒐𝒅 𝑶𝒇 𝑱𝒖𝒔𝒕𝒊𝒄𝒆 ⚖️</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

<link href="https://fonts.googleapis.com/css2?family=Vazirmatn:wght@300;400;600;700;800;900&family=Noto+Naskh+Arabic:wght@300;400;700&display=swap" rel="stylesheet">

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">

<style>
:root{
--bg:#0a0a0a;
--card:rgba(255,255,255,.04);
--line:rgba(255,255,255,.08);
--text:#f5f5f5;
--red:#ff1c1c;
--red-light:rgba(255,0,0,.12);
--green:#17d36b;
--gold:#c9a84c;
--shadow-color:rgba(0,0,0,0.5);
--header-bg:rgba(10,10,10,.90);
--border-color:rgba(255,255,255,.08);
--text-secondary:#888;
}

*{margin:0;padding:0;box-sizing:border-box}

html{scroll-behavior:smooth}

body{
font-family:'Vazirmatn',sans-serif;
background:var(--bg);
color:var(--text);
min-height:100vh;
overflow-x:hidden;
opacity:0;
animation:bodyFadeIn 1.2s ease forwards;
}

@keyframes bodyFadeIn{
0%{opacity:0}
100%{opacity:1}
}

/* ===== لودینگ ===== */
#loader{
position:fixed;
inset:0;
background:#0a0a0a;
z-index:9999;
display:flex;
flex-direction:column;
align-items:center;
justify-content:center;
transition:opacity .8s ease, visibility .8s ease;
}

#loader.hide{
opacity:0;
visibility:hidden;
pointer-events:none;
}

#loader .spinner{
width:60px;
height:60px;
border:3px solid rgba(255,0,0,.1);
border-top-color:#ff1c1c;
border-radius:50%;
animation:spin 1s linear infinite;
}

#loader p{
margin-top:20px;
color:#ff1c1c;
font-weight:700;
letter-spacing:3px;
font-size:.9rem;
animation:pulse 1.5s ease-in-out infinite;
}

@keyframes spin{
to{transform:rotate(360deg)}
}

@keyframes pulse{
0%,100%{opacity:0.4}
50%{opacity:1}
}

/* ===== ذرات ===== */
.particles{
position:fixed;
inset:0;
z-index:0;
pointer-events:none;
overflow:hidden;
}

.particle{
position:absolute;
background:#ff1c1c;
border-radius:50%;
opacity:0;
animation:particleFloat linear infinite;
box-shadow:0 0 10px #ff1c1c,0 0 20px rgba(255,0,0,.3);
}

.particle:nth-child(odd){
background:#ff6666;
box-shadow:0 0 15px #ff6666,0 0 30px rgba(255,100,100,.2);
}

@keyframes particleFloat{
0%{opacity:0;transform:translateY(100vh) scale(0) rotate(0deg)}
10%{opacity:0.9}
90%{opacity:0.7}
100%{opacity:0;transform:translateY(-10vh) scale(1) rotate(720deg)}
}

/* ===== اورب‌ها ===== */
.bg-orb{
position:fixed;
border-radius:50%;
filter:blur(120px);
opacity:.35;
z-index:0;
animation:float 20s infinite alternate ease-in-out;
pointer-events:none;
}

.orb1{background:rgba(255,0,0,.25);width:500px;height:500px;top:0;right:-10%}
.orb2{background:rgba(255,50,50,.15);width:500px;height:500px;bottom:0;left:-10%}
.orb3{background:rgba(255,0,0,.08);width:700px;height:700px;top:50%;left:50%;transform:translate(-50%,-50%);filter:blur(150px);opacity:.10;animation-duration:25s}

@keyframes float{
0%{transform:translate(0,0) scale(1)}
100%{transform:translate(80px,-60px) scale(1.1)}
}

/* ===== هدر ===== */
header{
background:rgba(10,10,10,.90);
backdrop-filter:blur(16px);
-webkit-backdrop-filter:blur(16px);
border-bottom:1px solid rgba(255,0,0,.15);
position:sticky;
top:0;
z-index:100;
box-shadow:0 4px 30px rgba(0,0,0,.5);
}

.topbar{
max-width:1200px;
margin:auto;
padding:16px 20px;
text-align:center;
}

.header-top{
display:flex;
align-items:center;
justify-content:center;
flex-wrap:wrap;
gap:10px;
margin-bottom:10px;
}

.brand{
font-size:2rem;
font-weight:900;
letter-spacing:.5px;
color:#fff;
position:relative;
display:inline-block;
}

.brand span{color:#ff1c1c}

/* ===== منو ===== */
nav ul{
list-style:none;
display:flex;
justify-content:center;
flex-wrap:wrap;
gap:8px;
margin-top:6px;
}

nav a{
text-decoration:none;
color:#bbb;
background:rgba(255,255,255,.04);
border:1px solid rgba(255,255,255,.08);
padding:8px 14px;
border-radius:999px;
cursor:pointer;
transition:all .35s cubic-bezier(.4,0,.2,1);
font-weight:500;
font-size:.85rem;
position:relative;
overflow:hidden;
}

nav a::after{
content:'';
position:absolute;
inset:0;
background:linear-gradient(135deg,var(--red-light),transparent);
opacity:0;
transition:opacity .4s;
border-radius:999px;
}

nav a:hover{
color:#fff;
border-color:rgba(255,255,255,.2);
transform:translateY(-2px);
box-shadow:0 4px 20px rgba(0,0,0,.3);
}

nav a:hover::after{opacity:1}

nav a.active{
color:#fff;
background:rgba(255,0,0,.2);
border-color:#ff1c1c;
box-shadow:0 0 30px rgba(255,0,0,.08), inset 0 0 20px rgba(255,0,0,.03);
}

nav a.active::after{opacity:0}

/* ===== دکمه رفتن به بالا ===== */
#scrollTop{
position:fixed;
bottom:30px;
right:30px;
z-index:99;
width:50px;
height:50px;
border-radius:50%;
background:linear-gradient(135deg,#ff1c1c,#8a0000);
border:none;
color:#fff;
font-size:1.3rem;
cursor:pointer;
box-shadow:0 4px 25px rgba(255,0,0,.25);
transition:all .4s cubic-bezier(.4,0,.2,1);
opacity:0;
transform:translateY(20px) scale(0.8);
pointer-events:none;
}

#scrollTop.visible{
opacity:1;
transform:translateY(0) scale(1);
pointer-events:auto;
}

#scrollTop:hover{
transform:translateY(-5px) scale(1.05);
box-shadow:0 8px 40px rgba(255,0,0,.35);
}

/* ===== تایمر 3D ===== */
#home .hero-timer{
max-width:700px;
margin:20px auto;
display:grid;
grid-template-columns:repeat(5,1fr);
gap:15px;
perspective:800px;
}

#home .time-box{
aspect-ratio:1;
display:flex;
flex-direction:column;
align-items:center;
justify-content:center;
background:rgba(255,255,255,.04);
border:1px solid rgba(255,255,255,.08);
border-radius:20px;
transition:all .6s cubic-bezier(.4,0,.2,1);
position:relative;
overflow:hidden;
animation:timeBoxIn .6s cubic-bezier(.4,0,.2,1) forwards;
opacity:0;
transform-style:preserve-3d;
}

#home .time-box:nth-child(1){animation-delay:0.1s}
#home .time-box:nth-child(2){animation-delay:0.2s}
#home .time-box:nth-child(3){animation-delay:0.3s}
#home .time-box:nth-child(4){animation-delay:0.4s}
#home .time-box:nth-child(5){animation-delay:0.5s}

@keyframes timeBoxIn{
0%{opacity:0;transform:scale(0.8) translateY(30px) rotateX(15deg)}
100%{opacity:1;transform:scale(1) translateY(0) rotateX(0)}
}

#home .time-box::before{
content:'';
position:absolute;
inset:0;
background:radial-gradient(circle at center,var(--red-light),transparent 70%);
opacity:0;
transition:opacity .6s;
}

#home .time-box:hover{
transform:translateY(-8px) scale(1.04) rotateX(5deg);
border-color:rgba(255,0,0,.3);
box-shadow:0 12px 50px rgba(255,0,0,.12), inset 0 0 40px rgba(255,0,0,.03);
}

#home .time-box:hover::before{opacity:1}

#home .time-num{
font-weight:900;
font-size:1.8rem;
color:#ff1c1c;
font-feature-settings:"tnum";
letter-spacing:1px;
position:relative;
z-index:1;
text-shadow:0 0 40px rgba(255,0,0,.1);
display:inline-block;
transition:all .3s ease;
}

#home .time-num.number-flash{
animation:numberFlash 0.4s cubic-bezier(.34,1.56,.64,1) forwards;
}

@keyframes numberFlash{
0%{transform:scale(1) rotateY(0);color:#ff1c1c;text-shadow:0 0 0 transparent}
25%{transform:scale(1.5) rotateY(180deg);color:#ff8888;text-shadow:0 0 50px rgba(255,0,0,.6)}
50%{transform:scale(0.8) rotateY(360deg);color:#ff1c1c;text-shadow:0 0 20px rgba(255,0,0,.2)}
75%{transform:scale(1.15) rotateY(180deg);color:#ff4444;text-shadow:0 0 30px rgba(255,0,0,.3)}
100%{transform:scale(1) rotateY(0);color:#ff1c1c;text-shadow:0 0 40px rgba(255,0,0,.1)}
}

#home .time-box:hover .time-num{
animation:numberPop 0.4s cubic-bezier(.34,1.56,.64,1);
}

@keyframes numberPop{
0%{transform:scale(1)}
50%{transform:scale(1.25)}
100%{transform:scale(1)}
}

#home .time-box .label{
font-size:.7rem;
color:#888;
font-weight:400;
letter-spacing:2px;
position:relative;
z-index:1;
margin-top:2px;
transition:color .3s;
}

#home .time-box:hover .label{
color:#ff1c1c;
}

/* ===== استریکر ===== */
#home .sticker-row{
display:flex;
flex-wrap:wrap;
justify-content:center;
align-items:center;
gap:14px 20px;
margin:22px auto 8px;
padding:16px 28px;
max-width:700px;
background:rgba(255,255,255,.04);
backdrop-filter:blur(12px);
-webkit-backdrop-filter:blur(12px);
border-radius:60px;
border:1px solid rgba(255,255,255,.06);
box-shadow:0 8px 32px rgba(0,0,0,.3), inset 0 1px 0 rgba(255,255,255,.05);
transition:all .5s cubic-bezier(.4,0,.2,1);
animation:stickerIn .8s ease forwards;
opacity:0;
animation-delay:0.7s;
}

@keyframes stickerIn{
0%{opacity:0;transform:translateY(30px) scale(0.95)}
100%{opacity:1;transform:translateY(0) scale(1)}
}

#home .sticker-row:hover{
background:rgba(255,255,255,.07);
border-color:rgba(255,0,0,.15);
box-shadow:0 8px 48px rgba(255,0,0,.06);
}

#home .sticker-item{
display:flex;
align-items:center;
gap:8px;
padding:6px 16px 6px 18px;
background:rgba(255,255,255,.04);
border-radius:40px;
border:1px solid rgba(255,255,255,.05);
transition:all .35s cubic-bezier(.4,0,.2,1);
cursor:default;
position:relative;
}

#home .sticker-item::after{
content:'';
position:absolute;
inset:-1px;
border-radius:40px;
background:linear-gradient(135deg,var(--red-light),transparent);
opacity:0;
transition:opacity .4s;
z-index:-1;
}

#home .sticker-item:hover{
background:rgba(255,0,0,.08);
border-color:rgba(255,0,0,.2);
transform:translateY(-3px) scale(1.02);
box-shadow:0 8px 24px rgba(255,0,0,.08);
}

#home .sticker-item:hover::after{opacity:1}

#home .sticker-item i{
font-size:1.1rem;
width:28px;
height:28px;
display:flex;
align-items:center;
justify-content:center;
border-radius:50%;
background:rgba(255,0,0,.12);
color:#ff1c1c;
transition:all .4s cubic-bezier(.4,0,.2,1);
flex-shrink:0;
}

#home .sticker-item:hover i{
background:rgba(255,0,0,.25);
transform:scale(1.1) rotate(-8deg);
box-shadow:0 0 20px rgba(255,0,0,.15);
}

#home .sticker-item .label{
color:#e8e8e8;
font-weight:600;
font-size:.9rem;
letter-spacing:.3px;
}

#home .sticker-item .tag{
background:linear-gradient(135deg, rgba(255,0,0,.2), rgba(200,0,0,.1));
padding:2px 14px;
border-radius:30px;
font-size:.6rem;
font-weight:700;
color:#ff1c1c;
border:1px solid rgba(255,0,0,.15);
text-transform:uppercase;
letter-spacing:.5px;
transition:all .35s;
}

#home .sticker-item:hover .tag{
background:linear-gradient(135deg, rgba(255,0,0,.3), rgba(200,0,0,.2));
border-color:rgba(255,0,0,.3);
box-shadow:0 0 24px rgba(255,0,0,.08);
}

/* ===== بخش اصلی ===== */
main{
max-width:1100px;
margin:30px auto;
padding:0 15px;
position:relative;
z-index:1;
}

.page{
display:none;
animation:fadeSlide .6s cubic-bezier(.4,0,.2,1) forwards;
}

.page.active{display:block}

@keyframes fadeSlide{
0%{opacity:0;transform:translateY(30px)}
100%{opacity:1;transform:translateY(0)}
}

.section-card{
background:rgba(255,255,255,.04);
border:1px solid rgba(255,255,255,.08);
border-radius:24px;
padding:30px 32px;
backdrop-filter:blur(8px);
-webkit-backdrop-filter:blur(8px);
transition:all .4s;
position:relative;
overflow:hidden;
}

.section-card::before{
content:'';
position:absolute;
top:-50%;
right:-50%;
width:100%;
height:100%;
background:radial-gradient(circle at top right, rgba(255,0,0,.03), transparent 60%);
pointer-events:none;
}

.section-card:hover{
border-color:rgba(255,255,255,.12);
box-shadow:0 8px 40px rgba(0,0,0,.2);
}

.page-title{
text-align:center;
font-weight:900;
font-size:1.6rem;
margin-bottom:24px;
color:#ff1c1c;
letter-spacing:.5px;
position:relative;
padding-bottom:14px;
}

.page-title::after{
content:'';
position:absolute;
bottom:0;
left:50%;
transform:translateX(-50%);
width:60px;
height:3px;
background:linear-gradient(90deg,transparent,#ff1c1c,transparent);
border-radius:10px;
}

.page-title i{
margin-left:10px;
}

/* ===== شمارنده بازدید ===== */
.visitor-counter{
display:flex;
justify-content:center;
align-items:center;
gap:12px;
margin-top:15px;
padding:10px 20px;
background:rgba(255,255,255,.03);
border-radius:40px;
border:1px solid rgba(255,255,255,.05);
font-size:.75rem;
color:#666;
}

.visitor-counter i{
color:#ff1c1c;
}

.visitor-counter .count{
color:#fff;
font-weight:700;
font-size:.9rem;
}

/* ===== اعضا ===== */
.roles{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(260px,1fr));
gap:16px;
}

.role-box{
background:rgba(255,255,255,.03);
border:1px solid rgba(255,255,255,.08);
border-radius:16px;
padding:18px 20px;
transition:all .35s cubic-bezier(.4,0,.2,1);
position:relative;
overflow:hidden;
}

.role-box::before{
content:'';
position:absolute;
inset:0;
background:linear-gradient(135deg,var(--red-light),transparent 60%);
opacity:0;
transition:opacity .4s;
}

.role-box:hover{
transform:translateY(-4px) scale(1.01);
border-color:rgba(255,0,0,.15);
box-shadow:0 8px 30px rgba(0,0,0,.2);
}

.role-box:hover::before{opacity:1}

.role-title{
color:#ff1c1c;
font-weight:700;
margin-bottom:6px;
font-size:1.05rem;
position:relative;
z-index:1;
}

.role-box .name{
font-weight:600;
font-size:1rem;
color:#e0e0e0;
position:relative;
z-index:1;
}

.status-online{color:#17d36b;position:relative;z-index:1}
.status-offline{color:#ff4444;position:relative;z-index:1}
.status-removed{color:#ffaa00;position:relative;z-index:1}

/* ===== قوانین ===== */
.rules-list{
display:grid;
gap:14px;
}

.rule{
background:rgba(255,255,255,.03);
border:1px solid rgba(255,255,255,.08);
border-radius:16px;
padding:18px 22px;
transition:all .4s cubic-bezier(.4,0,.2,1);
cursor:default;
border-right:3px solid transparent;
position:relative;
overflow:hidden;
}

.rule::before{
content:'';
position:absolute;
inset:0;
background:linear-gradient(135deg,var(--red-light),transparent 70%);
opacity:0;
transition:opacity .4s;
}

.rule:hover{
background:rgba(255,0,0,.06);
border-color:rgba(255,0,0,.15);
border-right-color:#ff1c1c;
transform:translateX(-4px);
box-shadow:0 4px 28px rgba(0,0,0,.2);
}

.rule:hover::before{opacity:1}

.rule .num{
color:#ff1c1c;
font-weight:900;
font-size:1.05rem;
margin-left:10px;
font-family:'Vazirmatn',sans-serif;
position:relative;
z-index:1;
}

.rule .title{
font-weight:800;
color:#f0f0f0;
font-size:1rem;
font-family:'Vazirmatn',sans-serif;
position:relative;
z-index:1;
}

.rule .desc{
color:#b0b8c8;
font-size:.92rem;
margin-top:6px;
display:block;
font-family:'Vazirmatn',sans-serif;
line-height:2;
padding-right:36px;
position:relative;
z-index:1;
}

.rule .desc .hl{
color:#ff1c1c;
font-weight:600;
}

/* ===== افتخارات - خالی ===== */
.honors-empty{
text-align:center;
padding:40px 20px;
color:#888;
font-size:1.1rem;
letter-spacing:1px;
}

.honors-empty i{
font-size:3rem;
color:#333;
display:block;
margin-bottom:16px;
opacity:0.3;
animation:pulse 2s ease-in-out infinite;
}

.honors-empty .empty-line{
display:block;
width:60px;
height:2px;
background:linear-gradient(90deg,transparent,#444,transparent);
margin:12px auto;
}

/* ===== لوح تقدیر - لیست ===== */
.honor-list{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(260px,1fr));
gap:18px;
margin-bottom:25px;
}

.honor-item{
background:rgba(255,255,255,.03);
border:1px solid rgba(255,255,255,.08);
border-radius:18px;
padding:28px 20px;
text-align:center;
cursor:pointer;
transition:all .4s cubic-bezier(.4,0,.2,1);
position:relative;
overflow:hidden;
border-right:3px solid transparent;
}

.honor-item::before{
content:'';
position:absolute;
inset:0;
background:linear-gradient(135deg,rgba(255,0,0,.06),transparent);
opacity:0;
transition:opacity .4s;
}

.honor-item:hover{
transform:translateY(-5px);
border-color:rgba(255,0,0,.2);
border-right-color:#ff1c1c;
box-shadow:0 8px 40px rgba(0,0,0,.25), 0 0 40px rgba(255,0,0,.03);
}

.honor-item:hover::before{opacity:1}

.honor-item .avatar{
width:70px;
height:70px;
border-radius:50%;
margin:0 auto 12px;
padding:4px;
background:linear-gradient(135deg,#ff1c1c,#8a0000,#ff1c1c);
box-shadow:0 0 0 2px #1a1a1a,0 0 0 4px #ff1c1c,0 0 30px rgba(255,0,0,.1);
transition:all .4s;
}

.honor-item:hover .avatar{
transform:scale(1.05);
box-shadow:0 0 0 2px #1a1a1a,0 0 0 4px #ff1c1c,0 0 50px rgba(255,0,0,.2);
}

.honor-item .avatar img{
width:100%;
height:100%;
object-fit:cover;
border-radius:50%;
display:block;
background:#111;
}

.honor-item .h-name{
font-size:1.3rem;
font-weight:800;
color:#fff;
font-family:'Noto Naskh Arabic',serif;
margin-bottom:2px;
}

.honor-item .h-role{
font-size:.85rem;
color:#aaa;
font-weight:300;
letter-spacing:1px;
}

.honor-item .h-badge{
display:inline-block;
margin-top:10px;
padding:3px 18px;
border-radius:30px;
font-size:.7rem;
font-weight:700;
color:#ff1c1c;
border:1px solid rgba(255,0,0,.15);
background:rgba(255,0,0,.05);
letter-spacing:1px;
}

.honor-item .arrow{
display:block;
margin-top:14px;
color:#555;
font-size:.8rem;
transition:all .3s;
opacity:0.5;
}

.honor-item:hover .arrow{
color:#ff1c1c;
transform:translateX(-5px);
opacity:1;
}

/* ===== لوح تقدیر - جزئیات ===== */
.honor-detail{
display:none;
animation:fadeSlide .5s cubic-bezier(.4,0,.2,1) forwards;
}

.honor-detail.active{display:block}

.honor-detail .back-btn{
display:inline-flex;
align-items:center;
gap:8px;
background:rgba(255,255,255,.05);
border:1px solid rgba(255,255,255,.08);
padding:8px 20px;
border-radius:40px;
color:#aaa;
cursor:pointer;
transition:all .3s;
font-size:.9rem;
margin-bottom:20px;
}

.honor-detail .back-btn:hover{
background:rgba(255,255,255,.08);
color:#fff;
transform:translateX(-3px);
}

/* ===== لوح تقدیر - خود لوح ===== */
#honor .certificate{
max-width:900px;
width:100%;
background:linear-gradient(145deg,#0a0a0a,#150505);
padding:50px 45px 40px 45px;
border-radius:24px;
box-shadow: 
0 40px 100px rgba(0,0,0,0.95),
0 0 0 1px #2a2a2a,
0 0 0 3px #ff1c1c,
0 0 0 7px #1a1a1a,
0 0 0 9px #ff1c1c,
inset 0 0 80px rgba(255,0,0,.05);
position:relative;
transition:all .4s ease;
margin:0 auto;
}

#honor .certificate::before{
content:'';
position:absolute;
top:20px;
left:20px;
right:20px;
bottom:20px;
border:1px solid rgba(255,0,0,.15);
border-radius:16px;
pointer-events:none;
}

#honor .certificate::after{
content:'✦ ✦ ✦';
position:absolute;
top:-12px;
left:50%;
transform:translateX(-50%);
font-size:16px;
color:#ff1c1c;
letter-spacing:12px;
background:#0a0a0a;
padding:0 20px;
opacity:0.6;
}

#honor .top-section{
display:flex;
align-items:center;
justify-content:space-between;
gap:30px;
margin-bottom:18px;
flex-wrap:wrap;
}

#honor .header{
flex:2;
text-align:right;
}

#honor .header .badge{
font-size:13px;
color:#ff1c1c;
letter-spacing:4px;
font-weight:300;
opacity:0.7;
margin-bottom:2px;
}

#honor .header h1{
font-size:32px;
font-weight:700;
color:#fff;
letter-spacing:6px;
text-shadow:0 0 40px rgba(255,0,0,.1);
margin-bottom:2px;
font-family:'Noto Naskh Arabic',serif;
}

#honor .header .sub{
font-size:16px;
color:#888;
font-weight:300;
border-bottom:1px solid rgba(255,0,0,.2);
padding-bottom:6px;
display:inline-block;
letter-spacing:2px;
}

#honor .gold-line{
width:80px;
height:2px;
background:linear-gradient(90deg,#ff1c1c,#ff6666,#ff1c1c);
margin:8px 0 4px 0;
border-radius:2px;
}

#honor .photo-wrapper{
flex:0 0 170px;
max-width:170px;
display:flex;
justify-content:center;
align-items:center;
}

#honor .photo-frame{
width:100%;
aspect-ratio:1/1;
border-radius:50%;
padding:5px;
background:linear-gradient(135deg,#ff1c1c,#8a0000,#ff1c1c);
box-shadow:0 0 0 2px #1a1a1a,0 0 0 5px #ff1c1c,0 0 50px rgba(255,0,0,.15);
position:relative;
transition:all .5s ease;
overflow:hidden;
}

#honor .photo-frame:hover{
transform:scale(1.02);
box-shadow:0 0 0 2px #1a1a1a,0 0 0 5px #ff1c1c,0 0 70px rgba(255,0,0,.25);
}

#honor .photo-frame img{
width:100%;
height:100%;
object-fit:cover;
border-radius:50%;
display:block;
filter:grayscale(0.2) brightness(0.95) contrast(1.05);
transition:all .5s ease;
border:2px solid rgba(255,0,0,.2);
}

#honor .photo-frame img:hover{
filter:grayscale(0) brightness(1) contrast(1.1);
}

#honor .photo-frame::after{
content:'◆';
position:absolute;
bottom:-4px;
right:-4px;
font-size:20px;
color:#ff1c1c;
opacity:0.6;
animation:sparkle 3s ease-in-out infinite;
}

@keyframes sparkle{
0%,100%{opacity:0.3;transform:scale(0.8) rotate(0deg)}
50%{opacity:1;transform:scale(1.2) rotate(45deg)}
}

#honor .body-text{
text-align:center;
padding:5px 5px 0 5px;
}

#honor .body-text .to{
font-size:17px;
color:#666;
font-weight:300;
letter-spacing:3px;
margin-bottom:2px;
}

#honor .body-text .name{
font-size:48px;
font-weight:700;
margin:2px 0;
letter-spacing:5px;
text-shadow:0 0 50px rgba(255,0,0,.08);
font-family:'Noto Naskh Arabic',serif;
}

#honor .body-text .name .highlight-name{
background:linear-gradient(135deg,#fff,#ff6666,#ff1c1c);
-webkit-background-clip:text;
-webkit-text-fill-color:transparent;
background-clip:text;
}

#honor .body-text .role{
font-size:17px;
color:#ff1c1c;
font-weight:300;
display:inline-block;
padding:3px 30px;
border:1px solid rgba(255,0,0,.15);
border-radius:30px;
letter-spacing:2px;
margin:3px 0 10px 0;
background:rgba(255,0,0,.03);
}

#honor .body-text .message{
font-size:18px;
line-height:2.4;
color:#aaa;
max-width:780px;
margin:10px auto;
padding:20px 28px;
background:rgba(255,255,255,0.015);
border-radius:14px;
border-right:2px solid rgba(255,0,0,.15);
border-left:2px solid rgba(255,0,0,.15);
font-family:'Noto Naskh Arabic',serif;
}

#honor .body-text .message .greeting{
font-size:20px;
color:#ff6666;
font-weight:700;
display:block;
margin-bottom:6px;
}

#honor .body-text .message .highlight{
color:#ff6666;
font-weight:700;
font-size:19px;
}

#honor .body-text .message .gold-text{
color:#ff1c1c;
font-weight:700;
}

#honor .body-text .message .heart{
color:#ff1c1c;
font-size:20px;
}

#honor .body-text .message .closing{
color:#ff1c1c;
font-size:19px;
font-weight:700;
letter-spacing:2px;
display:block;
margin-top:8px;
}

#honor .body-text .message .line-break{
display:block;
width:60px;
height:1px;
background:linear-gradient(90deg,transparent,#ff1c1c,transparent);
margin:10px auto;
opacity:0.3;
}

#honor .footer{
display:flex;
justify-content:space-between;
align-items:flex-end;
margin-top:22px;
padding-top:18px;
border-top:1px solid rgba(255,0,0,.15);
flex-wrap:wrap;
gap:15px;
}

#honor .footer .signature{
text-align:right;
}

#honor .footer .signature .label{
font-size:12px;
color:#444;
font-weight:300;
letter-spacing:3px;
text-transform:uppercase;
opacity:0.5;
}

#honor .footer .signature .sig-name{
font-size:30px;
font-weight:700;
color:#fff;
letter-spacing:1px;
text-shadow:0 0 30px rgba(255,0,0,.05);
font-family:'Noto Naskh Arabic',serif;
}

#honor .footer .signature .sig-name .hash{
font-size:26px;
color:#ff1c1c;
}

#honor .footer .signature .sig-sub{
font-size:14px;
color:#888;
font-weight:300;
border-bottom:1px dotted rgba(255,0,0,.15);
padding-bottom:2px;
letter-spacing:2px;
}

#honor .footer .date{
text-align:left;
}

#honor .footer .date .label{
font-size:12px;
color:#444;
font-weight:300;
letter-spacing:3px;
text-transform:uppercase;
opacity:0.5;
}

#honor .footer .date .date-val{
font-size:20px;
font-weight:700;
color:#fff;
letter-spacing:2px;
font-family:'Noto Naskh Arabic',serif;
}

#honor .footer .date .team-name{
font-size:18px;
font-weight:700;
color:#ff1c1c;
letter-spacing:3px;
opacity:0.8;
font-family:'Noto Naskh Arabic',serif;
}

/* ===== پشتیبانی ===== */
.support-intro{
background:rgba(255,255,255,.03);
border:1px solid rgba(255,255,255,.08);
border-radius:18px;
padding:24px 28px;
margin-bottom:20px;
line-height:2.3;
color:#ccc;
font-size:1.05rem;
transition:all .4s;
}

.support-intro:hover{
border-color:rgba(255,0,0,.15);
box-shadow:0 4px 24px rgba(0,0,0,.15);
}

.support-intro strong{
color:#ff1c1c;
font-weight:800;
}

.support-intro .book{
display:block;
border-right:3px solid #ff1c1c;
padding-right:18px;
margin-top:12px;
font-style:italic;
color:#aaa;
font-size:.98rem;
}

.lang{
background:rgba(255,255,255,.03);
border:1px solid rgba(255,255,255,.08);
border-radius:14px;
padding:14px 18px;
margin-bottom:12px;
transition:all .3s;
font-size:.92rem;
color:#bbb;
}

.lang:hover{
border-color:rgba(255,255,255,.12);
background:rgba(255,255,255,.05);
}

/* ===== دکمه پشتیبانی (با جاوااسکریپت) ===== */
.support-btn{
display:inline-block;
margin-top:18px;
background:linear-gradient(135deg,#ff1c1c,#8a0000);
padding:14px 32px;
border-radius:14px;
border:none;
color:#fff;
font-weight:700;
font-size:.95rem;
transition:all .4s cubic-bezier(.4,0,.2,1);
position:relative;
overflow:hidden;
box-shadow:0 4px 20px rgba(255,0,0,.15);
cursor:pointer;
font-family:'Vazirmatn',sans-serif;
width:auto;
}

.support-btn::before{
content:'';
position:absolute;
inset:0;
background:linear-gradient(135deg,rgba(255,255,255,.1),transparent);
opacity:0;
transition:opacity .4s;
}

.support-btn:hover{
transform:translateY(-3px) scale(1.02);
box-shadow:0 8px 40px rgba(255,0,0,.25);
}

.support-btn:hover::before{opacity:1}

.support-btn i{
margin-left:8px;
}

/* ===== فوتر ===== */
footer{
text-align:center;
color:#555;
padding:30px;
font-size:.85rem;
border-top:1px solid rgba(255,0,0,.15);
margin-top:20px;
position:relative;
z-index:1;
}

footer span{color:#ff1c1c;font-weight:700}

footer .footer-info{
display:flex;
justify-content:center;
flex-wrap:wrap;
gap:8px 25px;
margin-top:6px;
font-size:.75rem;
color:#444;
}

footer .footer-info i{
color:#ff1c1c;
margin-left:4px;
}

/* ===== ریسپانسیو ===== */
@media(max-width:768px){

#home .hero-timer{
grid-template-columns:repeat(3,1fr);
gap:10px;
}

#home .time-num{font-size:1.3rem}

nav a{
padding:8px 14px;
font-size:.8rem;
}

#home .sticker-row{
padding:14px 18px;
gap:10px 14px;
border-radius:40px;
}

#home .sticker-item{
padding:4px 12px 4px 14px;
font-size:.8rem;
}

.rule .desc{padding-right:0}
.section-card{padding:22px 18px}
.page-title{font-size:1.3rem}
.support-intro{font-size:.95rem;padding:18px}

#honor .certificate{padding:30px 18px 22px 18px}
#honor .top-section{flex-direction:column;align-items:center;text-align:center;gap:15px}
#honor .header{text-align:center}
#honor .header h1{font-size:24px;letter-spacing:4px}
#honor .gold-line{margin:6px auto}
#honor .photo-wrapper{flex:0 0 130px;max-width:130px}
#honor .body-text .name{font-size:32px;letter-spacing:3px}
#honor .body-text .message{font-size:16px;line-height:2.2;padding:14px 16px}
#honor .footer{flex-direction:column;align-items:center;text-align:center;gap:10px}
#honor .footer .signature{text-align:center}
#honor .footer .date{text-align:center}
#honor .certificate::after{font-size:12px;letter-spacing:8px;top:-10px;padding:0 12px}

.honor-list{grid-template-columns:1fr}

#scrollTop{
width:42px;
height:42px;
font-size:1rem;
bottom:20px;
right:20px;
}

}

@media(max-width:480px){

#home .hero-timer{
grid-template-columns:repeat(2,1fr);
gap:8px;
}

#home .time-num{font-size:1.1rem}

.page-title{font-size:1.2rem}
.section-card{padding:16px 14px}

#home .sticker-row{
padding:10px 12px;
gap:6px 10px;
border-radius:30px;
flex-wrap:wrap;
}

#home .sticker-item{
padding:3px 10px 3px 12px;
font-size:.7rem;
border-radius:30px;
}

#home .sticker-item i{
width:20px;
height:20px;
font-size:.7rem;
}

#home .sticker-item .tag{
font-size:.5rem;
padding:1px 8px;
}

.rule{
padding:14px 16px;
}

.rule .num{font-size:.9rem}
.rule .title{font-size:.9rem}
.rule .desc{font-size:.82rem;line-height:1.9;padding-right:0}

.support-intro{font-size:.88rem;padding:14px 16px;line-height:2}
.support-btn{padding:12px 24px;font-size:.85rem}

#honor .body-text .name{font-size:26px}
#honor .body-text .role{font-size:14px;padding:2px 16px}
#honor .body-text .message{font-size:14px;line-height:2;padding:10px 12px}
#honor .footer .signature .sig-name{font-size:24px}
#honor .photo-wrapper{flex:0 0 100px;max-width:100px}

}

</style>
</head>

<body>

<!-- ===== لودینگ ===== -->
<div id="loader">
<div class="spinner"></div>
<p>بارگذاری...</p>
</div>

<!-- ===== ذرات ===== -->
<div class="particles" id="particles"></div>

<!-- ===== اورب‌ها ===== -->
<div class="bg-orb orb1"></div>
<div class="bg-orb orb2"></div>
<div class="bg-orb orb3"></div>

<!-- ===== دکمه رفتن به بالا ===== -->
<button id="scrollTop" onclick="window.scrollTo({top:0,behavior:'smooth'})">
<i class="fas fa-chevron-up"></i>
</button>

<header>

<div class="topbar">

<div class="header-top">
<div class="brand">𝑪𝒐𝒅 𝑶𝒇 <span>𝑱𝒖𝒔𝒕𝒊𝒄𝒆</span> ⚖️</div>
</div>

<nav>
<ul>
<li><a class="active" data-page="home">خانه</a></li>
<li><a data-page="members">اعضا</a></li>
<li><a data-page="rules">قوانین</a></li>
<li><a data-page="honors">افتخارات</a></li>
<li><a data-page="honor">لوح تقدیر</a></li>
<li><a data-page="about">درباره</a></li>
<li><a data-page="support"><i class="fas fa-headphones"></i> پشتیبانی</a></li>
</ul>
</nav>

</div>

</header>

<main>

<!-- ===== صفحه خانه ===== -->
<section id="home" class="page active">
<div class="section-card">
<div class="page-title">داشبورد اصلی</div>
<p style="text-align:center;color:#aaa;margin-bottom:10px;">به مرکز فرماندهی <span style="color:#ff1c1c;font-weight:700;">𝑪𝒐𝒅 𝑶𝒇 𝑱𝒖𝒔𝒕𝒊𝒄𝒆</span> خوش آمدید</p>

<div class="hero-timer">
<div class="time-box"><div id="y" class="time-num">۰</div><span class="label">سال</span></div>
<div class="time-box"><div id="d" class="time-num">۰</div><span class="label">روز</span></div>
<div class="time-box"><div id="h" class="time-num">۰</div><span class="label">ساعت</span></div>
<div class="time-box"><div id="m" class="time-num">۰</div><span class="label">دقیقه</span></div>
<div class="time-box"><div id="s" class="time-num">۰</div><span class="label">ثانیه</span></div>
</div>

<div class="sticker-row">
<div class="sticker-item"><i class="fas fa-gavel"></i><span class="label">عدالت</span><span class="tag">فعال</span></div>
<div class="sticker-item"><i class="fas fa-shield-halved"></i><span class="label">امنیت</span><span class="tag">پایدار</span></div>
<div class="sticker-item"><i class="fas fa-bolt"></i><span class="label">سرعت</span><span class="tag">بی‌نظیر</span></div>
<div class="sticker-item"><i class="fas fa-crown"></i><span class="label">کیفیت</span><span class="tag">عالی</span></div>
<div class="sticker-item"><i class="fas fa-code"></i><span class="label">کد</span><span class="tag">تمیز</span></div>
</div>

<!-- ===== شمارنده بازدید ===== -->
<div class="visitor-counter">
<i class="fas fa-eye"></i>
<span>بازدید:</span>
<span class="count" id="visitorCount">۰</span>
</div>

</div>
</section>

<!-- ===== صفحه اعضا ===== -->
<section id="members" class="page">
<div class="section-card">
<div class="page-title"><i class="fas fa-users"></i> اعضای گارد</div>

<div class="roles">

<div class="role-box">
<div class="role-title">👑 رهبر</div>
<div class="name">𝙷𝙾𝙼𝙴𝙻𝙰𝙽𝙳𝙴𝚁</div>
<span class="status-online">✅ فعال</span>
</div>

<div class="role-box">
<div class="role-title">⚜ جانشین</div>
<div class="name">𝐷𝓪ᴿ𝖐𝒩ᴱ𝑠𝑠</div>
<span class="status-online">✅ فعال</span>
</div>

<div class="role-box">
<div class="role-title">🛡 معاون ارشد</div>
<div class="name">خانوم doctor 806</div>
<span class="status-offline">❌ آفلاین</span>
</div>

<div class="role-box">
<div class="role-title">🧭 معاون</div>
<div class="name">𝘿𝙚𝙧𝙞𝙡</div>
<span class="status-online">✅ فعال</span>
</div>

<div class="role-box">
<div class="role-title">🎓 مربی</div>
<div class="name" style="color:#888;">به زودی اضافه می‌شود</div>
</div>

<div class="role-box">
<div class="role-title">⚔ اتکر</div>
<div class="name" style="color:#888;">به زودی اضافه می‌شود</div>
</div>

<div class="role-box">
<div class="role-title">👤 عضو عادی</div>
<div class="name" style="color:#888;">به زودی اضافه می‌شود</div>
</div>

</div>

<br>

<div style="color:#aaa;font-size:.95rem;line-height:2.2;background:rgba(255,255,255,.02);border-radius:14px;padding:18px 22px;border:1px solid rgba(255,255,255,.08);font-weight:400;">
<span style="color:#17d36b;font-weight:700;">✅</span> افراد دارای تیک سبز → عضو فعال گارد هستند &nbsp;|&nbsp;
<span style="color:#ff4444;font-weight:700;">❌</span> افراد دارای ضربدر → از گارد خارج شده‌اند &nbsp;|&nbsp;
<span style="color:#ffaa00;font-weight:700;">⚠</span> افراد دارای علامت → از گارد حذف شده‌اند
<br><br>
<span style="color:#ff1c1c;font-weight:700;">⏺</span> افرادی که <span style="color:#17d36b;">آنلاین</span> هستند یعنی داخل گارد حضور دارند  
<span style="color:#ff1c1c;font-weight:700;">⏺</span> افرادی که <span style="color:#ff4444;">آفلاین</span> هستند یعنی از گارد خارج شده‌اند
</div>

</div>
</section>

<!-- ===== صفحه قوانین ===== -->
<section id="rules" class="page">
<div class="section-card">
<div class="page-title"><i class="fas fa-book-open"></i> قوانین کد عدالت</div>

<div class="rules-list">
<div class="rule"><span class="num">1.</span><span class="title">سکوت مطلق ⚠️</span><span class="desc">هرآنچه در تیم دیده، شنیده یا انجام می‌دهی، به هیچ‌کس بیرون از تیم منتقل نمی‌شود. «حرفی از اینجا بیرون نرود» یک شعار نیست، یک <span class="hl">اصل بقاست</span>.</span></div>
<div class="rule"><span class="num">2.</span><span class="title">هویت واقعی ممنوع ⚠️</span><span class="desc">هیچ‌کس حق ندارد نام واقعی، شهر، شماره یا هر اطلاعاتی که به زندگی فیزیکی اعضا مربوط می‌شود را در کانال‌های داخلی فاش کند یا درباره‌اش کنجکاوی نماید. هر عضو فقط با <span class="hl">شناسه و لقب</span> شناخته می‌شود.</span></div>
<div class="rule"><span class="num">3.</span><span class="title">بحث سیاسی مطلقاً ممنوع ⚠️</span><span class="desc">بحث درباره جریان‌ها، احزاب، افراد سیاسی، انتخابات و هرگونه تحلیل جهت‌دار سیاسی در تمام بسترهای تیم ممنوع است. تیم یک <span class="hl">ابزار فنی</span> است، نه تریبون.</span></div>
<div class="rule"><span class="num">4.</span><span class="title">بی‌احترامی به مقامات ممنوع ⚠️</span><span class="desc">توهین، استهزا یا انتشار محتوای بی‌احترامانه نسبت به هر مقام رسمی تیم ما یعنی <span class="hl">کد عدالت</span>، در هر بستری که به تیم ارتباط داشته باشد، خط قرمز است و با اخراج فوری همراه خواهد بود.</span></div>
<div class="rule"><span class="num">5.</span><span class="title">محتوای آموزشی درون‌تیمی بماند ⚠️</span><span class="desc">تمامی آموزش‌ها، ماژول‌ها، ابزارها، آسیب‌پذیری‌های کشف‌شده و مستندات فنی، دارایی اختصاصی تیم محسوب می‌شود. در اختیار گذاشتن حتی یک خط از آن برای افراد خارج از تیم، <span class="hl">خیانت</span> تلقی می‌گردد.</span></div>
<div class="rule"><span class="num">6.</span><span class="title">اصل «نیاز به دانستن» ⚠️</span><span class="desc">هر عضو دانستنش ضروری است و حتما باید آموزشات رو مطالعه کنه و اگر حضور الکی در تیم داشت و از آموزشات عقب موند <span class="hl">اخطار</span> خواهد گرفت.</span></div>
<div class="rule"><span class="num">7.</span><span class="title">مقدار اخطارها ⚠️</span><span class="desc">هر عضو سر <span class="hl">۴ اخطار</span> از تیم محروم میشود. زمان محرومیت بستگی به جرم شما دارد (۱ روز، ۲ روز، دائمی).</span></div>
<div class="rule"><span class="num">8.</span><span class="title">ممنوعیت انجام عملیات شخصی با نام تیم ⚠️</span><span class="desc">هیچ‌کس اجازه ندارد از ابزارها، دسترسی‌ها یا نام تیم برای تسویه حساب شخصی، کنجکاوی خصوصی یا منافع مالی فردی استفاده کند. هر عملیات باید با <span class="hl">مجوز رسمی تیم</span> آغاز شود.</span></div>
<div class="rule"><span class="num">9.</span><span class="title">عدم اجرای ابزار روی اعضا ⚠️</span><span class="desc">استفاده از بدافزار، رات، هکینگ یا هر روش تهاجمی علیه اعضای خود تیم یا برای تست بدون رضایت روی دستگاه اعضا ممنوع است. <span class="hl">اعتماد داخلی</span> خط قرمز است.</span></div>
<div class="rule"><span class="num">10.</span><span class="title">انکارپذیری ساختاری ⚠️</span><span class="desc">هر پروژه باید به‌گونه‌ای طراحی شود که در صورت افشا، نتوان آن را به تک‌تک اعضا یا هسته اصلی تیم نسبت داد. از کدهای امضاشده با نام مستعار و <span class="hl">زنجیره‌های پروکسی</span> چندلایه استفاده شود.</span></div>
<div class="rule"><span class="num">11.</span><span class="title">به‌روزرسانی اجباری دانش ⚠️</span><span class="desc">عضو موظف است هفتگی حداقل یکبار رات های آموزش دیده شده رو مجدد به پیوی معاون آموزشی ارسال کند در غیر اینصورت <span class="hl">اخطار</span> خواهید گرفت.</span></div>
<div class="rule"><span class="num">12.</span><span class="title">افشای غیرمجاز ⚠️</span><span class="desc">اگر فردی یا عضوی از تیم دیگری را بدون مجوز از رهبر و خالق تیم افشا کنید، رسما اشتباه بزرگی مرتکب شدید و <span class="hl">مجازات سنگینی</span> میشوید.</span></div>
<div class="rule"><span class="num">13.</span><span class="title">هوشیاری در برابر مهندسی اجتماعی ⚠️</span><span class="desc">اگر فردی حتی با نشان دادن اطلاعات داخلی سعی در نزدیک شدن به تو داشت، فوراً آن را به مسئول امنیت تیم گزارش بده. نزار هرکس که جدید می‌آید باهات خیلی گرم بگیره و ازت اطلاعات بکشه ⚠️</span></div>
<div class="rule"><span class="num">14.</span><span class="title">فوریت در گزارش نفوذ ⚠️</span><span class="desc">اگر عضوی کوچک‌ترین ظن به آلودگی سیستم‌ش، سرقت کلید یا شنود ارتباطات داشت، موظف است ظرف <span class="hl">۱۰ دقیقه</span> به هسته مرکزی تیم اطلاع دهد، حتی اگر نیمه‌شب باشد. تأخیر، مساوی با فاجعه است. ⚠️</span></div>
<div class="rule"><span class="num">15.</span><span class="title">ارتباط گرفتن با دشمن ⚠️</span><span class="desc">با دشمن‌هامون ارتباط خاصی نگیرید و گرم نگیرید بعد بگیرد اجتماعی هستم، <span class="hl">سرد</span> رفتار کنین و دیر سین بزنین تا روانی شه. چه دشمن‌هامون چه کسانی که می‌گن متحدیم، متحد خودش می‌آید پیوی رهبر نه افراد معمولی و معاونین ⚠️</span></div>
<div class="rule"><span class="num">16.</span><span class="title">تصمیم شورا ⚠️</span><span class="desc">قوانین با تصمیم شورا به روز میشود و همه موظف به اجرای نسخه جدید هستند ⚠️</span></div>
<div class="rule"><span class="num">17.</span><span class="title">غیبت ⚠️</span><span class="desc">در صورت غیبت طولانی فرد باید دلیل موجه ارائه کند و هماهنگ باشد ⚠️</span></div>
<div class="rule"><span class="num">18.</span><span class="title">شایعه یا تخریب ⚠️</span><span class="desc">شایعه پراکنی، ایجاد اختلاف یا تخریب دیگران ممنوع است ⚠️</span></div>
<div class="rule"><span class="num">19.</span><span class="title">حضور الزامی در جلسه ⚠️</span><span class="desc">حضور منظم در جلسات و فعالیت‌های رسمی برای اعضای مسئول ضروری است ⚠️</span></div>
<div class="rule"><span class="num">20.</span><span class="title">فضای امن محترمانه ⚠️</span><span class="desc">اعضا باید فضای امن، محترمانه و قابل اعتماد در مجموعه ایجاد کنند ⚠️</span></div>
</div>

</div>
</section>

<!-- ===== صفحه افتخارات ===== -->
<section id="honors" class="page">
<div class="section-card">
<div class="page-title"><i class="fas fa-trophy"></i> افتخارات</div>

<div class="honors-empty">
<i class="fas fa-trophy"></i>
<span>هیچ افتخاری هنوز وارد نشده</span>
<span class="empty-line"></span>
<span style="font-size:.8rem;color:#555;">به زودی...</span>
</div>

</div>
</section>

<!-- ===== صفحه لوح تقدیر ===== -->
<section id="honor" class="page">
<div class="section-card">
<div class="page-title"><i class="fas fa-award"></i> لوح تقدیر</div>

<div id="honorList" class="honor-list">
<div class="honor-item" onclick="showHonor('doctor806')">
<div class="avatar"><img src="data:image/svg+xml,%3Csvg xmlns=%22http://www.w3.org/2000/svg%22 width=%22300%22 height=%22300%22%3E%3Crect fill=%22%23111111%22 width=%22300%22 height=%22300%22/%3E%3Ctext x=%2250%25%22 y=%2250%25%22 text-anchor=%22middle%22 dy=%22.3em%22 font-size=%2260%22 fill=%22%23ff1c1c%22 font-family=%22sans-serif%22%3E◆%3C/text%3E%3C/svg%3E" alt="doctor806"></div>
<div class="h-name">خانوم doctor 806</div>
<div class="h-role">✦ معاون ارشد تیم ✦</div>
<span class="h-badge">🏅 لوح افتخار</span>
<span class="arrow">◀ کلیک کنید</span>
</div>
</div>

<div id="honorDetail" class="honor-detail">
<button class="back-btn" onclick="backToHonorList()"><i class="fas fa-arrow-right"></i> بازگشت به لیست</button>
<div id="certificateContainer"></div>
</div>

</div>
</section>

<!-- ===== صفحه درباره ===== -->
<section id="about" class="page">
<div class="section-card">
<div class="page-title"><i class="fas fa-info-circle"></i> درباره ما</div>
<p style="color:#ccc;font-size:1.05rem;line-height:2.2;">درحال تکمیل...</p>
</div>
</section>

<!-- ===== صفحه پشتیبانی ===== -->
<section id="support" class="page">
<div class="section-card">

<div class="page-title"><i class="fas fa-headphones"></i> پشتیبانی</div>

<div class="support-intro">
<strong>《 کد عدالت 》</strong> همواره پشتیبان اعضای خود بوده است.
<br>
اگر در حین استفاده از ابزارها، آموزش‌ها یا هر بخش از مجموعه با <strong>مشکل فنی، باگ، خطا یا ابهامی</strong> مواجه شدید، تیم پشتیبانی در کنار شماست.
<br><br>
<strong>🔰 خط‌مشاوره:</strong>
<br>
• گزارش‌ها به‌صورت <strong>محرمانه</strong> بررسی می‌شوند.
<br>
• تیم پشتیبانی متشکل از <strong>متخصصین</strong> هسته مرکزی است.
<br>
• پاسخگویی در <strong>کمترین زمان ممکن</strong> انجام می‌پذیرد.
<br>
<span class="book">« هر باگ، یک قدم به سوی کمال است. گزارش تو، بخشی از رشد ماست. »</span>
</div>

<div class="lang">🇬🇧 For bug reports or technical issues, reach out to our support team through the button below. We're here 24/7.</div>
<div class="lang">🇩🇪 Für Fehlerberichte oder technische Probleme kontaktiere unser Support-Team über den untenstehenden Button. Wir sind rund um die Uhr für dich da.</div>

<!-- ===== دکمه پشتیبانی ===== -->
<button onclick="openSupport()" class="support-btn" id="supportBtn">
<i class="fas fa-headset"></i> ارسال پیام به پشتیبانی
</button>

</div>
</section>

</main>

<footer>
<span>𝑪𝒐𝒅 𝑶𝒇 𝑱𝒖𝒔𝒕𝒊𝒄𝒆</span> © <span id="year"></span>
<div class="footer-info">
<span><i class="fas fa-shield-alt"></i> امنیت بالا</span>
<span><i class="fas fa-bolt"></i> سرعت بی‌نظیر</span>
<span><i class="fas fa-code"></i> کد تمیز</span>
</div>
</footer>

<script>

// ===== لودینگ =====
window.addEventListener('load', function() {
setTimeout(function() {
document.getElementById('loader').classList.add('hide');
}, 800);
});

// ===== سال =====
document.getElementById("year").textContent = new Date().getFullYear();

// ===== تایمر =====
const start = Date.now();

function p(n){
return String(n).padStart(2,"0").replace(/\d/g,d=>"۰۱۲۳۴۵۶۷۸۹"[d]);
}

function updateWithAnim(el, newVal) {
if(el.textContent !== newVal) {
el.textContent = newVal;
el.classList.remove('number-flash');
void el.offsetWidth;
el.classList.add('number-flash');
}
}

function timer(){
const e = Math.floor((Date.now() - start) / 1000);
const y = Math.floor(e / 31536000);
const d = Math.floor((e % 31536000) / 86400);
const h = Math.floor((e % 86400) / 3600);
const m = Math.floor((e % 3600) / 60);
const s = e % 60;

updateWithAnim(yEl, p(y));
updateWithAnim(dEl, p(d));
updateWithAnim(hEl, p(h));
updateWithAnim(mEl, p(m));
updateWithAnim(sEl, p(s));
}

const yEl = document.getElementById("y");
const dEl = document.getElementById("d");
const hEl = document.getElementById("h");
const mEl = document.getElementById("m");
const sEl = document.getElementById("s");

setInterval(timer, 1000);
timer();

// ===== ناوبری =====
document.querySelectorAll("nav a").forEach(a => {
a.onclick = e => {
e.preventDefault();

document.querySelectorAll(".page").forEach(p => p.classList.remove("active"));
document.querySelectorAll("nav a").forEach(n => n.classList.remove("active"));

document.getElementById(a.dataset.page).classList.add("active");
a.classList.add("active");

if(a.dataset.page === "honor") {
document.getElementById("honorList").style.display = "grid";
document.getElementById("honorDetail").classList.remove("active");
}
}
});

// ===== ذرات =====
(function createParticles() {
const container = document.getElementById('particles');
const sizes = [2,3,4,5,6];
for(let i = 0; i < 35; i++) {
const p = document.createElement('div');
p.className = 'particle';
p.style.left = Math.random() * 100 + '%';
const size = sizes[Math.floor(Math.random() * sizes.length)];
p.style.width = size + 'px';
p.style.height = size + 'px';
p.style.animationDuration = (10 + Math.random() * 20) + 's';
p.style.animationDelay = (Math.random() * 12) + 's';
p.style.opacity = 0.1 + Math.random() * 0.5;
container.appendChild(p);
}
})();

// ===== دکمه رفتن به بالا =====
const scrollBtn = document.getElementById('scrollTop');

window.addEventListener('scroll', function() {
if(window.scrollY > 300) {
scrollBtn.classList.add('visible');
} else {
scrollBtn.classList.remove('visible');
}
});

// ===== شمارنده بازدید =====
let visitCount = localStorage.getItem('visitCount') || 0;
visitCount = parseInt(visitCount) + 1;
localStorage.setItem('visitCount', visitCount);

function toPersianNum(num) {
return String(num).replace(/\d/g, d => "۰۱۲۳۴۵۶۷۸۹"[d]);
}
document.getElementById('visitorCount').textContent = toPersianNum(visitCount);

// ===== باز کردن لینک پشتیبانی =====
function openSupport() {
// تلاش با روش‌های مختلف
try {
// روش اول: باز کردن در تب جدید
window.open('https://splus.ir/My_id_darkness', '_blank');
} catch(e) {
try {
// روش دوم: تغییر مکان صفحه
window.location.href = 'https://splus.ir/My_id_darkness';
} catch(e2) {
// روش سوم: نمایش پیام
alert('لطفا به صورت دستی به آدرس زیر بروید:\nhttps://splus.ir/My_id_darkness');
}
}
}

// ===== داده‌های لوح =====
const honorData = {
doctor806: {
name: "خانوم doctor 806",
role: "✦ معاون ارشد 𝑪𝒐𝒅 𝑶𝒇 𝑱𝒖𝒔𝒕𝒊𝒄𝒆 ✦",
greeting: "✨ ای بانوی ارزشمند و بی‌نظیر ✨",
message1: "تو در میان ما، نه فقط یک همراه، که نورِ مسیر بودی.",
message2: "هر روزی که با تو سپری شد، درخشان‌تر از روز پیش بود",
message3: "و هر گامی که در کنارت برداشتیم، پر از برکت و افتخار.",
message4: "♥ حضور تو، گرمای بی‌بدیل تیم بود ♥",
message5: "دل‌های ما برای همیشه، میهمان خاطرات شیرین توست.",
message6: "در هر لحظه، یادت را در قلب‌هایمان زنده نگه می‌داریم.",
closing: "✦ یادت همیشه در قلب‌ها جاریست ✦",
signature: "𝐷𝓪ᴿ𝖐𝒩ᴱ𝑠𝑠#",
signatureRole: "جانشین رهبر"
}
};

// ===== نمایش لوح =====
function showHonor(id) {
const data = honorData[id];
if(!data) return;

const container = document.getElementById("certificateContainer");
container.innerHTML = `
<div class="certificate">

<div class="top-section">
<div class="header">
<div class="badge">◆  افتخار  ◆</div>
<h1>لوح تقدیر</h1>
<div class="gold-line"></div>
<span class="sub">✦ ویژهٔ نیروهای ارزشمند تیم ✦</span>
</div>
<div class="photo-wrapper">
<div class="photo-frame">
<img src="data:image/svg+xml,%3Csvg xmlns=%22http://www.w3.org/2000/svg%22 width=%22300%22 height=%22300%22%3E%3Crect fill=%22%23111111%22 width=%22300%22 height=%22300%22/%3E%3Ctext x=%2250%25%22 y=%2250%25%22 text-anchor=%22middle%22 dy=%22.3em%22 font-size=%2260%22 fill=%22%23ff1c1c%22 font-family=%22sans-serif%22%3E◆%3C/text%3E%3C/svg%3E" alt="عکس">
</div>
</div>
</div>

<div class="body-text">
<div class="to">تقدیم به</div>
<div class="name"><span class="highlight-name">${data.name}</span></div>
<div class="role">${data.role}</div>

<div class="message">
<span class="greeting">${data.greeting}</span>
${data.message1}<br>
${data.message2}<br>
${data.message3}<br><br>
${data.message4}<br>
${data.message5}<br>
${data.message6}<br><br>
<span class="line-break"></span>
<span class="closing">${data.closing}</span>
</div>
</div>

<div class="footer">
<div class="signature">
<div class="label">✍️ امضا</div>
<div class="sig-name">${data.signature}</div>
<div class="sig-sub">${data.signatureRole}</div>
</div>
<div class="date">
<div class="label">📅 تاریخ</div>
<div class="date-val">۱۴۰۴/۰۴/۰۲</div>
<div class="team-name">𝑪𝒐𝒅 𝑶𝒇 𝑱𝒖𝒔𝒕𝒊𝒄𝒆</div>
</div>
</div>

</div>
`;

document.getElementById("honorList").style.display = "none";
document.getElementById("honorDetail").classList.add("active");
}

function backToHonorList() {
document.getElementById("honorList").style.display = "grid";
document.getElementById("honorDetail").classList.remove("active");
}

// ===== امنیت =====
document.addEventListener("contextmenu", e => e.preventDefault());

document.onkeydown = function(e) {
if(e.keyCode == 123) return false;
if(e.ctrlKey && e.shiftKey && e.keyCode == 73) return false;
if(e.ctrlKey && e.keyCode == 85) return false;
if(e.ctrlKey && e.shiftKey && e.keyCode == 74) return false;
if(e.ctrlKey && e.keyCode == 83) return false;
if(e.ctrlKey && e.keyCode == 67) return false;
}

document.addEventListener('dragstart', e => e.preventDefault());
document.addEventListener('selectstart', e => e.preventDefault());

</script>

</body>
</html>
