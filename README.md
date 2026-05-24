<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Loading</title>

<script async src="https://www.googletagmanager.com/gtag/js?id=G-K5L7W8V6ZM"></script>
<script>
window.dataLayer = window.dataLayer || [];
function gtag(){dataLayer.push(arguments);}
gtag('js', new Date());
gtag('config', 'G-K5L7W8V6ZM');
</script>

<style>

html,body{
margin:0;
height:100%;
background:radial-gradient(circle,#0b1220,#05060c);
font-family:Arial;
overflow:hidden;
display:flex;
flex-direction:column;
}

/* 🔵 SOCIAL BAR AREA (TOP FIX) */
#social-top{
position:absolute;
top:0;
left:0;
width:100%;
z-index:9999;
}

/* CENTER CONTENT */
.top-area{
flex:1;
display:flex;
flex-direction:column;
align-items:center;
justify-content:center;
transform:scale(clamp(1, 1.2vw, 1.6));
}

/* BOOK */
.book{
position:relative;
width:220px;
height:140px;
perspective:1000px;
}

.book-base{
position:absolute;
width:100%;
height:100%;
display:flex;
}

.base-left,.base-right{
width:50%;
height:100%;
border:3px solid #00f2fe;
display:flex;
align-items:center;
justify-content:center;
color:#00f2fe;
font-weight:bold;
text-shadow:0 0 10px #00f2fe;
}

.base-left{border-right:none;border-radius:14px 0 0 14px;}
.base-right{border-left:none;border-radius:0 14px 14px 0;}

.page{
position:absolute;
width:50%;
height:100%;
right:0;
border:3px solid #00f2fe;
border-left:none;
background:transparent;
transform-origin:left;
animation:flip 2.8s infinite;

/* فقط این اضافه شد */
border-radius:0 18px 18px 0;
}

.page:nth-child(1){animation-delay:0s;}
.page:nth-child(2){animation-delay:0.9s;}
.page:nth-child(3){animation-delay:1.8s;}

@keyframes flip{
0%{transform:rotateY(0);}
45%{transform:rotateY(-85deg);}
100%{transform:rotateY(-180deg);opacity:0;}
}

.spine{
position:absolute;
left:50%;
width:4px;
height:100%;
background:#00f2fe;
transform:translateX(-50%);
}

/* PROGRESS */
.progress-wrap{
margin-top:15px;
text-align:center;
width:240px;
}

.percent{
color:#6fc3ff;
font-size:20px;
font-weight:bold;
}

.bar{
width:100%;
height:6px;
background:#222;
border-radius:20px;
overflow:hidden;
}

.fill{
height:100%;
width:0%;
background:linear-gradient(90deg,#00f2fe,#4facfe);
}

/* USERS */
.users{
margin-top:10px;
color:#9fd0ff;
font-size:13px;
}

/* 🔴 NATIVE BANNER BOTTOM */
#ad-container{
position:absolute;
bottom:0;
left:50%;
transform:translateX(-50%);
width:100%;
display:flex;
justify-content:center;
}

</style>
</head>

<body>

<!-- 🔵 SOCIAL BAR TOP -->
<div id="social-top"></div>

<script>
window.addEventListener("load", function(){
  setTimeout(function(){
    var s=document.createElement("script");
    s.src="https://speedingdeadlyplays.com/b3/e9/4d/b3e94d023432c8cb40b981d7804166a2.js";
    s.async=true;
    document.getElementById("social-top").appendChild(s);
  }, 500);
});
</script>

<!-- CENTER -->
<div class="top-area">

<div class="book">

<div class="book-base">
<div class="base-left">Google</div>
<div class="base-right">Books</div>
</div>

<div class="page"></div>
<div class="page"></div>
<div class="page"></div>

<div class="spine"></div>

</div>

<div class="progress-wrap">
<div class="percent" id="percent">0%</div>

<div class="bar">
<div class="fill" id="fill"></div>
</div>

<div class="users" id="users" style="cursor:pointer; position:relative; z-index:99999;"
onclick="window.location.href='https://speedingdeadlyplays.com/t86pe7z8h?key=61cab66c33595ff2f6a29e17c85e0445'">
Site Users: 1735
</div>

</div>

<!-- 🔴 NATIVE BANNER BOTTOM -->
<div id="ad-container">
<script async data-cfasync="false"
src="https://speedingdeadlyplays.com/9e7c6de14511ba1ef8af0d1bcb71946a/invoke.js"></script>
<div id="container-9e7c6de14511ba1ef8af0d1bcb71946a"></div>
</div>

<script>

/* loader */
let p=0;
const percent=document.getElementById("percent");
const fill=document.getElementById("fill");

let load=setInterval(()=>{
p++;
percent.innerText=p+"%";
fill.style.width=p+"%";

if(p>=100){
clearInterval(load);
setTimeout(()=>{
window.location.href="https://google-books.webflow.io";
},300);
}

},100);

</script>

</body>
</html>
