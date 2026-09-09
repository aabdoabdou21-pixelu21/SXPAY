
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>آراء العملاء | SXPay</title>

<style>
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Arial,sans-serif;
}

body{
background:#050505;
overflow:hidden;
height:100vh;
display:flex;
justify-content:left;
align-items:left;
position:relative;
color:#fff;
}

body::before{
content:"";
position:absolute;
width:600px;
height:600px;
background:#00bfff;
filter:blur(180px);
opacity:.18;
animation:bgMove 8s infinite alternate;
}

@keyframes bgMove{
from{transform:translate(-200px,-120px);}
to{transform:translate(180px,120px);}
}

.container{
position:relative;
width:50%;
max-width:700px;
text-align:left;
z-index:2;
}

.logo{
font-size:55px;
font-weight:bold;
color:#00bfff;
letter-spacing:5px;
text-shadow:
0 0 10px #00bfff,
0 0 25px #00bfff,
0 0 50px #00bfff;
margin-bottom:10px;
}

.title{
font-size:34px;
margin-bottom:40px;
}

.review-box{
position:relative;
height:300px;
overflow:hidden;
}

.review{
position:absolute;
width:80%;
padding:30px;
border-radius:25px;
background:rgba(255,255,255,.06);
backdrop-filter:blur(15px);
border:1px solid rgba(255,255,255,.08);
opacity:0;
transform:translateY(120px) scale(.9);
transition:1s;
box-shadow:0 0 25px rgba(0,191,255,.15);
}

.review.active{
opacity:1;
transform:translateY(0) scale(1);
}

.avatar{
width:70px;
height:70px;
border-radius:50%;
background:#00bfff;
display:flex;
justify-content:left;
align-items:left;
font-size:28px;
font-weight:bold;
margin:auto;
margin-bottom:15px;
}

.name{
font-size:24px;
margin-bottom:8px;
}

.verify{
display:inline-block;
padding:5px 12px;
background:#00bfff;
border-radius:20px;
font-size:13px;
margin-bottom:15px;
color:#000;
font-weight:bold;
}

.stars{
font-size:24px;
color:#FFD700;
margin-bottom:18px;
animation:shine 1.5s infinite;
}

@keyframes shine{
50%{
transform:scale(1.08);
}
}

.text{
font-size:20px;
line-height:1.8;
color:#ddd;
}

.time{
margin-top:18px;
color:#888;
font-size:15px;
}

.stats{
display:flex;
justify-content:left;
gap:40px;
margin-top:50px;
flex-wrap:wrap;
}

.stat{
font-size:18px;
}

.stat strong{
display:block;
font-size:28px;
color:#00bfff;
margin-bottom:5px;
}

button{
margin-top:45px;
padding:16px 45px;
border:none;
border-radius:12px;
background:#00bfff;
color:#fff;
font-size:20px;
cursor:pointer;
transition:.3s;
}

button:hover{
transform:scale(1.06);
box-shadow:0 0 20px #00bfff;
}
</style>

</head>

<body>

<div class="container">

<div class="logo">SXPay</div>

<div class="title">
ماذا يقول عملاؤنا؟
</div>

<div class="review-box">

<div class="review active">
<div class="avatar">أ</div>
<div class="name">أحمد</div>
<div class="verify">✔ عميل موثق</div>
<div class="stars">★★★★★</div>
<div class="text">
وصلني الطلب خلال يومين، الجودة ممتازة والتغليف رائع.
</div>
<div class="time">قبل دقيقة</div>
</div>

<div class="review">
<div class="avatar">س</div>
<div class="name">سارة</div>
<div class="verify">✔ عملية شراء مؤكدة</div>
<div class="stars">★★★★★</div>
<div class="text">
أفضل متجر تعاملت معه، الأسعار ممتازة وخدمة العملاء رائعة.
</div>
<div class="time">قبل 4 دقائق</div>
</div>

<div class="review">
<div class="avatar">م</div>
<div class="name">محمد</div>
<div class="verify">✔ عميل موثق</div>
<div class="stars">★★★★★</div>
<div class="text">
أنصح الجميع بالتسوق من SXPay، تجربة ممتازة بكل المقاييس.
</div>
<div class="time">قبل 8 دقائق</div>
</div>

</div>

<div class="stats">

<div class="stat">
<strong>500</strong>
عميل سعيد
</div>

<div class="stat">
<strong>1k</strong>
طلب مكتمل
</div>

<div class="stat">
<strong>3.9★</strong>
متوسط التقييم
</div>

</div>

<button onclick="location.href='index.html'">
ابدأ التسوق
</button>

</div>

<script>
const reviews=document.querySelectorAll(".review");
let i=0;

setInterval(()=>{

reviews[i].classList.remove("active");

i++;

if(i>=reviews.length){
i=0;
}

reviews[i].classList.add("active");

},4000);
</script>

</body>
</html>

