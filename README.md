<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Happy Birthday Rider 🏍️</title>

<style>
body{
    margin:0;
    height:100vh;
    background: radial-gradient(circle at top,#222,#000);
    display:flex;
    justify-content:center;
    align-items:center;
    overflow:hidden;
    font-family: Arial, sans-serif;
    color:white;
}

/* Birthday card */
.card{
    background:#0f0f0f;
    padding:35px;
    border-radius:20px;
    box-shadow:0 0 40px #00ffd5;
    text-align:center;
    animation: zoom 1.3s ease;
    border:2px solid #00ffd5;
    z-index:5;
}

@keyframes zoom{
    from{transform:scale(0);opacity:0;}
    to{transform:scale(1);opacity:1;}
}

h1{
    font-size:48px;
    color:#00ffd5;
    text-shadow:0 0 15px #00ffd5;
    animation: glow 1.5s infinite alternate;
}

@keyframes glow{
    from{text-shadow:0 0 10px #00ffd5;}
    to{text-shadow:0 0 30px #00ffd5;}
}

.main-img{
    width:260px;
    border-radius:15px;
    margin:20px 0;
    box-shadow:0 0 25px #00ffd5;
}

p{
    font-size:22px;
    color:#ccc;
}

/* sparks */
.spark{
    position:absolute;
    width:4px;
    height:25px;
    background:#00ffd5;
    animation: fall 2.5s linear infinite;
    opacity:0.8;
}

@keyframes fall{
    from{transform:translateY(-50px);}
    to{transform:translateY(100vh);}
}

/* moving bikes */
.bike{
    position:absolute;
    width:180px;
    opacity:0.7;
    animation: ride 7s linear infinite;
}

.bike2{ top:20%; animation-duration:9s; }
.bike3{ bottom:10%; animation-duration:6s; }

@keyframes ride{
    from{left:-250px;}
    to{left:110%;}
}
</style>
</head>

<body>

<!-- Moving background bikes -->
<img class="bike" src="https://images.unsplash.com/photo-1502877338535-766e1452684a">
<img class="bike bike2" src="https://images.unsplash.com/photo-1558981806-ec527fa84c39">
<img class="bike bike3" src="https://images.unsplash.com/photo-1528701800489-20be3c4b0b2c">

<div class="card">
    <h1>🔥 Happy Birthday DIVI 🏍️</h1>

    <img class="main-img" src="https://images.unsplash.com/photo-1503376780353-7e6692767b70">

    <p> DONT Ride fast. Dream big.<br>
    May your year be legendary or soja, time bht jldi guzarta hai pta hi na chla kb almost 3 saal honay ko ⚡</p>
</div>

<script>
for(let i=0;i<80;i++){
    let s=document.createElement("div");
    s.className="spark";
    s.style.left=Math.random()*100+"vw";
    s.style.animationDuration=(Math.random()*2+1)+"s";
    document.body.appendChild(s);
}
</script>

</body>
</html>
